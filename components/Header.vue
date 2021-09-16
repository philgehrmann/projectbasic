<template>
<div id="header" class=" mx-auto grid grid-cols-3 px-20 py-10 items-center">
    <div class="header__navbutton text-left">
        <div class="header__navbutton--wrapper  hover:bg-darktuerkis-lighter rounded-sm transition bg-opacity-25 duration-500 ">
            <div class="header__navbutton--item"></div>
        </div>
    </div>
    <div class="header__spacer text-center">b</div>
    <div class="header__logo text-right">c</div>
</div>
</template>

<script lang="ts">
export default  {
    data() {
        return {
            greeting: 'hello'
        }
    }
}
</script>

<style scoped lang="scss">
#header {
    width: 100%;
}

$nav-btn-width: 30px;
$color-main: #A1FCDF;
$color-sub: #7FD8BE;
$color-champagne: #FCD29F;
$color-rajah: #FCAB64;
$color-snow: #FCEFEF;


.header__navbutton--wrapper {
    width: 60px;
    height: 60px;
    display: grid;
    align-items: center;
    justify-items: center;
} 


.header__navbutton--item {
    position:relative;
    width: $nav-btn-width;
    height: 2px;
    background: #fff;
    &::after {
        content:"";
        position:absolute;
        background: #fff;
        width: $nav-btn-width;
        height: 2px;
        top: -5px;
    }
    &::before {
        content:"";
        position:absolute;
        background: #fff;
        width: $nav-btn-width;
        height: 2px;
        top: 5px;

    }

}
</style>

