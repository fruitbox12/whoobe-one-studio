<template>
    <div ref="blockAction" class="flex flex-col p-2 pr-20">
        <label>Type</label>
        <select v-model="$store.state.editor.current.type">
            <option value="text">text</option>
            <option value="email">email</option>
            <option value="number">number</option>
        </select>
        <label>Name</label>
        <input type="text" v-model="$store.state.editor.current.data.attributes.name"/>
        <label>ID</label>
        <input type="text" v-model="$store.state.editor.current.data.attributes.id"/>
        <label>Placeholder</label>
        <input type="text" v-model="$store.state.editor.current.data.attributes.placeholder"/>
        <label>Required</label>
        <input type="checkbox" v-model="$store.state.editor.current.data.attributes.required"/>
    </div>
</template>

<script>
export default {
    name: 'BlockInput',
    mounted(){
        //let position = this.$refs.blockAction.getBoundingClientRect()
        //this.$emit('position',position.height)
    }
}
</script>