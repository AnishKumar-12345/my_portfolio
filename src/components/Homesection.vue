<template>  
  <div>    
    <v-section class="home-hero">
        <v-row>
        <v-col 
        cols="12" md="1"
        class="home-hero-social-wrapper"
         >
        <v-row class="home-hero-social">
            <v-col cols="12"><v-icon icon="mdi-linkedin" color="black" size="x-large"></v-icon></v-col>            
            <v-col cols="12"> <v-icon icon="mdi-github" color="black" size="x-large"></v-icon></v-col>
            <v-col cols="12"> <v-icon icon="mdi-instagram" color="black" size="x-large"></v-icon></v-col>
        </v-row>
        </v-col>
        <v-col cols="12" md="10">
            <div class="home-hero-content">
                <h1>Hey, I'm Anish Kumar Behera</h1>
                <p class="text">A Frontend focused Web Developer building the Frontend of Websites and Web Applications that leads to the success of the overall product</p>
            </div>
            <div class="home-hero-btn">
                <v-btn class="btn-bg">Projects</v-btn>
            </div>
            <div class="home-hero-mouse">
                <div class="mouse"></div>
            </div>
        </v-col>
    </v-row>
    </v-section>
  </div>   
</template>

<script>
export default {}
</script>

<style scoped>
.home-hero {
    color: #fff;
    background: linear-gradient(to right,rgba(245,245,245,.8),rgba(245,245,245,.8)),url(./src/assets/common-bg.svg);
    background-position: center;
    height: 100vh;
    min-height: 42rem;
    max-height: 30rem;
    position: relative;
    display: block;
    margin-top:-2.5%;
}
.home-hero-social-wrapper {
    display: block;
}

.home-hero-social {
    background-color: white;
    width: 70px;
    padding: 10px;
    margin-top: 160%;
}

.home-hero-content h1 {
    font-size: 3rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    text-align: center;
    color: #111;
    font-weight: 800;
    margin-top: 12%;
}

@media (max-width: 768px) {
    .home-hero-content h1 {
        font-size: 2.5rem;
    }
    .text {
        width: 100%;
        margin-left: 0;
    }
    .home-hero-social-wrapper {
        display: none;
    }
}

.text {
    color: #333;
    font-size: 1.3rem;
    text-align: center;
    width: 70%;
    line-height: 1.6;
    margin-left: 15%;
    margin-top: 3.6%;
}

.btn-bg {
    background: #7843e9;
    color: #fff;
    text-transform: uppercase;
    letter-spacing: 1px;
    display: inline-block;
    font-weight: 700;
    border-radius: 5px;
    box-shadow: 0 5px 15px 0 rgba(0,0,0,.15);
    transition: transform .3s;
    padding: 1.4rem 3rem;
    font-size: 1.4rem;
    height: 4.4rem;
    margin-top: 3.6%;
}

.home-hero-btn {
    justify-content: center;
    display: flex;
    align-items: center;
}

.home-hero-mouse {
    justify-content: center;
    display: flex;
    align-items: center;
    margin-top: 15%;
}

.mouse {
    width: 25px;
    height: 40px;
    border: 2px solid #333;
    border-radius: 60px;
    position: relative;
    overflow: hidden;
}

.mouse::before {
    content: '';
    width: 5px;
    height: 5px;
    position: absolute;
    top: 7px;
    left: 50%;
    transform: translateX(-50%);
    background-color: #333;
    border-radius: 50%;
    opacity: 1;
    animation: wheel 1.3s infinite;
    -webkit-animation: wheel 1.3s infinite;
}

@keyframes wheel {
    0%, 100% {
        opacity: 1;
        transform: translateY(0);
    }
    50% {
        opacity: 0.5;
        transform: translateY(10px);
    }
}

@-webkit-keyframes wheel {
    0%, 100% {
        opacity: 1;
        transform: translateY(0);
    }
    50% {
        opacity: 0.5;
        transform: translateY(10px);
    }
}
</style>
