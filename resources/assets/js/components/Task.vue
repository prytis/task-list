<template>
        <tr>
            <td>{{ task.id }}</td>
            <td>{{ task.title }}</td>
            <td>{{ task.priority }}</td>
            <td><button @click="remove" class="btn btn-danger">RRRRRRRR</button></td>
        </tr>

</template>


<script>


    export default{

        data(){
            return{
            }

        },

        methods: {

            remove(){

                this.$emit('delete', this.task.id)

            }


        },


        props: ['task']


    }


</script>

<style>
</style>