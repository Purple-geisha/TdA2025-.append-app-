
<style module>
.purple{
    font-style: italic;
    font-family: sans-serif;
    font-size: 100px;
    color:#d6970e;
    border: 4px dotted rgba(0, 0, 0, 0.315);
}
</style>
<template>
    <p :class="$style.purple">Hello TdA</p>
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