<template>
  <footer>
    <p><a href="mailto:mauriciolfsilva@gmail.com" class="contact-link">mauriciolfsilva@gmail.com</a> | 
       <a href="https://www.linkedin.com/in/mauricio-leonardo/" class="contact-link">Linkedin</a> |
       <a href="https://github.com/mauriciolfsilva" class="contact-link">Github</a>
    </p>
  </footer>
</template>

<script>
export default {
}
</script>
<style scoped>
footer {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background: linear-gradient(45deg, #333333, #222222);
  color: white;
  padding: 20px 0;
  text-align: center;
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.3);
}
.contact-link {
  color: #fff;
  text-decoration: none;
  border-bottom: 1px dotted #fff;
  transition: border-color 0.3s ease;
}
.contact-link:hover {
  border-bottom-color: transparent;
}
</style>
