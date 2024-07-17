<script>
export default {
    name: 'EquipeView',
    data() {
        return {
            equipe: [
                {
                    nome: 'João Vitor Guiotti',
                    cargo: 'Desenvolvedor'
                },
                {
                    nome: 'Gabriel Campregher Mohr',
                    cargo: 'Designer'
                },
                {
                    nome: 'Luiz Miguel Lima de Souza',
                    cargo: 'Gerente de Projetos'
                },
                {
                    nome: 'Brayan Pedroso de Mattos',
                    cargo: 'desenvolvedor'
                }
            ]
        }
    }
}
</script>

<template>
    <div>
        <h1>Equipe</h1>
        <ul>
            <li v-for="membro in equipe" :key="membro.nome">
                <h2>{{ membro.nome }}</h2>
                <p>{{ membro.cargo }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped>
/* Your component-specific styles go here */
</style>