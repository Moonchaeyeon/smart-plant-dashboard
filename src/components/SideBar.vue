<template>
<div class="side-bar">
    <div style="color: white; padding:20px; text-align:center; font-size:20px;">Smart M</div>
    <div class="menu">
        <div class="menu1">대시보드</div>
        <div class="menu2">
            <p @click="$router.push('/detection')">지능형 이상감지</p>
            <p>CCTV 영상인식</p>
            <p>IoT 모니터링</p>
        </div>
    </div>

    <div class="menu">
        <div class="menu1">IoT 관리</div>
        <div class="menu2">
            <p>센서 관리</p>
            <p>센서 위치 등록</p>
        </div>
    </div>

    <div class="menu">
        <div class="menu1">e-SOP 관리</div>
        <div class="menu2">
            <p>e-SOP 에디터</p>
            <p>담당자 관리</p>
            <p>문자메시지 기록</p>
        </div>
    </div>

    <div class="menu">
        <div class="menu1">이상 감지 관리</div>
        <div class="menu2">
            <p>이상 경고 설정</p>
            <p>이상 감지 이력</p>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'SideBar',
}
</script>

<style>

</style>