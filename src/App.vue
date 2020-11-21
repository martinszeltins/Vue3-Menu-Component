<template>
    <div style="position: absolute; right: 20px; bottom: 5px;">
        <dropdown-menu
            v-model="show">

            <button @click="show = !show">
                Click to open dropdown
            </button>

            <template v-slot:dropdown>
                <div class="menu-wrapper">
                    <div>Action</div>
                    <div>Another action</div>
                    <div>Something else here blah blah blah</div>
                    <div>Something else here</div>
                    <div>Something else here</div>
                    <div>Something else here</div>
                </div>
            </template>
        </dropdown-menu>
    </div>
</template>

<script>
    import { ref } from 'vue'
    import DropdownMenu from './components/DropdownMenu.vue'

    export default {
        components: { DropdownMenu },

        setup()
        {
            const show = ref(false)

            return { show }
        },
    }
</script>

<style>
    .menu-wrapper {
        background: #000;
        color: #fff;
    }
</style>