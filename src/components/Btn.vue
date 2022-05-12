<template>
<button class="[outlined,baseButton]"> <img :src="iconBefore"/> {{buttonText}} <img :src="iconAfter"/> </button>
</template>

<script>
export default {
    props: {
        
        buttonText: {
            type: String,
            default: () => "Default",
        },
        buttonIcon: {
            type: Image,
        },
        baseButton: {
            type: Boolean,
            default: () => true,
        },
        outlined: {
            type: Boolean,
            default: () => false,
        },
    },
};
</script>

<style scoped>

.baseButton {
    position: absolute;
    width: 81px;
    height: 36px;
    left: 319px;
    top: 141px;
    border:none;
    background: #E0E0E0;
    box-shadow: 0px 2px 3px rgba(51, 51, 51, 0.2);
    border-radius: 6px;
}
.baseButton:hover,.baseButton:focus {
    position: absolute;
    width: 81px;
    height: 36px;
    left: 319px;
    top: 141px;

    background: #AEAEAE;
    box-shadow: 0px 2px 3px rgba(51, 51, 51, 0.2);
    border-radius: 6px; 
}
.outlined {
    position: absolute;
    width: 88px;
    height: 36px;
    left: 319px;
    top: 246px;
    color:#3D5AFE;
    background-color: white;
    border: 1px solid #3D5AFE;
    border-radius: 6px;
}

.outlined:hover,.outlined:focus {
    position: absolute;
    width: 88px;
    height: 36px;
    left: 319px;
    top: 246px;
    background: rgba(41, 98, 255, 0.1);
    border: 1px solid #3D5AFE;
    border-radius: 6px;
}

.text {
    position: absolute;
    color:blue;
    width: 88px;
    height: 36px;
    left: 319px;
    top: 351px;
    border:none;
    background: white;
    border-radius: 6px;
}

.text:hover,.text:focus {
    position: absolute;
    color:blue;
    width: 88px;
    height: 36px;
    left: 319px;
    top: 351px;
    border:none;
    background: rgba(41, 98, 255, 0.1);
    border-radius: 6px;
}
.disableShadow {
    position: absolute;
    width: 81px;
    height: 36px;
    left: 319px;
    top: 453px;
    color:white;
    border:none;
    background: #3D5AFE;
    border-radius: 6px;
}
.disabled {
    position: absolute;
    width: 88px;
    height: 36px;
    left: 319px;
    top: 558px;
    border:none;
    background: #E0E0E0;
    border-radius: 6px;
}
.disabledText {
    position: absolute;
    width: 62px;
    height: 20px;
    left: 558px;
    top: 566px;
    color: #9E9E9E;
    border:none;
    background:white;
    border-radius: 6px;
}
</style>