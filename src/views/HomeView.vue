<template>
<div class="landing">
      <div class="container">
        <div class="text">
          <h3>Hi, my name is Ala Eddine Nour</h3>
          <p>
            I am a junior web developer with a Master's degree in computer science and a passion for building responsive, user-friendly websites.
            I am committed to improving my skills and staying up-to-date with the latest web development technologies.
          </p>
        </div>
        <div class="image">
          <img src="../assets/landing-image.png" alt="" />
        </div>
      </div>
    </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'HomeView',

}
</script>
<style scoped>
  .landing {
  position: relative;
}

.landing::after {
  content: "";
  position: absolute;
  left: 0;
  top: -40px;
  width: 100%;
  height: 100%;
  background-color: #ececec;
  z-index: -1;
  transform: skewY(-6deg);
  transform-origin: top left;
}

.landing a {
  color: var(--main-color);
  position: absolute;
  bottom: 30px;
  left: 50%;
  transform: translateX(-50%);
  transition: var(--main-transition);
}


.landing .container {
  min-height: calc(100vh - 72px);
  display: flex;
  align-items: center;
  padding-bottom: 120px;
}

.landing .text {
  flex: 1;
}

@media (max-width:991px) {
  .landing .text {
    text-align: center;
  }
}

.landing .text h3 {
  font-size: 40px;
  margin: 0;
  letter-spacing: -2px;
}

.landing .text p {
  font-size: 23px;
  line-height: 1.7;
  margin: 5px 0 0;
  color: #666;
  max-width: 500px;
}

@media (max-width:991px) {
  .landing .text p {
    margin: 20px auto;
  }
}

.landing .image img {
  position: relative;
  width: 600px;
  animation: up-down 8s linear infinite;
}

@media (max-width:991px) {
  .landing .image {
    display: none;
  }
}

/* start animation */

@keyframes up-down {

0%,
100% {
  top: 0;
}

50% {
  top: -50px;
}
}

/* end animation */
</style>
