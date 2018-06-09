<template>
    <div class="modal">
        <i-p @click="modal1 = true">Click Here</i-p>
        <Modal
                v-model="modal1"
                title="A Modal"
                @on-ok="ok"
                @on-cancel="cancel">
            <h1> Hello VuePress</h1>

        </Modal>
    </div>
</template>
<script>
    import Vue from 'vue';
    import iView from 'iview';
    import 'iview/dist/styles/iview.css';
    import locale from 'iview/dist/locale/en-US';
    Vue.use(iView, {locale: locale});
    export default {
        data () {
            return {
                modal1: false
            }
        },
        methods: {
            ok () {
                this.$Message.info('Clicked ok');
            },
            cancel () {
                this.$Message.info('Clicked cancel');
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