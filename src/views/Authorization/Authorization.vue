<template>
    <div class="authorization">
        <div class="authorization__inner">
                <Registration />
                <!-- <Login /> -->
        </div>
    </div>
</template>

<script>
import Registration from './components/Registration.vue'
import Login from './components/Login.vue'
export default {
    components: {Registration, Login}
}
</script>

<style scoped lang="scss">
.authorization{
    height:100%;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    &__inner{
        max-height: 560px;
        height:100%;
        max-width:  800px;
        width: 100%;
        box-shadow: 2px 1px 7px 0px rgba(0,0,0,0.59);
        -webkit-box-shadow: 2px 1px 7px 0px rgba(0,0,0,0.59);
        -moz-box-shadow: 2px 1px 7px 0px rgba(0,0,0,0.59);
        border-radius: 5px
    }
}
</style>