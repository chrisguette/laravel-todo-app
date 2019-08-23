<template>
   <div class="card">
                    <div class="card-header">Activities</div>
                    <div class="card-header">Task added the {{ task.created_at }}</div>
    
                    <div class="card-body">
                        <h1>{{ task.title }}</h1>
                        <p>{{ task.description }}</p>
                    </div>
                    <div class="panel-footer">
                            <button class="btn btn-primary">Edit</button>
                            <button class="btn btn-danger">Delete</button>
                    </div>
                </div>
</template>

<script>
    export default {
        props: ['task'],
        data () {
            return {
               task: {
                   id: '',
                   description: '',
                   title: '',
                   created_at: ''
               }  
            };
        },
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>
