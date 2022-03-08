<template>

    <div id="app">
        <h3>ToDos</h3>
        <div class="todos">
            <div class="todo" v-for="todo in allTodos" :key="todo.id">
                {{todo.title}}
            </div>
        </div>
    </div>
</template>

<script>
import { mapGetters } from 'vuex';

export default {
    name: "ToDos",
    computed:{
       ... mapGetters(['allTodos'])
    }
}
</script>

<style>

</style>
