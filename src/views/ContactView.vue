<template>
 <div class="contact" id="contact">
      <div class="container">
          <div class="speacial-heading-two">Contact</div>
          <p>We are born to create</p>
          <div class="contact-content">
              <a href="mailto:allaeddine.nour@gmail.com?subject=Contact">allaeddine.nour@gmail.com</a>
              <div class="social">
                  <p>Find Me On Social Networks</p>
                      <a href="https://github.com/aladine-lab" target="_blank" arial-label="Facebook"><i class="fab fa-github"></i></a>
                      <a href="https://www.linkedin.com/in/ala-eddine-nour-83690b21b/" target="_blank" arial-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
                  
              </div>
          </div>
      </div>
    </div>
  </template>
   <style scoped>
.contact {
  padding-top: var(--main-padding);
  padding-bottom: var(--main-padding);
  background-color: var(--background-section);
  min-height: 100vh;
}

.contact .contact-content {
  text-align: center;
}

.contact .contact-content a {
  color: var(--main-color);
  text-decoration: none;
  font-weight: 800;
  font-size: larger;
}
.contact .social {
  margin-top: 5px;
}

.contact .social p {
  margin-bottom: 10px;
}

.contact .social a {
  cursor: pointer;
  font-size: 30px;
  margin-right: 10px;
}

.speacial-heading-two {
  margin: 0;
  font-size: 100px;
  text-align: center;
  color: #ebeced;
  font-weight: 800;
  letter-spacing: -3px;
}

.speacial-heading-two+p {
  margin-top: -30px;
  margin-bottom: 60px;
  text-align: center;
  font-size: 20px;
  color: #797979;
}

@media (max-width:768px) {
  .speacial-heading-two {
      font-size: 90px;
  }

  .speacial-heading-two+p {
      margin-top: -40px;
      font-size: 28px;
      margin-bottom: 50px;
  }
}
</style>