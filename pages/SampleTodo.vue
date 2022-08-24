<template>

    <TodosList :todos="my_todos" />

</template>


<script>

export default {
    data() {
        return {
            my_todos: [
                {
                    id:1,
                    title: "Clean the House",
                    desc: "The house should be cleaned before noon"
                },
                {
                    id:2,
                    title: "Read for Exam",
                    desc: "Hey rookie! You have an exam coming up tommorrow morning"
                }
            ]
        }
    }
}

</script> 

