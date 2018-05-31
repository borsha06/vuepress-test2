<template>
    <div class="modal">
        <div class="modal" @click="modal">
            <strong>Click Here!!!</strong>
        </div>

    </div>


</template>
<script>
    import Swal from 'sweetalert2'
    export default{

        data(){
            return {

                message:"Hello Vuepress"
            }
        },
        methods: {


            modal: function () {
                Swal(this.message)            }
        }
    }

</script>
<style>
    .modal{
        color:#50b07c;
        font-size: 30px;
    }
</style>