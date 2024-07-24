<script>
export default {
    name: 'EquipeView',
    data() {
        return {
            equipe: [
                {
                    nome: 'João Vitor Guiotti',
                    cargo: 'Gerente de projetos'
                },
                {
                    nome: 'Gabriel Campregher Mohr',
                    cargo: 'Analista de sistemas'
                },
                {
                    nome: 'Luiz Miguel Lima de Souza',
                    cargo: 'Desenvolvedor'
                },
                {
                    nome: 'Brayan Pedroso de Mattos',
                    cargo: 'Desenvolvedor'
                },
                {
                    nome: 'Matheus Henrique Calsavara',
                    cargo: 'Designer'
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