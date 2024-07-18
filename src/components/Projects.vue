<template>
  <div class="projects">
    <h1>Mis proyectos</h1>
    <div class="project-list">
      <div class="project" v-for="project in projects" :key="project.id">
        <!-- <img :src="project.image" alt="Project Image" class="project-image"> -->
        <div class="project-content">
          <h2>{{ project.title }}</h2>
          <p>{{ project.description }}</p>
          <a :href="project.link" target="_blank" class="project-link">Ver proyecto</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data() {
    return {
      projects: [
        { id: 1, title: 'Velion', description: 'Solución ERP para la gestión de clínicas de salud, incluyendo pacientes, citas, facturas y una app móvil para una mejor experiencia de usuario.', link: 'https://github.com/sergiofrubio/velion-symfony' },
        // { id: 2, title: 'Project Two', description: 'Description for project two.' },
        // { id: 3, title: 'Project Three', description: 'Description for project three.' }
      ]
    };
  }
}
</script>

<style scoped>
.projects {
  text-align: center;
  padding: 50px;
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
  width: 300px;
  background: white;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s, box-shadow 0.2s;
}

.project:hover {
  transform: translateY(-10px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.project-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.project-content {
  padding: 20px;
  text-align: left;
}

.project h2 {
  margin: 0 0 10px;
  font-size: 1.5em;
  color: #333;
}

.project p {
  margin: 0 0 15px;
  color: #666;
}

.project-link {
  display: inline-block;
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
