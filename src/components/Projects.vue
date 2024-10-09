<template>
  <div class="projects">
    <h1>Mis proyectos</h1>
    <div class="project-list">
      <div class="project" v-for="project in projects" :key="project.id">
        <img :src="project.image" :alt="project.title + ' Image'" class="project-image" />
        <div class="project-content">
          <h2>{{ project.title }}</h2>
          <p>{{ project.description }}</p>
          <div class="project-footer">
            <div class="tech-icons">
              <img
                v-for="(icon, index) in project.tech"
                :key="index"
                :src="icon.url"
                :alt="icon.name"
                class="tech-icon"
              />
            </div>
            <a :href="project.link" target="_blank" class="project-link">Ver proyecto</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "SIGEFI",
          description: "Solución ERP para la gestión integral de clínicas de salud, mejorando la atención sanitaria",
          image: "https://placehold.it/300x200",
          link: "https://github.com/sergiofrubio/velion-symfony",
          tech: [
            { name: "Symfony", url: "https://cdn.worldvectorlogo.com/logos/symfony.svg" },
            { name: "Vue.js", url: "https://cdn.worldvectorlogo.com/logos/vue-9.svg" },
            { name: "AndroidStudio", url: "https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Android_Studio_icon_%282023%29.svg/2048px-Android_Studio_icon_%282023%29.svg.png" },
            // Agrega más iconos según sea necesario
          ]
        },
        {
          id: 2,
          title: "EduNote",
          description: "Sistema de Gestión Escolar para instituciones educativas de Colombia.",
          image: "https://placehold.it/300x200",
          link: "https://github.com/sergiofrubio/velion-symfony",
          tech: [
            { name: "Spring", url: "https://cdn.worldvectorlogo.com/logos/spring-3.svg" },
            { name: "React", url: "https://www.svgrepo.com/show/303500/react-1-logo.svg" },
            // Agrega más iconos según sea necesario
          ]
        },
        // Agrega más proyectos según sea necesario
      ],
    };
  },
};
</script>

<style scoped>
.projects {
  text-align: center;
  padding: 50px;
  /* Puedes descomentar la siguiente línea si deseas un fondo */
  /* background-color: #f5f5f5; */
}

.project-list {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 1cm;
}

.project {
  width: 300px; /* Ancho fijo para todas las tarjetas */
  background: white;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s, box-shadow 0.2s;
  
  /* Convertimos cada tarjeta en un contenedor flex con dirección columna */
  display: flex;
  flex-direction: column;
  
  /* Aseguramos que todas las tarjetas tengan la misma altura */
  height: 100%;
}

.project:hover {
  transform: translateY(-10px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.project-image {
  width: 100%;
  height: 200px; /* Altura fija para la imagen */
  object-fit: cover;
}

.project-content {
  padding: 20px;
  text-align: left;
  
  /* Convertimos el contenido en un contenedor flex con dirección columna */
  display: flex;
  flex-direction: column;
  
  /* Permitimos que el contenido crezca para llenar el espacio disponible */
  flex-grow: 1;
}

.project h2 {
  margin: 0 0 10px;
  font-size: 1.5em;
  color: #333;
}

.project p {
  margin: 0 0 15px;
  color: #666;
  /* Permitimos que el párrafo ocupe el espacio disponible */
  flex-grow: 1;
}

.project-footer {
  /* Empujamos este contenedor hacia el fondo de .project-content */
  margin-top: auto;
  
  /* Alineamos los elementos horizontalmente con espacio entre ellos */
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.tech-icons {
  display: flex;
  flex-wrap: wrap;
  margin: 0;
}

.tech-icon {
  width: 30px;
  height: 30px;
  margin-right: 5px;
  margin-bottom: 5px;
}

.project-link {
  padding: 10px 15px;
  color: white;
  background-color: #007bff;
  border-radius: 4px;
  text-decoration: none;
  transition: background-color 0.2s;
}

.project-link:hover {
  background-color: #0056b3;
}
</style>
