<template>
<v-app-bar app color="black" dark flat class="px-12">
    <v-btn style="width: 50px;">
        <v-avatar style="width: 70px; height: 40px;" >
            <v-img src="../../public/i13.png" left  style="height: 100%; object-fit: cover;"></v-img>
        </v-avatar>
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')" style="color:#9c3fc5">Home</v-btn>
    <v-btn text @click="scroll('sobre')">Sobre mim</v-btn>
    <v-btn text @click="scroll('profissional')">Profissional</v-btn>
    <!-- <v-btn text @click="scroll('atuacao')">Atuação</v-btn> -->
    <!-- <v-btn text @click="scroll('portifolio')">Portifólio</v-btn> -->
    <v-btn text @click="scroll('experiencia')">Experiência</v-btn>
    <v-btn text @click="scroll('contato')">Contato</v-btn>
</v-app-bar>
</template>

<script>
export default {
    methods: {
        scroll(refName) {
            const element = document.getElementById(refName);
            element.scrollIntoView({ behavior: 'smooth' });
        }
    }
}

</script>