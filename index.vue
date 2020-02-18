<template>
    <Legend checkbox :legend="legend" />
</template>
<script lang="ts">
import {Component, Emit, Prop, Vue} from 'vue-property-decorator';
import Legend from './Legend.vue'

export default class Page extends Vue {

    get legend() {
        return 32342
    }

}
</script>