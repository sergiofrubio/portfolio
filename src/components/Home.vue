<template>
  <div class="home">
    <img src="@/assets/mi-foto.jpg" alt="Foto Personal" class="profile-pic">
    <h1>¡Bienvenido!</h1>
    <p>Explora mis proyectos y conóceme.</p>
    <a href="https://www.linkedin.com/in/fisicarubio">
      <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
    </a>
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped>
.home {
  text-align: center;
  padding: 50px;
}

.profile-pic {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  margin-bottom: 20px;
}

.linkedin-link {
  display: inline-block;
  margin-top: 10px;
  font-size: 1.2em;
  text-decoration: none;
  color: #0077b5;
  align-items: center;
}

.linkedin-logo {
  width: 20px;
  height: 20px;
  margin-right: 5px;
  vertical-align: middle;
}
</style>
