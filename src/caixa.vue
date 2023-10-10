<template>
    <div class="cxa" v-if="contador<6">
        <div>
            caixa com nome {{ nome }}
        </div>
        <div>
            contador {{ contador }}
            <button @click="incrementa">
                Incrementar 
            </button>
        </div>
    </div>
</template>

<script>

export default {
    data() {
        return {
            contador: 1,
            nome: "Maria"
        }
    },
    methods: {
        incrementa() {
            this.contador++;
        }

    }
}

</script>

<style > .cxa {
     border: 1px solid black;
     padding: 2px;
     margin: 2px;
 }
</style>