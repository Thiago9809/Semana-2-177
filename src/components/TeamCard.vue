<template>
    <div>
            <div class="card text-white bg-dark">
                <div class="d-flex justify-content-center p-2">
                    <img :src="member.image" alt="Imag de integrante" width="200" height="200">
                </div>
                <div class="card-body">
                    <h5 class="card-title">{{member.nombre}}</h5>
                    <p class="card-text">{{member.descripcion}}</p>
                    <p class="card-text">Código: {{member.codigo}}</p>
                </div>
                <div class="card-footer">
                    <small class="text-muted">Rol:{{member.rol}}</small>
                </div>
            </div>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
