<template>
    <div class="row">
        <div class="col-md-12 border off-set-md-3 d-flex flex-row justify-content-between align-items-center p-2 pb-2">
          <span class="font-weight-lighter">{{ todo.text }}</span>
          <button class="btn btn-danger" @click="$emit('deleteTodo', todo.id)">Delete</button>
        </div>
      </div>
</template>

<script>
export default {
    props: ["todo"]
}
</script>
