<template>
  
    <div class="row justify-content-center">
        <div class="col-md-8">
           
                <add-component></add-component>
                <task-component 
                v-for="task in tasks" 
                :key="task.id"
                :task="task">
                </task-component>

        </div>
    </div>


</template>

<script>
    export default {
      data() {
          return {
              tasks:[{
                 'id': 1,
                 'description': 'abc',
                 'title': 'abc',
                 'created_at': '22/08/2019', 
              }]
          }
      },
      
      mounted() {
            console.log('Component mounted.')
        }
    }
</script>
