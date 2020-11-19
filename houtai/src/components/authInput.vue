<template>
        <input class="input" :type="type" @input="dataChange">
</template>

<script>
export default {
        props:[
                "type"
        ],
        data () {
                return {
                        rule: '\d{11}',
                        isOk: ture
                }
        },
        methods:{
                dataChange($event) {
                        var regex = new RegExp(this.rule);
                        
                        var isOk = regex.test($event.target.value) 
                }
        }
}
</script>
<style lang="less" scoped>
        .input{
               width: 200px; 
               height: 28px;
               padding: 10px;
               box-sizing: border-box;
               background: #fff;
               border: none;
               border-bottom: 2px solid #000;
               outline: none;
        }
</style>