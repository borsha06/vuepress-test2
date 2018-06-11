<template>
    <div class="modal">
        <i-button @click="modal">Click Here</i-button>
    </div>
</template>
<script>
    import Vue from 'vue';
    import iView from 'iview';
    import 'iview/dist/styles/iview.css';
    import locale from 'iview/dist/locale/en-US';
    import Swal from 'sweetalert2'
    Vue.use(iView, {locale: locale});
    export default {
        data () {
            return {
                modal1: false
            }
        },
        methods: {

            modal: function () {
                Swal('Hello world!')
            }
        }
    }

</script>
<style>
    .modal{
        color:#50b07c;
        font-size: 30px;
        cursor: pointer;
    }
</style>