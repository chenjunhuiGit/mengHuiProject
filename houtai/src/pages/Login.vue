<template>
    <div class="box1">
        <div class="head">
            <img src="../assets/timg.jpg" alt="">
        </div>

        <div class="inputName">
            <authInput type="text" placeholder="请输入账号"></authInput>
        </div>

        <div class="inputPwd">
            <authInput type="password" placeholder="请输入密码"></authInput>
        </div>

        <div class="btn">
            <button>登录</button>
        </div>
    </div>
</template>

<script>
import authInput from '../components/authInput'

export default {
    components:{
        authInput:authInput
    }
}
</script>

<style lang="less" scoped>
.box1{
    width: 100vw;
    padding-top: 20vh;
    .head{
        width: 80px;
        height: 80px;
        margin: 0 auto;
        border: 3px solid #000;
        border-radius: 50%;
        img{
            width: 100%;
            height: 100%;
            border-radius: 50%;
        }
    }
    .inputPwd,
    .inputName{
        padding-top: 20px;
        width: 200px;
        margin: 0 auto;
    }
    .btn{
        padding-top: 20px;
        width: 100px;
        margin: 0 auto;
    }
}
</style>