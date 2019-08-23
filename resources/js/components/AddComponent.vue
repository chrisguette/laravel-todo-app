<template>
           <div class="card">
                <div class="card-header">Activities</div>

                <div class="card-body">
                  

                    <form action="" v-on:submit.prevent="newTask()">
                        <div class="form-group">
                            <label for="">Add task</label>
                            <input type="text" class="form-control" name="task" 
                            v-model="taskadded">
                            
                        </div>
                        <button type="submit" class="btn btn-primary">
                            Submit
                        </button>
                    </form>
                </div>
            </div>

</template>

<script>
    export default {
       data() {
           return {
               description: ''
           }
       },
       mounted() {
            console.log('Component mounted.')
        },
        methods: {
           newTask() {
             alert('Task added');    
           } 
        }
    }
</script>
