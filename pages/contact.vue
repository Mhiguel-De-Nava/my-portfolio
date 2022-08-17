<template>
    <v-container>
        <v-row class="contacts">
            <v-col align-self=center class="contact">
                <p class="location"><v-icon>mdi-map-marker</v-icon> Based in Manila, Philippines</p>
                <p class="number"><v-icon>mdi-cellphone</v-icon> +639152376648</p>
                <p class="email"><v-icon>mdi-email</v-icon> mhiguelrovy.denava@gmail.com</p>
            </v-col>
            <v-col align-self=center class="social">
                <p class="social-media">Social Medias</p>
                <p class="media"><v-icon>mdi-facebook</v-icon> Facebook</p>
                <p class="media"><v-icon>mdi-linkedin</v-icon> LinkedIn</p>
                <p class="media"><v-icon>mdi-instagram</v-icon> Instagram</p>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {

}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Abel&family=Jost&family=Poppins:wght@200;400&display=swap');
.contact{
    margin: 20px;
    margin-left: 2rem;
}
.contact p{
    font-family: 'Jost', sans-serif;
    margin-top: 20px;
}
.contact .location{
    margin-top: 20px;
}
.social-media{
    font-weight: 500;
    letter-spacing: 2px;
    margin: 15px 20px 20px 20px;
    margin-left: 2rem;
}
.social .media{
    font-size: 16px;
    font-weight: 400;
    margin-left: 2rem;
}
.social .media .v-icon{
    margin: 0 5px 5px 0;

}
</style>