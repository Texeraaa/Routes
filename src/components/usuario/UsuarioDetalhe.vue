<template>
    <div class="usuario-detalhe">
        <h3>Usuario Detalhe</h3>
        <hr>
        <p><strong>Código:</strong> {{  id  }}</p>
        <router-link tag="button" primario 
            :to="{ name: 'editarUsuario', params: { id },
                query: { completo : true, lingua: 'pt-br'},
                hash: '#rodape' }">
            Editar
        </router-link>
    </div>
</template>

<script>
export default {
    props: ['id'],
    beforeRouteEnter(to, from, next){
        console.log('dentro do componente -> usuario detalhe')
        next()
    }
    // data(){
    //     return{
    //         id: this.$route.params.id
    //     }
    // },
    // watch: {
    //     $route(to,from){
    //         this.id = to.params.id
    //     }
    // },
}
</script>

<style>

</style>