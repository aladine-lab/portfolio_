<template>
    <div class="projects" id="Portfolio">
      <div class="container">
        <div class="speacial-heading">
          <h2>Portfolio</h2>
        </div>
        <div class="portfolio-content">
          <div class="project">
            <div class="image">
              <img src="../assets/1.png" alt="" />
            </div>
            <div class="text">
              <h3>Dashboard Design</h3>
              <p>
                Html & Css
               </p>
               <a href="https://github.com/aladine-lab/Template-four" target="_blank">
                 View github sources 
               </a>
            </div>
            <a class="info" href="https://aladine-lab.github.io/Template-four/index.html" target="_blank">
              <button>View Live Demo</button>
              <i class="fa-solid fa-right-long"></i>
            </a>
          </div>
          <div class="project">
            <div class="image">
              <img src="../assets/2.png" alt="" />
            </div>
            <div class="text">
              <h3>Portfolio</h3>
              <p>
                Html & Css
               </p>
               <a href="https://github.com/aladine-lab/Template-Three" target="_blank">
                 View github sources 
               </a>
            </div>
            <a class="info" href="https://aladine-lab.github.io/Template-Three/" target="_blank">
              <button>View Live Demo</button>
              <i class="fa-solid fa-right-long"></i>
            </a>
          </div>
          <div class="project">
            <div class="image">
              <img src="../assets/3.png" alt="" />
            </div>
            <div class="text">
              <h3>Kasper Portfolio</h3>
              <p>
                Html & Css
               </p>
               <a href="https://github.com/aladine-lab/Template-two" target="_blank">
                 View github sources 
               </a>
            </div>
            <a class="info" href="https://aladine-lab.github.io/Template-two/index.html" target="_blank">
              <button>View Live Demo</button>
              <i class="fa-solid fa-right-long"></i>
            </a>
          </div>
          <div class="project">
            <div class="image">
              <img src="../assets/4.png" alt="" />
            </div>
            <div class="text">
              <h3>Dashboard Design</h3>
              <p>
                Html & Css
               </p>
               <a href="https://github.com/aladine-lab/Template-one" target="_blank">
                 View github sources 
               </a>
            </div>
            <a class="info" href="https://aladine-lab.github.io/Template-One/index.html" target="_blank">
              <button>View Live Demo</button>
              <i class="fa-solid fa-right-long"></i>
            </a>
          </div>
          <div class="project">
            <div class="image">
              <img src="../assets/5.png" alt="" />
            </div>
            <div class="text">
              <h3>Doctor Appointment</h3>
              <p>
                Vue Js
               </p>
               <a href="https://github.com/aladine-lab/doctor-appointments" target="_blank">
                 View github sources 
               </a>
            </div>
            <a class="info" href="https://aladine-lab.github.io/doctor_appointments/" target="_blank">
              <button>View Live Demo</button>
              <i class="fa-solid fa-right-long"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
</template>

<style scoped>
/* start projects */
.projects {
  padding-top: var(--main-padding);
  padding-bottom: var(--main-padding);
}

.projects .container .portfolio-content {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  grid-gap: 40px;
}

.projects .container .portfolio-content .project {
  border-radius: 4px;
  box-shadow: 0 2px 15px rgb(0 0 0 / 10%);
  transition: transform var(--transition-dur), box-shadow var(--transition-dur);
}

.projects .container .portfolio-content .project:hover {
  transform: translateY(-10px);
  box-shadow: 0 2px 15px rgb(0 0 0 / 20%);
}

.projects .container .portfolio-content .project .image {
  max-height: 250px;
  overflow: hidden;
}

.projects .container .portfolio-content .project .image img {
  width: 100%;
  border-radius: 4px 4px 0 0;
}

.projects .container .portfolio-content .project .text {
  padding: 25px 15px;
  border-bottom: 1px solid #ddd;
}

.projects .container .portfolio-content .project .text h3 {
  text-transform: capitalize;
  margin-bottom: 15px;
}

.projects .container .portfolio-content .project .text p {
  line-height: 1.5;
  color: #777;
  margin-bottom: 15px;
}

.projects .container .portfolio-content .project .text a {
  border: 1px solid #ddd;
  padding: 0 10px;
  border-radius: 10px;
  background-color: #f6f6f6;
}

.projects .container .portfolio-content .project .info {
  padding: 20px 15px;
  color: var(--main-color);
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer;
}

.projects .container .portfolio-content .project .info button {
  border: none;
  background-color: white;
  color: var(--main-color);
  font-weight: bold;
  cursor: pointer;
}

.projects .container .portfolio-content .project:hover i {
  animation: move-rl 0.6s linear infinite;
}

@keyframes move-rl {
  100% {
    transform: translateX(7px);
  }
}

/* start title */
.speacial-heading {
  margin-bottom: 80px;
}

.speacial-heading h2 {
  position: relative;
  font-size: 30px;
  text-transform: uppercase;
  padding: 15px;
  border: 1px solid;
  width: fit-content;
  margin: auto;
  z-index: 5;
}

.speacial-heading h2:hover {
  animation: color-changing .3s linear forwards;
  animation-delay: 0.4s;
}

.speacial-heading h2::before {
  content: '';
  position: absolute;
  left: -30px;
  top: 50%;
  transform: translateY(-50%);
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background-color: var(--main-color);
  z-index: -1;
}

.speacial-heading h2::after {
  content: '';
  position: absolute;
  right: -30px;
  top: 50%;
  transform: translateY(-50%);
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background-color: var(--main-color);
  z-index: -1;
}

.speacial-heading h2:hover::before {
  animation: move-right .5s linear forwards;
}

.speacial-heading h2:hover::after {
  animation: move-left .5s linear forwards;

}

@keyframes move-left {
  50% {
    right: 0;
  }

  100% {
    right: 0;
    width: 60%;
    height: 100%;
    border-radius: 0;
  }
}

@keyframes move-right {
  50% {
    left: 0;
  }

  100% {
    left: 0;
    width: 50%;
    height: 100%;
    border-radius: 0;
  }
}

@keyframes color-changing {
  100% {
    color: white;
    border: 1px solid white;
  }
}

/* end title */
</style>
