<template>
  <div class="projects">
    <h1>My Projects</h1>
    <div class="row">
      <div class="col-md-4" v-for="project in projects" :key="project.id">
        <div class="card mb-4">
          <img :src="project.image" class="card-img-top" :alt="project.title" />
          <div class="card-body">
            <h5 class="card-title">{{ project.title }}</h5>
            <p class="card-text">{{ project.description }}</p>
            <a :href="project.link" class="btn btn-primary">View Project</a>
          </div>
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
        {
          id: 1,
          title: 'Project 1',
          description: 'Description of project 1.',
          image: 'path/to/image1.jpg',
          link: '#',
        },
        {
          id: 2,
          title: 'Project 2',
          description: 'Description of project 2.',
          image: 'path/to/image2.jpg',
          link: '#',
        },
        {
          id: 3,
          title: 'Project 3',
          description: 'Description of project 3.',
          image: 'path/to/image3.jpg',
          link: '#',
        },
      ],
    }
  },
}
</script>

<style scoped>
.projects {
  text-align: center;
  padding: 50px;
}
.card-img-top {
  height: 200px;
  object-fit: cover;
}
</style>
