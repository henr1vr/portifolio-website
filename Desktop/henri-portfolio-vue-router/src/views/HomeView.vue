<template>
  <div class="home">

    <!-- HERO SECTION -->
    <section class="hero">
      <h3 class="name">Henri van Rensburg</h3>
      <h1 class="heading">PORT<br class="mobile-break">FOLIO</h1>
      <h3 class="subtitle">I design digital experiences that balance usability, beauty, and storytelling.</h3>
      
      <div class="tags">
        <span class="tag red">Designer</span>
        <span class="tag purple">UI Designer</span>
        <span class="tag green">Graphic Designer</span>
        <span class="tag blue">Artist</span>
        <span class="tag yellow">Creative Thinker</span>
      </div>
    </section>

    <!-- MY WORK SECTION -->
    <section id="mywork" class="mywork">
      <h2>My Work</h2>
      <div class="Projects">
        <div class="Project" @mouseenter="showProject(0)">
          <span class="label yellow">WoodWorX</span>
          <img src="@/assets/images/Woodworx Preview image.png" alt="WoodWorX">
        </div>
        <div class="Project" @mouseenter="showProject(1)">
          <span class="label orange">HaptiNav</span>
          <img src="@/assets/images/Haptinav Preview image.png" alt="HaptiNav">
        </div>
        <div class="Project" @mouseenter="showProject(2)">
          <span class="label dark-orange">Ilitha</span>
          <img src="@/assets/images/Ilitha Preview image.png" alt="Ilitha">
        </div>
        <div class="Project" @mouseenter="showProject(3)">
          <span class="label purple">Fa Tanimals</span>
          <img src="@/assets/images/fa tanimals Preview image.png" alt="Fa Tanimals">
        </div>
        <div class="Project" @mouseenter="showProject(4)">
          <span class="label blue">Explorations</span>
          <img src="@/assets/images/Explorations Preview image.png" alt="Explorations">
        </div>
      </div>
    </section>

  </div>
</template>

<script>
export default {
  name: 'HomeView',
  methods: {
    showProject(index) {
      const projects = [
        { title: 'WoodWorX', desc: 'Gamified mobile app for woodworking projects' },
        { title: 'HaptiNav', desc: 'Haptic navigation interface for smart watches' },
        { title: 'Ilitha', desc: 'Design system and interface for Ilitha' },
        { title: 'Fa Tanimals', desc: 'Branding and product design for Fa Tanimals' },
        { title: 'Explorations', desc: 'Collection of creative experiments and sketches' }
      ]
      alert(projects[index].title + '\n\n' + projects[index].desc)
    }
  }
}
</script>

<style scoped>
/* You can paste parts of your existing CSS here later, or we'll import your full styles.css globally */
</style>