<style scoped>
.text{
    position: middle;
    border: 50px;
    font-family:"DIN 2014";
    font-size: 40px;
    color:#323297;

}
@font-face {
     font-family: "DIN 2014";
     src: url(/DIN-2014.otf);
    }
</style>
<template>
    <div class="text">
        Hello TdA
    </div>
</template>

//.circle{
    position: middle;
    width: 80px;
    height: 80px;
    border-radius:50%;
}
.circle::before,
.circle:after{
    content:"";
    position: absolute;
    border-radius: inherit;
}
.circle:before{
        width: 100%;
        height: 100%;
        background-image:linear-gradient(
            0deg,#ff00cc 0%,
            #323297 100%);
        animation: spin .5s infinite linear;
}
.circle:after{
    width: 85%;
    height: 85%;
    background-color: rgb(1, 8, 17);
    top:50%;
    left:50%;
    transform: translate(-50%, -50%);
}
@keyframes spin {
    to {
        transform: rotate(360deg);
    }
}