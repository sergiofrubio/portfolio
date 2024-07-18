<template>
  <div class="about">
    <h1>Sobre mí</h1>
    <p>Soy un estudiante de Matemáticas y desarrollador apasionado por la tecnología y la programación. Me encanta aprender nuevas habilidades y aplicar mis conocimientos en proyectos interesantes. Estoy comprometido con la mejora continua y siempre busco desafíos que me permitan crecer profesional y personalmente.</p>
    
    <div class="tech-logos">
      <img src="https://cdn-icons-png.flaticon.com/256/732/732212.png" alt="HTML5" width="50" height="50"/>
      <img src="https://cdn-icons-png.flaticon.com/256/732/732190.png" alt="CSS3" width="50" height="50"/>
      <img src="https://cdn-icons-png.flaticon.com/256/5968/5968292.png" alt="JavaScript" width="50" height="50"/>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1200px-Vue.js_Logo_2.svg.png" alt="Vue" width="50" height="50"/>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Bootstrap_logo.svg/2560px-Bootstrap_logo.svg.png" alt="BootStrap" width="50" height="50"/>
      <img src="https://cdn-icons-png.flaticon.com/256/5968/5968332.png" alt="PHP" width="50" height="50"/>
      <img src="https://cdn.worldvectorlogo.com/logos/symfony.svg" alt="Symfony" width="50" height="50"/>
      <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.vhv.rs%2Fdpng%2Fd%2F543-5438423_mysql-logo-hd-png-download.png&f=1&nofb=1&ipt=33151a5129ff80d6aa6cb22c4dc399125935436c4009eaa4ce728acbfc43d377&ipo=images" alt="MySQL" width="50" height="50"/>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Git_icon.svg/2048px-Git_icon.svg.png" alt="Git" width="50" height="50"/>
    </div>

    <div class="education">
      <h2>Formación</h2>
      <ul>
        <li>
          <h3>Grado en Matemáticas</h3>
          <p>Universidad Nacional de Educación a Distantia (España) - 2024 - Presente</p>
        </li>
        <li>
          <h3>Técnico Superior en Desarrollo de Aplicaciones Multiplataforma</h3>
          <p>CES Lope de Vega - 2022 - 2024</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.about {
  padding: 50px;
  /* background-color: #f5f5f5; */
  text-align: center;
}

.about h1 {
  font-size: 2.5em;
  margin-bottom: 20px;
}

.about p {
  margin: 20px auto;
  max-width: 800px;
  line-height: 1.6;
  font-size: 1.2em;
}

.tech-logos {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
  margin: 40px 0;
}

.education {
  margin-top: 40px;
}

.education h2 {
  font-size: 2em;
  margin-bottom: 20px;
}

.education ul {
  list-style-type: none;
  padding: 0;
}

.education li {
  background: white;
  padding: 20px;
  margin-bottom: 10px;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.education h3 {
  margin: 0 0 10px;
  font-size: 1.5em;
}

.education p {
  /* margin: 0 0 10px; */
  font-size: 1.1em;
  color: #666;
}
</style>
