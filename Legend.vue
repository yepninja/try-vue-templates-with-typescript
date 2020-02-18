<script lang="ts">
    import {Component, Emit, Prop, Vue} from 'vue-property-decorator';

    @Component
    export default class Legend extends Vue {
        @Prop(Boolean)
        public readonly checkbox!: boolean;

        @Prop({default: () => []})
        public legend!: string[];

        private isOpen: boolean = true;

        private toggle(): void {
            this.isOpen = !this.isOpen;
        }
    }
</script>
