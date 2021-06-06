<template>
  <input
    type="text"
    placeholder="Ingrese el nombre de la tareita"
    v-model.trim="task.description"
    />
  <input
    type="date"
    v-model="task.deadline"
    />
    <button>Agregar</button>
</template>

<script>
export default {
    props: {
        task: Object
    }
}
</script>

