<template>
  <v-app>
    <v-container>
        <h2 class="heading-sec">
            <span class="heading-sec-main">ABOUT ME</span>
            <span class="heading-sec-sub">Here you will find more information about me, what I do, and my current skills mostly in terms of programming and technology</span>
        </h2>
        <v-row class="ma-5 mt-13">
            <v-col
          
             cols="12"
             md="6"
            >
                <h3  class="about-content-title ma-5">Get to know me!</h3>
                <div class="about-content-details ma-5">
                    <p class="about-content-details-para">
                        I'm a Frontend Focused Web Developer building and managing the Front-end of Websites and Web Applications that leads to the success of the overall product. Check out some of my work in the Projects section.
                    </p>
                    <p class="about-content-details-para">
                        I also like sharing content related to the stuff that I have learned over the years in Web Development so it can help other people of the Dev Community. Feel free to Connect or Follow me on my Linkedin and Instagram where I post useful content related to Web Development and Programming
                    </p>
                    <p class="about-content-details-para">
                        I'm open to Job opportunities where I can contribute, learn and grow. If you have a good opportunity that matches my skills and experience then don't hesitate to contact me.
                    </p>
                </div>
                <v-btn class="btn-bg ma-5">Contact</v-btn>
            </v-col>
            <v-col
           
             cols="12"
             md="6"
             
            >
                <!-- <h3  class="about-content-title">My Skills </h3> -->
                <div class="about-content-skills ma-5" >
            <h3 class="about-content-title">My Skills</h3>
            <div class="skills">
              <div class="skills__skill">HTML</div>
              <div class="skills__skill">CSS</div>
              <div class="skills__skill">JavaScript</div>
              <div class="skills__skill">React</div>
              <div class="skills__skill">Wordpress</div>
              <div class="skills__skill">PHP</div>
              <div class="skills__skill">SASS</div>
              <div class="skills__skill">GIT</div>
              <div class="skills__skill">Github</div>
              <div class="skills__skill">Responsive Design</div>
              <div class="skills__skill">SEO</div>
              <div class="skills__skill">Terminal</div>
            </div>
            </div>

            </v-col>
        </v-row>
    </v-container>
  </v-app>
</template>
<script>
export default {
    
}
</script>
<style scoped>
h1{
    display: flex;
    justify-content: center;
    align-items: center;
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
    padding: 1.4rem 2rem;
    font-size: 0.9rem;
    height: 3.5rem;
    margin-top: 4%;
}
.about-content-title{
    font-weight: 700;
    font-size: 1.8rem;
    margin-bottom: 3rem;
    color: #000000;
}
.about-content-details-para{
    font-size: 1.2rem;
    color: #666;
    max-width: 60rem;
    line-height: 1.7;
    margin-bottom: 1rem;
}
.heading-sec-main {
    display: block;
    font-size: 3rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    letter-spacing: 3px;
    text-align: center;
    margin-bottom: 3.5rem;
    position: relative;
    color: #000000;
}
.heading-sec-sub {
    display: block;
    text-align: center;
    color: #555;
    font-size: 1.2rem;
    font-weight: 400;
    max-width: 80rem;
    margin: auto;
    line-height: 1.6;
}
.skills {
    display: flex;
    flex-wrap: wrap;
}
.skills__skill {
    padding: 0.8rem 1.5rem;
    margin-bottom: 1.2rem;
    margin-right: 1.2rem;
    font-size: 1rem;
    background: rgba(153, 153, 153, 0.2);
    border-radius: 5px;
    font-weight: 500;
    color: #666;
}

.heading-sec-main::after {
    content: '';
    position: absolute;
    top: calc(100% + 1.5rem);
    height: 5px;
    width: 3rem;
    background: #7843e9;
    left: 50%;
    transform: translateX(-50%);
    border-radius: 5px;
}
</style>