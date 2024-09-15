<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap");

/* Styling */
html,
body {
  height: 100%;
  margin: 0;
  padding: 0;
}

/* Style untuk navbar */
#navbar {
  display: flex;
  margin-top: 70px;
  width: 100%;
  border-radius: 20px;
  justify-content: space-between;
  align-items: center;
  background-color: rgb(28, 28, 28); /* Warna background */
  padding: 0 20px;
  height: 80px;
}

.logo {
  color: white;
  font-size: 24px;
  font-weight: bold;
}

.nav-links {
  display: flex;
  list-style: none;
}

.nav-links li {
  margin: 0 15px;
}

.nav-links a {
  color: white;
  text-decoration: none;
  font-size: 18px;
  padding: 8px 12px;
  transition: background-color 0.3s ease-in-out, color 0.3s ease-in-out;
}

/* Hover effect untuk link */
.nav-links a:hover {
  background-color: #00d4ff;
  border-radius: 20px;
  color: black;
  font-weight: bold;
}

/* Menu burger (untuk tampilan mobile) */
.burger {
  display: none;
  cursor: pointer;
}

.burger div {
  width: 25px;
  height: 3px;
  background-color: white;
  margin: 5px;
  transition: all 0.3s ease;
}

#app {
  font-family: sans-serif;
  text-align: center;
  color: #e0e0e0;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 20px;
  transition: background-color 0.5s ease;
  background: linear-gradient(150deg, #0014ef, #5361ff, #9aa2ff);
}

header {
  margin-bottom: 30px;
}

h1 {
  color: #00d4ff;
  margin: 0;
  font-size: 3em;
  text-shadow: 0 1px 2px rgba(0, 212, 255, 0.3),
    0 2px 4px rgba(0, 212, 255, 0.2);
  border: 1px solid rgb(0, 0, 232);
  background-color: rgb(28, 28, 28);
  height: 80px;
  width: 500px;
  border-radius: 25px;
  cursor: pointer;
}

h1:hover {
  border-radius: 25px;
  transform: translateY(-2px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2), 0 4px 8px rgba(0, 0, 0, 0.3);
}

/* Layout and Grid */
.content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  max-width: 1200px;
  width: 100%;
}

/* Card Styling */
.card {
  background: rgba(255, 255, 255, 0.1);
  padding: 20px;
  border-radius: 15px;
  backdrop-filter: blur(10px);
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
  color: #fff;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  background: linear-gradient(50deg, #0010bc, #191919, #0010bc);
  border: 2px solid black;
}

.card:hover {
  transform: translateY(-8px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2), 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 50px;
}

/* Counter Section */
.counter {
  font-size: 2em;
  margin: 10px 0;
}

.counter-buttons {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
}

/* Buttons Styling */
.btn {
  background-color: #00d4ff;
  color: #fff;
  border: none;
  padding: 14px 28px;
  border-radius: 30px;
  cursor: pointer;
  transition: background-color 0.4s ease-in-out, transform 0.3s ease;
  box-shadow: 0 2px 4px rgba(0, 212, 255, 0.2), 0 1px 3px rgba(0, 0, 0, 0.1);
}

.btn1 {
  background-color: #00b200;
  color: #fff;
  border: none;
  padding: 14px 28px;
  border-radius: 30px;
  cursor: pointer;
  transition: background-color 0.4s ease-in-out, transform 0.3s ease;
  box-shadow: 0 2px 4px rgba(0, 212, 255, 0.2), 0 1px 3px rgba(0, 0, 0, 0.1);
  margin-left: 5px;
}

.btn2 {
  background-color: #00b200;
  color: #fff;
  border: none;
  padding: 14px 28px;
  border-radius: 30px;
  cursor: pointer;
  transition: background-color 0.4s ease-in-out, transform 0.3s ease;
  box-shadow: 0 2px 4px rgba(0, 212, 255, 0.2), 0 1px 3px rgba(0, 0, 0, 0.1);
}

.btn:hover {
  transform: scale(1.05);
  border: 2px solid white;
}

.btn1:hover {
  transform: scale(1.05);
  border: 2px solid white;
}

.btn2:hover {
  transform: scale(1.05);
  border: 2px solid white;
}

/* Increment and Decrement Buttons */
.increment-btn {
  background-color: #00b200;
}

.decrement-btn {
  background-color: #a40e00;
}

/* Carousel Styling */
.carousel-section {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.carousel {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.carousel-image {
  width: 100%;
  max-width: 350px;
  height: auto;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
  margin-bottom: 10px;
  transition: transform 0.3s ease;
  margin-top: 20px;
  margin-bottom: 20px;
}

.carousel-image:hover {
  transform: scale(1);
}

/* Color Picker Styling */
.color-picker {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.current-color-box {
  width: 100px;
  height: 100px;
  margin: 10px auto 20px;
  border-radius: 50px;
  border: 2px solid #fff;
  transition: background-color 0.3s ease;
  border: 2px solid white;
}

.color-btn {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin: 5px;
  border: none;
  cursor: pointer;
  transition: transform 0.3s, box-shadow 0.3s;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  border: 2px solid black;
}

.color-btn:hover {
  transform: scale(1.2);
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
}
</style>

<!-- Kerangka kodingan -->
<template>
  <nav id="navbar">
    <div class="logo">Tugas Vue 1</div>
    <ul class="nav-links">
      <li><a href="#">Home</a></li>
      <li><a href="#">Click counter</a></li>
      <li><a href="#">box change color</a></li>
      <li><a href="#">Image carousel</a></li>
    </ul>
    <div class="burger">
      <div class="line1"></div>
      <div class="line2"></div>
      <div class="line3"></div>
    </div>
  </nav>
  <div id="app">
    <header>
      <h1>Hallo, Selamat Datang!</h1>
    </header>

    <main>
      <div class="content">
        <section class="card">
          <h2>Click Counter</h2>
          <div class="counter">
            <p>Count: {{ count }}</p>
            <div class="counter-buttons">
              <button @click="decrementCount" class="btn decrement-btn">
                -
              </button>
              <button @click="incrementCount" class="btn increment-btn">
                +
              </button>
            </div>
          </div>
        </section>

        <section class="card carousel-section">
          <h2>Image Carousel</h2>
          <div class="carousel">
            <img
              :src="currentImage"
              alt="Carousel Image"
              class="carousel-image"
            />
            <div class="carousel-controls">
              <button @click="prevImage" class="btn">Previous</button>
              <button @click="nextImage" class="btn1">Next</button>
            </div>
          </div>
        </section>

        <section class="card">
          <h2>Ganti Warna Background</h2>
          <div
            class="current-color-box"
            :style="{ backgroundColor: backgroundColor }"
          ></div>
          <div class="color-changer">
            <button @click="changeBackgroundColor" class="btn2">
              Ubah Warna
            </button>
          </div>
          <div class="color-options">
            <h3>Select a Color:</h3>
            <div class="color-picker">
              <button
                v-for="(color, index) in colors"
                :key="index"
                :style="{ backgroundColor: color }"
                @click="setColor(color)"
                class="color-btn"
              ></button>
            </div>
          </div>
        </section>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
      backgroundColor: "#2F4F4F",
      images: [
        "https://1.bp.blogspot.com/-uCadQ9loQ4s/V5evshgs7WI/AAAAAAAACY4/_RnyaMZqZLw9dHpxQTEtdrQ9m_EgvoIFwCLcB/s1600/Gambar-kucing-1.JPG",
        "https://th.bing.com/th/id/OIP.EEOKUkTukt_-G1eQphGK7wHaD-?rs=1&pid=ImgDetMain",
        "https://i1.wp.com/www.nesabamedia.com/wp-content/uploads/2019/05/featured-images-2.jpg?fit=1200%2C675&ssl=1",
        "https://o-cdn-cas.sirclocdn.com/parenting/images/kucing-domestik.width-800.format-webp.webp",
      ],
      currentImageIndex: 0,
      colors: [
        "#989861",
        "#647381",
        "#009958",
        "#777190",
        "#487496",
        "#FFEB3B",
        "#000000",
        "#111132",
        "#213347",
        "#001355",
      ],
    };
  },
  computed: {
    currentImage() {
      return this.images[this.currentImageIndex];
    },
  },
  methods: {
    incrementCount() {
      this.count++;
    },
    decrementCount() {
      if (this.count > 0) {
        this.count--;
      }
    },
    changeBackgroundColor() {
      const randomIndex = Math.floor(Math.random() * this.colors.length);
      this.backgroundColor = this.colors[randomIndex];
    },
    setColor(color) {
      this.backgroundColor = color;
    },
    nextImage() {
      this.currentImageIndex =
        (this.currentImageIndex + 1) % this.images.length;
    },
    prevImage() {
      this.currentImageIndex =
        (this.currentImageIndex - 1 + this.images.length) % this.images.length;
    },
  },
};
</script>
