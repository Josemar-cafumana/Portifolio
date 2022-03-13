<template>
  <footer class=" d-flex align-content-center justify-content-between">
        <p>@ 2022 - Josemar Cafumana</p>
        <p>Powered by <img src="../assets/logo-footer.svg" alt="logo footer"></p>
  </footer>
</template>

<script>
export default {
        name:"Footer"
}
</script>

<style lang="scss" scoped>
    footer{
        padding: 2rem 9rem;
        padding-bottom:.8rem ;
        background: var(--dark-200) !important;

        p{
             font-size: var(--font-size);
            color: var(--gray-light);

            img{
                width: 2rem;
            }
                   
        }
    }
</style>