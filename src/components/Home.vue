<template>
  <div style="display:flex;">
    <!--CCRV-->
    <div class="box" style="width: 300px; height:300px;">
        <div class="box_title">영상 분석</div>
        <div class="title_div"></div>
    </div>
    <!--복합 데이터-->
    <div class="box" style="position: absolute; bottom:0%; left: inherit;">
        <div class="box_title">복합 데이터 분석</div>
        <div class="title_div"></div>
    </div>
    <!--가스-->
    <div class="box" style="position: absolute; top:inherit; right:260px;">
        <div class="box_title">우드펠릿 버킷엘리베이터 1구역 - 가스</div>
        <div id="noise-chart1"></div>
        <div class="value_text" id="`">0</div>
    </div>
    <!--분진-->
    <div style="width: 250px; height: 100%; right:30px; position: absolute; display: flex; flex-direction: column;
    align-items: flex-end;">
        <div class="box">
            <div class="box_title">우드펠릿 버킷엘리베이터 2구역 - 분진</div>
            <div class="dust_circle">
                <div class="dust_circle" style="width:145px; height:145px; border-width: 4px; line-height: 120px; flex-direction:column;">
                    <div id="dustValue" style="font-weight: bold;">0</div>
                    <div style="font-size: 20px; color: white; line-height: 10%; position: relative; bottom: 15px;">mg/m<sup>3</sup></div>
                </div>
            </div>
        </div>
        <!--온도-->
        <div class="box" style="top: 10px;">
            <div class="box_title">우드펠릿 버킷엘리베이터 3구역 - 온도</div>
        </div>
        <!--습도-->
        <div class="box" style="top: 20px;">
            <div class="box_title">우드펠릿 버킷엘리베이터 2구역 - 습도</div>
            <div class="humid"></div>
            <div class="value_text" id="humidityValue" style="bottom: 50%;">0</div>
        </div>

        <div class="box" style="position: absolute; bottom: 0%; left:0px; width: 400px; height:200px;">
          <div class="box_title">알람이력</div>
          <div class="title_div"></div>
        <table class="table table-bordered dataex-html5-selectors">
            <thead>
                <tr>
                    <th rowspan="2" class="align-top">
                        발생일시
                    </th>
                    <th>유형</th>
                    <th>레벨</th>
                    <th>위치</th>
                    <th>구역</th>>

                    <th>맵구역</th>
                </tr>
            </thead>
        </table>

    </div>
  </div>
  </div>
</template>

<script>
export default {
name: 'Home',
}
</script>

<style>
	.box {
		background-color: #272e4890;
		opacity: 50;
		width: 230px;
		height: 250px;
		padding: 10px;
		overflow: visible;
		position: relative;
		border-radius: 5px;
		text-align: center;
	}

	.box_title {
		color: white;
		text-align: left;
		font-weight: bold;
		margin-top: 5px;
		margin-bottom: 10px;
	}

	.title_div {
		background-color: white;
		width: 100%;
		height: 1.5px;
		border-radius: 2px;
		opacity: 40;
	}

	.value_text {
		color: aqua;
		font-size: 40px;
		font-weight: bold;
		position: relative;
	}

	.dust_circle {
		width: 170px;
		height: 170px;
		border: 9px solid;
		border-radius: 50%;
		border-color: aqua;
		display: inline-flex;
		align-self: center;
		justify-content: center;
		color: aqua;
		font-weight: 8px;
		font-size: 40px;
		text-align: center;
	}

	.humid {
		width: 150px;
		height: 150px;
		border-radius: 0 50% 50% 50%;
		border: 3px solid black;
		transform: rotate(45deg);
		margin-top: 30px;
		margin-left: 30px;
		border-width: 9px;
		border-color: aqua;
	}


</style>