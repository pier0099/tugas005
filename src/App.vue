<template>
  <div>
    <!-- Komponen Navbar -->
    <Navbar />

    <!-- Komponen Carousel -->
    <Carousel />

    

    <!-- Komponen Footer -->
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Carousel from './components/Carousel.vue';
import Card from './components/Card.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Navbar,
    Carousel,
    Card,
    Footer
  },
}
</script>

<style>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #4CAF50;
    color: white;
    text-align: center;
    padding: 1em 0;
}

.container {
    width: 80%;
    max-width: 100%;
    margin: 0 auto;
    padding: 1em;
    background-color: #f4f4f4;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.content {
    margin: 20px 0;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 1em 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

.carousel {
  margin: auto;
  margin-top: 20px;
  margin-bottom: 100px;
    position: relative;
    width: 600px;
    max-width: 1400px;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.carousel-inner {
    display: flex;
    transition: transform 0.5s ease-in-out;
}

.carousel-caption {
    padding: 1em;
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
    border-radius: 0 0 8px 8px;
    text-align: center;
    width: 100%;
    box-sizing: border-box;
}

.carousel-item {
    min-width: 100%;
    transition: transform 0.5s ease-in-out;
}

.carousel-item img {
    width: 100%;
    display: block;
    border-radius: 8px;
}

.carousel-control {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    border: none;
    color: white;
    font-size: 2rem;
    padding: 0.5em 1em;
    cursor: pointer;
    z-index: 10;
    border-radius: 50%;
}

.carousel-control.prev {
    left: 10px;
}

.carousel-control.next {
    right: 10px;
}

.carousel-control:hover {
    background-color: rgba(0, 0, 0, 0.8);
}

.title-carousel {
  font-size: 23px;
}

hr {
  width: 80%;
}

</style>
