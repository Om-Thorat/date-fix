<template>
  <!--  Navigation Section-->

  <Nav/>


  <!--  Landing Section-->


  <div class="home" id="home">
    <div class="container">
      <p id="heading">Aperta Fons</p>
      <p id="subH">A Month Long Open Source Challenge</p>
      <p id="text">Presented by The Programming Club, IIITDMJ</p>
      <div class="buttonContainer">
        <router-link to="/auth" style="text-decoration: none; color: inherit;">
          <button  class="button hvr-grow">
            <img src="../assets/register.svg" alt="register"/>
            <p>{{ user ? "Dashboard" : "Login" }}</p>
          </button>
        </router-link>
        <a target="_blank" href="https://discord.gg/c3WWbdf983" style="text-decoration: none">
          <button class="button hvr-grow">
            <img src="../assets/discord.svg" alt="discord" />
            <p>Discord</p>
          </button>
        </a>
      </div>
      <p id="start">The contest is now live until</p>
      <div class="timer" id="timer">
        <Confetti/>
        <span
        ><span> {{days}} </span> Days</span
        ><span>
          <span> {{hours}} </span> Hours</span
      ><span>
          <span> {{mins}} </span> Minutes</span
      ><span>
          <span> {{secs}} </span> Seconds</span
      >
      </div>
    </div>
  </div>

  <!--  About Section-->


  <div class="about-section" id="about">
    <div id="particles-js"></div>
    <div class="about">
      <h1 class="about-heading">About</h1>
      <div class="about-content">
        <p>
          Aperta Fons is a
          <span class="highlight">month-long open source event</span>, that is
          aimed at encouraging you towards the world of open-source and taking
          the first step towards licentious open-source programs like
          <span class="highlight">Outreachy, Google Summer of Code, MLH,</span>
          etc. This event is managed by BitByte, The Programming Club and Google
          DSC of IIITDM Jabalpur.
        </p>
        <p>
          This event is aimed at matching you with open source, free software,
          and technology-related organizations to write code and become part of
          these communities. The organizations provide mentors who act as guides
          through the entire process, from learning about the community to
          contributing code.
        </p>
        <p>
          The goals of our Event are to:
          <br/>
          - <span class="highlight">Inspire</span> you to begin participating in
          open source development.
          <br/>
          - <span class="highlight">Identifying</span> open-source projects and
          bring in new developers.
          <br/>
          - <span class="highlight">Provide</span> you the opportunity to do
          work and give you industry experience.
          <br/>
          - <span class="highlight">Give</span> you more exposure to real-world
          software development
        </p>
      </div>
    </div>
  </div>

  <!--  Prize Section-->


  <div class="prize-section" id="prize">
    <div class="prize">
      <h1 class="prize-heading">
        What's in it for you?
      </h1>
      <div class="prizes">
        <div class="list">
          <p>
            &bull; <span class="bolder">TOP CONTRIBUTORS</span> can win
            exclusive club t-shirts.
          </p>
          <p>
            &bull;
            <span class="bolder">EVERY CONTRIBUTOR</span> who has got at least 2
            easy-level and 1 medium-level PR merged to repositories with 100+⭐
            will get exclusive club stickers.
          </p>
          <p style="margin: 0 0 10px;">
            <span class="bolder">NOT ENOUGH?</span>
          </p>
          <p style="margin: 0">
            &bull; Top participants will get
            <span class="bolder"
            >Exclusive swags and merchandise</span
            >
            for their exceptional performance in the event.
          </p>
        </div>
      </div>
    </div>
  </div>

  <!--  FAQ Section-->

  <div class="faq" id="faq">
    <p class="faq_head">FAQS</p>
    <div class="accordion" id="accordionExample">
      <div class="accordion-item bg-black">
        <h2 class="accordion-header" id="headingOne">
          <button class="accordion-button bg-black collapsed" type="button" style="color: #ffffff;"
                  data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true"
                  aria-controls="collapseOne">
            Why should I participate?
          </button>
        </h2>
        <div id="collapseOne" class="accordion-collapse collapse" aria-labelledby="headingOne"
             data-bs-parent="#accordionExample">
          <div class="accordion-body" style="color : #FFFFFF">
            <strong>Ans. </strong>Participating in such events provides an amazing learning experience, helps in
            improving your development skills, getting involved in big organizations and helping to build networks. This
            is a great place to get you jump-started and up to speed with various industry-demanded technologies and
            getting involved with some great Open Source communities.
          </div>
        </div>
      </div>
      <div class="accordion-item bg-black">
        <h2 class="accordion-header">
          <button class="accordion-button bg-black collapsed" type="button" style="color: #ffffff; outline: none"
                  data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false"
                  aria-controls="collapseTwo">
            Why is Open Source important?
          </button>
        </h2>
        <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo"
             data-bs-parent="#accordionExample">
          <div class="accordion-body" style="color : #FFFFFF">
            <strong>Ans. </strong> Open source provides you first-hand experience with working on big and real-world
            projects, on which many top companies depend, which will give a huge boost in your development career. Not
            only this, but you also get to work with and learn from some of the most talented developers around the
            world.
          </div>
        </div>
      </div>
      <div class="accordion-item bg-black">
        <h2 class="accordion-header" id="headingThree">
          <button class="accordion-button bg-black collapsed" type="button" style="color: #ffffff"
                  data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false"
                  aria-controls="collapseThree">
            Are there any placement opportunities available?
          </button>
        </h2>
        <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree"
             data-bs-parent="#accordionExample">
          <div class="accordion-body" style="color : #FFFFFF">
            <strong>Ans. </strong>Contributing to some real world project will have a huge impact on your CV and you
            will gain some experience about how to work in a large organisation with hundreds of contributors. Though
            direct placement opportunities are rare, there are chances to get full time opportunities in the
            organisation you’re contributing for a long time. Mentors often recommend contributors to some startup
            companies or you might get to know people who work in FAANG companies which can help you later on when you
            apply to those companies with referral.
          </div>
        </div>
      </div>
      <div class="accordion-item bg-black">
        <h2 class="accordion-header" id="headingFour">
          <button class="accordion-button bg-black collapsed" type="button" style="color: #ffffff"
                  data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="false"
                  aria-controls="collapseFour">
            Can we work in groups to participate in this event?
          </button>
        </h2>
        <div id="collapseFour" class="accordion-collapse collapse" aria-labelledby="headingFour"
             data-bs-parent="#accordionExample">
          <div class="accordion-body" style="color : #FFFFFF">
            <strong>Ans. </strong>No, team participation is not allowed in this event. Everyone must participate
            individually. But you can collaborate with each other if contributing to the same organization.
          </div>
        </div>
      </div>
      <div class="accordion-item bg-black">
        <h2 class="accordion-header" id="headingFive">
          <button class="accordion-button bg-black collapsed" type="button" style="color: #ffffff"
                  data-bs-toggle="collapse" data-bs-target="#collapseFive" aria-expanded="false"
                  aria-controls="collapseFour">
            How do I submit my pull requests on Event Website?
          </button>
        </h2>
        <div id="collapseFive" class="accordion-collapse collapse" aria-labelledby="headingFive"
             data-bs-parent="#accordionExample">
          <div class="accordion-body" style="color : #FFFFFF">
            <strong>Ans. </strong>Head over to the Submit PR tab on your dashboard and fill the form accordingly.
          </div>
        </div>
      </div>
      <div class="accordion-item bg-black">
        <h2 class="accordion-header" id="headingSix">
          <button class="accordion-button bg-black collapsed" type="button" style="color: #ffffff"
                  data-bs-toggle="collapse" data-bs-target="#collapseSix" aria-expanded="false"
                  aria-controls="collapseSix">
            I am stuck. How do I get help?
          </button>
        </h2>
        <div id="collapseSix" class="accordion-collapse collapse" aria-labelledby="headingSix"
             data-bs-parent="#accordionExample">
          <div class="accordion-body" style="color : #FFFFFF">
            <strong>Ans. </strong>Join our discord server (<a href="https://discord.gg/c3WWbdf983"
                                                                style="color: #3770ff">click here to join</a>) and the
            mentors would be glad to help you there.
          </div>
        </div>
      </div>
      <div class="accordion-item bg-black">
        <h2 class="accordion-header" id="headingSeven">
          <button class="accordion-button bg-black collapsed" type="button" style="color: #ffffff"
                  data-bs-toggle="collapse" data-bs-target="#collapseSeven" aria-expanded="false"
                  aria-controls="collapseSix">
            Do I need to pay to enter this event?
          </button>
        </h2>
        <div id="collapseSeven" class="accordion-collapse collapse" aria-labelledby="headingSeven"
             data-bs-parent="#accordionExample">
          <div class="accordion-body" style="color : #FFFFFF">
            <strong>Ans. </strong> No purchase/payment is necessary to participate or win in this event. It is free of
            cost.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

import {ref} from "vue";
import Nav from "@/components/Nav";
import Confetti from "@/components/Confetti"
import {projectAuth} from "@/firebase/config";

export default {
  name: "Home",
  components: {Nav,Confetti},
  mounted() {
    this.initParticles()
  },
  methods: {
    initParticles() {
      window.particlesJS("particles-js", {
        "particles": {
          "number": {
            "value": 80,
            "density": {
              "enable": true,
              "value_area": 700
            }
          },
          "color": {
            "value": "#ffffff"
          },
          "shape": {
            "type": "circle",
            "stroke": {
              "width": 0,
              "color": "#000000"
            },
            "polygon": {
              "nb_sides": 5
            },
          },
          "opacity": {
            "value": 0.5,
            "random": false,
            "anim": {
              "enable": false,
              "speed": 1,
              "opacity_min": 0.1,
              "sync": false
            }
          },
          "size": {
            "value": 3,
            "random": true,
            "anim": {
              "enable": false,
              "speed": 40,
              "size_min": 0.1,
              "sync": false
            }
          },
          "line_linked": {
            "enable": true,
            "distance": 150,
            "color": "#ffffff",
            "opacity": 0.4,
            "width": 1
          },
          "move": {
            "enable": true,
            "speed": 6,
            "direction": "none",
            "random": false,
            "straight": false,
            "out_mode": "out",
            "bounce": false,
            "attract": {
              "enable": false,
              "rotateX": 600,
              "rotateY": 1200
            }
          }
        },
        "interactivity": {
          "detect_on": "canvas",
          "events": {
            "onhover": {
              "enable": true,
              "mode": "grab"
            },
            "onclick": {
              "enable": true,
              "mode": "push"
            },
            "resize": true
          },
          "modes": {
            "grab": {
              "distance": 140,
              "line_linked": {
                "opacity": 1
              }
            },
            "bubble": {
              "distance": 400,
              "size": 40,
              "duration": 2,
              "opacity": 8,
              "speed": 3
            },
            "repulse": {
              "distance": 200,
              "duration": 0.4
            },
            "push": {
              "particles_nb": 4
            },
            "remove": {
              "particles_nb": 2
            }
          }
        },
        "retina_detect": true
      })
    }
  },

  setup() {

    // a sleep function to use in async function with await
    function sleep(ms) {return new Promise(resolve => setTimeout(resolve, ms));}

    const days = ref(24);
    const hours = ref(24);
    const mins = ref(24);
    const secs = ref(24);
    const countDownDate = new Date("January 05 2024 00:00:00").getTime();
    
    // Update the count down every 1 second
    async function Countdown() {
        // Get today's date and time
        while (true){
          const now = new Date().getTime();
          // Find the distance between now and the count down date
          const distance = countDownDate - now;

          // Time calculations for days, hours, minutes and seconds
          days.value = Math.floor(distance / (1000 * 60 * 60 * 24));
          hours.value = Math.floor(
              (distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)
          );
          mins.value = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
          secs.value = Math.floor((distance % (1000 * 60)) / 1000);

          await sleep(1000);
        }
      }
    // function to countdown and blow confetti
    async function CountdownConfetti(){
      while(secs.value >0){
        days.value -= 1;
        hours.value -= 1;
        mins.value -= 1;
        secs.value -= 1;
        await sleep(30);
      }
      for(let i = 0;i<100;i++){
        Confetti.methods.frame()
        await sleep(2)
      }
      // The timer until end is triggered after the effect
      Countdown()
    }
    // confetti is triggered first
    CountdownConfetti()

    const user = projectAuth.currentUser

    return {days, hours, mins, secs, user};
  },
};
</script>

<style scoped>
.home {
  height: 100vh;
  background-image: url("../assets/home-bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.container {
  margin-left: 38vw;
  padding: 23vh 0 0 0;

  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

#heading {
  margin: 0;
  font-family: "Stargaze", serif;
  font-size: 12.4vh;
  line-height: 14vh;
  color: #fff;
  background: none;
  text-align: left;
}

#subH {
  font-family: "Stargaze", sans-serif;
  font-size: 4.2vh;
  line-height: 5.2vh;
  color: #fff;
  font-weight: initial;
  text-align: left;
  margin: 2vh 0 0 0;
}

#text {
  font-family: "Poppins", sans-serif;
  font-size: 2.3vh;
  line-height: 3.3vh;
  color: #ffffff;
  text-align: left;
  margin: 1.2vh 0 0 0;
}

.button {
  background: #3770ff;
  border-radius: 8px;
  width: fit-content;
  margin-right: 5vw;
  font-size: 1.5vw;
  padding: 1vh 2.5vw;
  color: #ffffff;
  display: flex;
  font-family: "Poppins", sans-serif;
  text-align: center;
  border: none;
  outline: none;
  cursor: pointer;
}

.buttonContainer button p {
  margin-bottom: 0;
}

.hvr-grow {
  transform: translateZ(0);
  box-shadow: 0 0 1px rgba(0, 0, 0, 0);
  backface-visibility: hidden;
  -moz-osx-font-smoothing: grayscale;
  transition-duration: 0.3s;
  transition-property: transform;
}

.hvr-grow:hover,
.hvr-grow:focus,
.hvr-grow:active {
  transform: scale(1.03);
}

.button img {
  margin-right: 1vw;
}

.buttonContainer {
  padding-top: 10vh;
  display: inline-flex;
  text-align: left;
}

.about-section {
  width: 100vw;
  background-color: #040509;
}

.about {
  overflow-x: hidden;
  color: #fff;
  height: 100vh;
  width: 72%;
  text-align: left;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: auto auto 0;
}

.about-heading {
  font-family: Stargaze, sans-serif;
  margin: 0;
  padding: 5vh 0;
  font-style: normal;
  font-weight: normal;
  font-size: 5.5vw;
  line-height: 10.6vh;
  align-items: center;
  text-align: center;
}

.about-content {
  font-family: Poppins, sans-serif;
  line-height: 4vh;
  font-size: 1.2vw;
}

.about-content p {
  padding: 10px 0;
}

.highlight {
  padding: 0 3px;
  position: relative;
  background-color: #3770ff;
}

.timer {
  width: 45vw;
  display: flex;
  justify-content: space-between;
}

#start {
  font-family: "Poppins", sans-serif;
  font-size: 2vh;
  color: #ffffff;
  margin: 5vh 0 0 0;
}

.timer span {
  font-size: 2vh;
  color: #ffffff;
  font-family: "Poppins", sans-serif;
}

.timer span span {
  font-family: Stargaze, sans-serif;
  color: #ffffff;
  font-size: 8vh;
}

.prize-section {
  width: 100vw;
  height: 100vh;
  background-color: #3770ff;
  display: flex;
  justify-content: center;
  align-items: center;
}

.prize {
  display: flex;
  flex-direction: column;
  height: 90vh;
  width: 80vw;
  justify-content: space-evenly;
}

.prize-heading {
  padding: 0;
  margin: 0;
  font-size: 5.6vw;
  letter-spacing: 2px;
  line-height: 7.36vw;
  font-family: Stargaze, sans-serif;
  color: #ffffff;
}

.list {
  width: 70%;
  margin: auto;
  text-align: left;
  color: #ffffff;
}

.list p {
  line-height: 2.6vw;
  font-size: 1.8vw;
  font-family: Poppins, sans-serif;
}

.bolder {
  font-family: Stargaze, sans-serif;
}

.faq {
  min-height: 100vh;
  width: 100%;
  background: #000000;
  padding-bottom: 10vh;
}

.faq_head {
  font-family: Stargaze, serif;
  font-size: 6vw;
  margin: 0;
  text-align: center;
  padding-top: 7vh;
  color: #ffffff;
}

.accordion {
  width: 55vw;
  margin: 12vh auto 0;
  color: #ffffff;
  font-family: 'Poppins', sans-serif;
}

.accordion-header {
  border-bottom: 0.3vh solid #ffffff;
}

.accordion-item {
  border: none;
}

.accordion-button {
  font-family: 'Poppins', sans-serif;
  color: #ffffff;
  font-size: 1.5vw;
}

.accordion-button:focus {
  box-shadow: none;
  border-color: rgba(0, 0, 0, .125);
}

.accordion-body {
  text-align: left;
}

@media (max-width: 900px) {

  .container {
    margin-left: 0;
    padding: 8rem 2rem 0 2rem;
    text-align: center;
  }

  .home {
    height: initial;
  }

  #heading {
    text-align: center;
    font-size: 4rem;
    line-height: initial;
  }

  #subH {
    text-align: center;
  }

  #text {
    text-align: center;
  }

  .buttonContainer {
    margin: auto;
  }

  .buttonContainer button {
    text-align: center;
  }

  .buttonContainer button p {
    margin: auto;
    font-size: 0.8rem;
  }

  .timer {
    width: initial;
  }

  .timer span span {
    font-size: 3rem;
  }

  .about {
    height: initial;
  }

  .about-heading {
    margin: initial;
    margin-top: 3rem;
    font-size: 3rem;

  }

  .about-content p {
    font-size: 1rem;
  }

  .prize-section {
    height: initial;
    padding: 4rem 1rem;
  }

  .prize-heading {
    margin: initial;
    font-size: 3rem;
    line-height: initial;
  }

  .prizes .list {
    width: initial;
    margin-top: 3rem;
    text-align: center;
  }

  .list p {
    font-size: 1rem;
    line-height: initial;
    margin-top: 30px;
  }

  .faq_head {
    font-size: 3rem;
  }

  .accordion {
    width: 80%;
    margin: 2rem auto;
  }

  .accordion button {
    font-size: 1rem;
  }
}

.accordion-button::after {
  background-image: url("../assets/arrow-204-32.png");
}

.accordion-button:not(.collapsed)::after {
  background-image: url("../assets/arrow-204-32.png");
}

#particles-js {
  position: absolute;
  width: 100vw;
  height: 100vh;
}
</style>
