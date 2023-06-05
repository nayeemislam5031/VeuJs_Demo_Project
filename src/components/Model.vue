<template>
    <div class="backdrop">
        <div class="model">
            <h1>{{header}}</h1>
            <p>model content</p>
        </div>

    </div>
</template>


<script>
export default {
   props: ['header']
}
</script>


<style  scoped>
 .model{
    width: 404px;
    padding: 20px;
    margin: 100px auto;
    background: #fff;
    border-radius: 10px;
    color: black;
    text-align: center;
 }
 .backdrop{
    top: 0;
    position: fixed;
    background: #3f3e3e64;
    width: 100%;
    height: 100%;   
 }
 h1{
    color: rgb(179, 22, 179);
    border: none;
    padding: 0;
 }
 .model p{
    font-style: normal;
 }
</style>