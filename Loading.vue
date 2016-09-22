<script>
    import NProgress from 'nprogress';
    const install = (VueInstance) => {
        const $loader = {
            show() {
                NProgress.start();
            },
            hide() {
                NProgress.done();
            },
        };

        VueInstance.prototype.$loader = $loader;
    } ;

    export default {install};
</script>
