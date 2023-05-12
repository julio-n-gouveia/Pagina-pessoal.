<template>
<v-app-bar app color="black" dark flat class="px-12">
    <v-btn style="width: 50px;">
        <v-avatar style="width: 70px; height: 40px;" >
            <v-img src="../assets/13.png" left  style="height: 100%; object-fit: cover;"></v-img>
        </v-avatar>
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')" style="color:#9c3fc5">Home</v-btn>
    <v-btn text @click="scroll('sobre')">Sobre</v-btn>
    <v-btn text @click="scroll('potifolio')">Potifólio</v-btn>
    <v-btn text @click="scroll('seviços')">Seviços</v-btn>
    <v-btn text @click="scroll('paginas')">Páginas</v-btn>
    <v-btn text @click="scroll('biografia')">Biográfia</v-btn>
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