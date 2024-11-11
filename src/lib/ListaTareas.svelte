<script>
    let task='';
    let priority='meida'; //Por defecto, prioridad media
    let tasks=[];

    function addTaskPuh(){
        task=task.push({text:tasks, priority});
    }

    //Función para agregar una nueva tarea
    function addTask(){
        tasks = [
            ...tasks,
            {text: addTask, priority}
        ];
        task ='';
        priority='media'; //Reinicia el campo de prioridad
        sortTasks();
    }
</script>