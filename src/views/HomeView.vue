<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-grey">Olá, tudo bem?</h1>
              <h1 class="text-white">Sou Julio Gouveia</h1>
              <span class="text-grey">Engenheiro de Software</span> <br />
              <v-btn tile dark class="mt-8 texto-roxo" variant="outlined">Fale comigo</v-btn>
            </div>
          </v-col>
          <v-col cols="2">
            <div style="position: absolute; z-index: 9999; bottom: 0; margin-left:auto; margin-right: auto; left: 0; right: 0; text-align: center;">
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="3">
            <div style="position: relative; z-index: 9999;" class="mt-16">
              <v-img src="../../public/i24.png" contain max-height="300" class="minha-foto"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" class="mt-16" id="sobre">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="ovo">
                <v-img src="../../public/i25.png"></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
                <h5 class="mt-16">Sobre mim</h5>
                <div style="width: 120px;">
                  <v-slider v-model="slider2" color="#9c3fc5" label="">

                  </v-slider>
                </div>
                <h4 class="mt-n4">Engenheiro de Software criativo</h4>
                <h4>e dedicado.</h4>
                <p class="text-grey">Sou uma pessoa apaixonada por criação, inovação e conhecimento, movida pela reinterpretação de paradigmas e pela busca constante por novos pontos de vista. Na minha carreira profissional, apresento resultados reconhecendo e resolvendo problemas de diferentes ângulos, sempre em busca de mais aprendizado. O motivo mais genuíno que me levou à área de tecnologia é o desejo de trazer qualidade de vida para as pessoas, utilizando meu conhecimento e habilidades para impactar positivamente a sociedade e criar soluções inovadoras que facilitem tarefas, melhorem processos e ampliem possibilidades.</p>
              <br />
                <p class="text-grey">Acredito na importância da diversidade de perspectivas e estou sempre aberto a explorar novas ideias e desafiar o status quo. Valorizo o trabalho em equipe e a colaboração, pois acredito que é através da união de habilidades e compartilhamento de ideias que podemos alcançar resultados significativos. Estou determinado a deixar um legado positivo, utilizando minha paixão pela criação, inovação e conhecimento para fazer a diferença na vida das pessoas e contribuir para um mundo melhor. Continuarei aprendendo, evoluindo e buscando soluções que tragam praticidade, bem-estar e qualidade de vida por meio da tecnologia.</p>
                <v-btn tile dark color="#9c3fc5" class="mt-4" download href="../assets/Julio Cesar N.  Gouveia - CV - geral.pdf">Download Curriculo</v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <div class="text-center mt-4">
        <h2 >Profissional</h2>
        <h5 class="text-grey">Minhas habilidades:</h5>
        <div style="width: 120px; margin: 0 auto">
          <v-slider v-model="slider2" color="#9c3fc5" label=""></v-slider>
        </div>
      </div>
      <v-col cols="12" class="padd" id="portifolio">
        <div class="primeiro" id="projetos">
          <v-row>
            <v-col cols="16">
              <div class="filho">
                <v-btn icon="fas fa-laptop" color="#9c3fc5" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Front-End</h3>
                <p class="text-grey ml-3 mt-4 text-caption">Com Vue.js e Quasar: interfaces interativas,<br /> responsivas e focadas na experiência do usuário.
                </p>
              </div>
              <div class="filho">
                <v-btn icon="fas fa-server" color="#9c3fc5" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Back-End</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Back-end em Java e Spring Boot: sistemas robustos,<br />  escaláveis e APIs eficientes e seguras.
                </p>
              </div> 
              <div class="filho">
                <v-btn icon="fas fa-database" color="#9c3fc5" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Data Science</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Data Science com Python, SQL, Pandas: análise e <br />manipulação de dados.  Power BI para visualização<br /> e insights valiosos.
                </p>
              </div>
            </v-col>
          </v-row>
          <v-divider></v-divider>
        </div>
      </v-col>
      <!-- <v-col cols="12" sm="12" id="portifolio">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#da85ff" class="mr-2">Todos</v-btn>
          <v-btn class="mr-2" variant="tonal"> Dev Front-End</v-btn>
          <v-btn class="mr-2" variant="tonal">Dev Back-End</v-btn>
          <v-btn class="mr-2" variant="tonal">Dev Full-Stack</v-btn>
        </div>
      </v-col>
      <v-col cols="12" class="imgHover">
        <v-row class="fill-height" align="center" justify="center">
          <template v-for="(item, i) in itens" :key="i">
            <v-col cols="12" md="4">
              <v-hover v-slot="{isHovering, props}">
                <v-card :elevation="isHovering ? 12:2" :class="{'on-hover' : isHovering}" v-bind="props">
                  <v-img :src="item.img" height="225px"></v-img>
                </v-card>
              </v-hover>
            </v-col>
          </template>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#da85ff" class="mt-4">Mostrar mais</v-btn>
        </div>
      </v-col> -->
      <!-- componente abaixo vai ser minhas maginas, ou seja meu portifolio -->
      <v-col cols="12" id="experiencia">
        <div class="pre">
          <v-row>
            <v-col cols="12" sm="4">
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="i14.png" height="200px" cover></v-img>
                <v-card-title>Template 1</v-card-title>
                <v-card-subtitle>
                  Função
                </v-card-subtitle>
                <v-card-text>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                  Quisquam, voluptatum. Quisquam, voluptatum.
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="i23.png" height="200px" cover></v-img>
                <v-card-title>Template 2</v-card-title>
                <v-card-subtitle>
                  Função
                </v-card-subtitle>
                <v-card-text>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                  Quisquam, voluptatum. Quisquam, voluptatum.
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4" >
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="i22.png" height="200px" cover></v-img>
                <v-card-title>Template 3</v-card-title>
                <v-card-subtitle>
                  Função
                </v-card-subtitle>
                <v-card-text>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                  Quisquam, voluptatum. Quisquam, voluptatum.
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <!-- o componente a baixo vai ser minhas experiencias -->
      <v-col cols="12" id="experiencia">
        <div class="contratado">
          <v-row>
            <v-col cols="12" sm="8">
              <h1 class="mt-9">Me contrate para seu projeto</h1>
              <p class="text-grey">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                Quisquam, voluptatum. Quisquam, voluptatum.
              </p>
            </v-col>
            <v-col cols="12" sm="4">
              <v-btn color="#da85ff" class="mt-15">Contrate-me</v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" sm="12" class="px-16" id="contato">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="filho">
              <h1>Infomações de contato</h1>
              <v-btn icon="fas fa-map-marker-alt" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">Rua: 0000, Bairro: 0000, Cidade: 0000</span><br />
              <v-btn icon="fas fa-phone-alt" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">+55 00 0000-0000</span><br />
              <span class="text-caption">+55 00 0000-0000</span><br />
              <v-btn icon="fas fa-envelope" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">gouveia.cesar07@gmail.com</span><br />
              <span class="text-caption">gouveia.cesar07@gmail.com</span><br />
            </div>
          </v-col>
          <v-col cols="12" sm="8">
            <h1 class="mt-8">Fale comigo</h1>
            <v-divider></v-divider>
            <span class="text-caption">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Molestiae esse enim excepturi tempora laboriosam cupiditate sit ducimus, laborum deserunt blanditiis illum soluta voluptates nisi reiciendis veritatis sunt veniam ipsam unde!
            </span>
            <v-row class="mt-10">
              <v-col cols="12" sm="6">
                <v-text-field label="Nome" persistent-hint variant="outlined"></v-text-field>
              </v-col>
              <v-col cols="12" sm="6">
                <v-text-field label="Seu Telefone" persistent-hint variant="outlined"></v-text-field>
              </v-col>
            </v-row>
            <V-textarea label="Mensagem" persistent-hint variant="outlined"></V-textarea>
            <v-btn color="#da85ff" class="mt-10">Enviar</v-btn>
          </v-col>
        </v-row>
      </v-col>
    </v-container>
  </v-app>
</template>

<script>
import { defineComponent } from 'vue';

// Component
import NavBar from '@/components/NavBar.vue';

export default defineComponent({
  name: 'HomeView',
  setup() {
    return {
      slider2: 50,
      itens: [
        { img: "i14.png" },
        { img: "i23.png" },
        { img: "i22.png" }
      ],
    }
  },

  components: {
    NavBar
  },
  mounted() {
      document.title = 'Julio Gouveia';
  }
});
</script>
<style scoped>
.v-container {
  padding: 16px 0;
}
.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  widows: 100%;
  color: white;
}
.head::before {
  content: " ";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}
.head::after {
  content: " ";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}
.texto-roxo {
  color: #9c3fc5;
}
.minha-foto {
  border-radius: 100%;
  background-color: #9c3fc5;
}
.ovo {
display: block;
margin-left: 100px;
margin-top: 50px;
width: 365px;
height: 300px;
background-color: #da85ff;
border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;;
}
.primeiro{
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 2rem 2rem;
}
.filho{
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}
.imgHover{
  padding: 0 200px;
}
.pre{
  width: 100%;
  height: 380px;
  text-align: center;
  padding: 0 200px;
  background-color: #f5f5f5f5;
}
.contratado{
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #e9e9e9;
  margin-top: -24px;
}

</style>