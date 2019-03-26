<template>
    <div v-on:click="opa">
        {{a}}
        <slot></slot>
    </div>
</template>

<script>
export default {
    data: function(){
        return {a: 1}
    },
    props:{
        'texto': String
    },
    methods:{
        opa(){
            this.a = 9;
            alert("teste");
        }
    }
}
</script>

<style scoped>
div{
    background-color: #aaa
}
</style>
