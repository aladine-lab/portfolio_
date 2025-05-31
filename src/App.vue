<template>
  <header>
      <div class="container">
        <a href="#" class="logo">AlaDine</a>
        <ul class="nav">
          <li><router-link to="/">About Me</router-link></li>
          <li><router-link to="/portfolio">Portfolio</router-link></li>
          <li><router-link to="/contact">Contact</router-link></li>
        </ul>
      </div>
    </header>
    <a href="assets/my-cv.pdf" class="btn-download" download="AlaEddine-Nour-cv.pdf"> Download CV</a>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

:root {
  --main-color: #2196f3;
  --main-color-alt: #1787e0;
  --transition-dur: .3s;
  --main-padding: 60px;
  --section-color: #ececec;
  --background-section: #f6f6f6;
}

* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

.container {
  padding-left: 15px;
  padding-right: 15px;
  margin-left: auto;
  margin-right: auto;
}

html {
  scroll-behavior: smooth;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

a {
  text-decoration: none;
  color: black;
}

/* small */

@media (min-width: 768px) {
  .container {
    width: 750px;
  }
}

/* meduim */
@media (min-width: 992px) {
  .container {
    width: 970px;
  }
}

/* large */
@media (min-width: 1200px) {
  .container {
    width: 1170px;
  }
}

/* start header */
header {
  box-shadow: 0 0 10px #ddd;
  background-color: white;
  position: relative;
}

header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  position: relative;
}

header .logo {
  color: var(--main-color);
  font-size: 26px;
  height: 72px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: 800;
}

header .nav {
  display: flex;
}

@media (max-width:767px) {
  header .logo {
    width: 100%;
  }

  header .nav {
    margin: auto;
  }
}

header .nav>li>a {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 15px;
  height: 72px;
  font-size: 18px;
  position: relative;
  overflow: hidden;
  transition: var(--transition-dur);
}

@media (max-width:767px) {
  header .nav>li>a {
    padding: 0 10px;
  }
}

header .nav>li>a::before {
  content: "";
  position: absolute;
  left: -100%;
  top: 0;
  width: 100%;
  height: 4px;
  background-color: var(--main-color);
  transition: var(--transition-dur);
}

header .nav>li>a:hover {
  color: var(--main-color);
  background-color: #fafafa;
}

header .nav>li>a:hover::before {
  left: 0;
}

/* download button */
.btn-download {
  padding: 16px 32px;
  font-size: 16px;
  position: fixed;
  right: 10px;
  bottom: 30px;
  background-color: white;
  border-radius: 15px;
  font-weight: bold;
  border: 1px solid black;
  cursor: pointer;
  z-index: 1000;
}

.btn-download:hover {
  scale: 1.1;
  transition: var(--transition-dur);
}

/* download button */
/* end header */

</style>
