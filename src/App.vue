<script setup>
</script>

<template>
  <!-- header-->
  <div class="main">
    <div class="nav-container">
      <nav class="nav">
        <a href="#header">Home</a>
        <a href="#about">About</a>
        <a href="#porjects">Projects</a>
        <a>Contact</a>
      </nav>
    </div>
    <div id="header" class="main-container">
      <div class="header-container">
        <h1
        v-motion
        :initial="{ opacity: 0, y: -100 }"
        :visible="{ opacity: 1, y: 0 }"
        :duration="1000" 
        class="greetings">
          <pre>Welcome To
My Portofolio
          </pre>
          <div
          v-motion
          :initial="{ opacity: 0, y: -100 }"
          :visible="{ opacity: 1, y: 0 }"
          :duration="2000" 
          class="name">
            <p 
              v-motion
            :initial="{ opacity: 0, y: -100 }"
            :visible="{ opacity: 1, y: 0 }"
            :duration="3000" 
            >
              Hari Cahyono/Web Developer
            </p>
          </div>
        </h1>
      <div
      v-motion
      :initial="{ opacity: 0, x: -100 }"
      :visible="{ opacity: 1, x: 0 }"
      :duration="1000"
      class="profile">
        <img src="./assets/medium.webp" alt="">
      </div>
    </div>
  </div>
  <!-- end of header -->

  <!-- about-->
  <div id="about" class="about-container">
    <div class="about-me">
      <Motion 
          :initial="{ opacity: 0, y: -100 }"
          :visible="{ opacity: 1, y: 0 }"
          :duration="1000"
      >
        <h1>
          <pre>Who Am I?</pre>
        </h1>
      </Motion>
      <div
        v-motion
        :initial="{ opacity: 0, y: 100 }"
        :visible="{ opacity: 1, y: 0 }"
        :duration="1000"
        class="my-desc"
      >
        <p 
        v-motion
        :initial="{ opacity: 0, y: 100 }"
        :visible="{ opacity: 1, y: 0 }"
        :duration="2000"
        >
          A web developer with expertise in building full-stack web applications. Experienced in API integration, database management, and creating responsive, interactive user interfaces. Passionate about developing efficient systems and committed to continuously learning and enhancing skills with the latest technologies in web development.</p>
      </div>
    </div>
    <div 
      class="image"
      v-motion
      :initial="{ opacity: 0, x: -100 }"
      :visible="{ opacity: 1, x: 0 }"
      :duration="1000"
    >
      <img src="https://images.unsplash.com/photo-1510751007277-36932aac9ebd?q=80&w=1474&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="">
    </div>
  </div>
  <!-- end of about-->

  <!-- projects -->
  <div id="porjects" class="my-projects">
    <h1
      v-motion
      :initial="{ opacity: 0, y: -100 }"
      :visible="{ opacity: 1, y: 0 }"
      :duration="1000"
    >
      <pre>My Projects</pre>
    </h1>
    <div class="projects-container">
      <div 
      v-motion
      :initial="{ opacity: 0, x: -100 }"
      :visible="{ opacity: 1, x: 0 }"
      :duration="2000"
      class="project">
        <img src="https://img.freepik.com/free-vector/coming-soon-banner-with-focus-lights_1017-33739.jpg" alt="project-image">
        <a href="">coming soon</a>
      </div>
      <div 
      v-motion
      :initial="{ opacity: 0, x: -300 }"
      :visible="{ opacity: 1, x: 0 }"
      :duration="2000"
      class="project">
        <img src="https://img.freepik.com/free-vector/coming-soon-banner-with-focus-lights_1017-33739.jpg" alt="project-image">
        <a href="">coming soon</a>
      </div>
      <div 
      v-motion
      :initial="{ opacity: 0, x: -500 }"
      :visible="{ opacity: 1, x: 0 }"
      :duration="2000"
      class="project">
        <img src="https://img.freepik.com/free-vector/coming-soon-banner-with-focus-lights_1017-33739.jpg" alt="project-image">
        <a href="">coming soon</a>
      </div>
    </div>
  </div>
  <!-- end of projects -->

  <!-- beautiful word-->
  <div id="header" class="main-container">
      <div class="word-container">
        <h1
        v-motion
        :initial="{ opacity: 0, x: -100 }"
        :visible="{ opacity: 1, x: 0 }"
        :duration="1000" 
        class="word">
          <pre>Behind every line of code,
there is a story 
that cannot be explained.
          </pre>
        </h1>
      <div
      v-motion
      :initial="{ opacity: 0, x: 100 }"
      :visible="{ opacity: 1, x: 0 }"
      :duration="1000"
      class="profile">
        <img src="https://img.freepik.com/free-photo/close-up-image-programer-working-his-desk-office_1098-18707.jpg?t=st=1735579842~exp=1735583442~hmac=1f2c39244b156c8611512f315687f27e801668910c1b1ba98c4102b2dc4daced&w=826" alt="">
      </div>
    </div>
  </div>
<!-- end of beautiful word-->
  </div>

<div class="soon">
  <h1>This is not done yet. The others will be coming soon. 😊</h1>
</div>

<div class="responsive-warning">
  <h1>the responsive version is not made yet. ^_^</h1>
</div>

</template>

<style>
*, body {
  scroll-behavior: smooth; 
  margin: 0;
  color: white;
  background-color: black;
}

a {
  text-decoration: none;
}

/* header styling */
.nav-container {
  background-color: rgb(0, 0, 0);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 9999;
}

.nav {
  padding: 15px;
  float: right;
  background-color: transparent;
}


.nav a {
  background-color: transparent;
  margin-right: 15px;
  font-family: "Days One", serif;
  font-weight: 400;
  font-style: normal;
  cursor: pointer;
}

.nav a:hover {
  color: darkgrey;
}

.main-container {
  margin-top: 100px;
}

.header-container {
  display: flex;
  justify-content: space-between;
  width: 90%;
  margin: auto;
}

/* .greetings {
  display: flex;
  flex-direction: row;
} */

.greetings pre {
  font-family: "EB Garamond", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
  font-size: 2.5em;
  line-height: 66px;
}

.name {
  margin-top: 50px;
  border: 1px solid white;
  width: fit-content;
  padding: 20px 40px;
  border-radius: 37px;
}

.name p {
  font-family: "Montserrat", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
}

.profile {
    width: 450px;
    height: 550px;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 90px;
}

.profile img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-top-left-radius: 80%;
    border-top-right-radius: 30%;
    border-bottom-left-radius: 30%;
    border-bottom-right-radius: 80%;
}
/* end of header styling */

/* about styling */
.about-container {
  display: flex;
  width: 90%;
  margin: 200px auto 200px auto;
}

.about-container .image {
  width: 400px;
  height: fit-content;
  margin-left: 50px;
}

.about-container img {
  width: 100%;
  object-fit: cover;
  border-radius: 50%;
}

.about-container .about-me {
  width: 600px;
  height: 400px;
}

.about-container .about-me pre {
  font-family: "EB Garamond", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
  font-size: 2.5em;
  line-height: 66px;
  width: fit-content;
}

.about-container .my-desc {
  width: 55%;
  height: fit-content;
  border-bottom: 1px solid white;
  padding-bottom: 20px;
  margin-top: 140px;
}

.about-container .my-desc p {
  font-family: "Montserrat", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
}
/* end of about styling */

/* word container */
.word-container {
  display: flex;
  justify-content: space-between;
  width: 90%;
  margin: auto;
}

.word {
  align-content: center;
}

.word pre {
  font-family: "EB Garamond", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
  font-size: 2em;
  line-height: 56px;
}
/* end of word container */

/* projects styling */
.my-projects {
  width: 90%;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 200px;
}

.my-projects h1 {
  margin-bottom: 100px;
}

.my-projects h1 pre {
  font-family: "EB Garamond", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
  font-size: 2.5em;
}

.my-projects .projects-container {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
}

.my-projects .projects-container .project {
  width: 300px;
  height: 300px;
  text-align: center;
}

.project img {
  width: 100%;
  object-fit: cover;
  border-radius: 65%;
}

.project a {
  font-family: "Montserrat", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
}
/* end of projects styling */


.soon {
  width: 100%;
  text-align: center;
  padding: 100px 0;
}

.soon h1 {
  font-family: "Montserrat", serif;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;
}

.responsive-warning {
  display: none;
}

@media only screen and (min-width: 600px) and (max-width: 1024px) {
  *, body {
    background-color: white;
    color: black;
  }
  
  .responsive-warning {
    display: block;
  }

  .main {
    display: none;
  }

  .soon {
    display: none;
  }
}

@media only screen and (min-width: 320px) and (max-width: 599px) {
  *, body {
    background-color: white;
    color: black;
  }
  
  .responsive-warning {
    display: block;
  }

  .main {
    display: none;
  }

  .soon {
    display: none;
  }
}

@media only screen and (max-width: 319px) {
  *, body {
    background-color: white;
    color: black;
  }
  
  .responsive-warning {
    display: block;
  }

  .main {
    display: none;
  }

  .soon {
    display: none;
  }
}
</style>
