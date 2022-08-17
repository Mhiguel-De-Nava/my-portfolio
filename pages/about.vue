<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-container class="about-img">
        <img src="../assets/Sketch1.png" alt="">
      </v-container>
    </v-col>
    <v-col cols="12" sm="8" md="6">
      <v-card elevation=4 id="about-title">
        <v-card-title  class="headline-about">
          About Me
        </v-card-title>
        <hr/>
        <v-card-text>
          <p align="justify" class="about-text">
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I am IT Fresh Graduate from Technological University of the Philippines - Manila. Aspiring to be a Web and Mobile Developer or an CCNA Professional. 
            However, I'm more currently focused on the Frontend side development of websites and mobiles being eager to learn various UI Frameworks and development tools while also
            honing my skills in the Backend develpment. Moreover, I'm an Tech enthusiast in which im also eager to learn networking as such I have knowledge on:
          </p>
          <p class="about-text">- Basic networking <br>- HTML & CSS<br>- Manual Testing<br> - Hardware Troubleshooting<br>- Object Oriented Programming
          </p>
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {

}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Abel&family=Jost&family=Poppins:wght@200;400&display=swap');
.row{
  margin: 20px;
}
.about-img{
  text-align: center;
  /* opacity: 50%; */
}
#about-title{
  background: rgb(61, 61, 61);
  border-radius: 20px;
  padding: 10px;
}
.headline-about{
  justify-content: center;
  font-size: 30px;
}
.about-text{
  font-family: 'Jost', sans-serif;
  font-size: 18px;
  line-height: 30px;
}
hr { 
  display: block;
  margin-bottom: 0.5em;
  margin-left: auto;
  margin-right: auto;
  border-style: inset;
  border-width: 1px;
  width: 40%;
}
</style>