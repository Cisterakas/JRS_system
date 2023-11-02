<!-- NavigationBar.vue -->
<template>
    <nav>
      <div class="div-2">
      <div class="div-3">
        <img
          loading="lazy"
          srcSet="https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&width=100 100w, https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&width=200 200w, https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&width=400 400w, https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&width=800 800w, https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&width=1200 1200w, https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&width=1600 1600w, https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&width=2000 2000w, https://cdn.builder.io/api/v1/image/assets/TEMP/3d2e8db6-3bc1-4ebe-bdb7-27f924fa0645?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&"
          class="img"
        />
        <button class="box" id="home">Home</button>
        <button class="box" id="shop">Shop</button>
          <button class="box" id="features">Features</button>
            <button class="box" id="contact">Contact</button>
            <button class="box" id="contact"> <img
          loading="lazy"
          src="https://cdn.builder.io/api/v1/image/assets/TEMP/89e840a4-5a8c-4a6d-adee-aa72786b3dd8?apiKey=3f6a7ddee9ae46558dc54af7e96aa0c9&"
          class="img-2"
        />
      </button>


      <button class="btnLogin">Login</button>
      </div>
    </div>
    </nav>
  </template>

  <script setup>

</script>

<style scoped>

.btnLogin {
  justify-content: center;
  align-items: center;
  border: 2px solid var(--color);
  border-radius: 6px;
  display: inline-block;

  margin: 20px;
  width: 6em;
  height: 2.6em;
  line-height: 2.5em;
  overflow: hidden;
  
  flex-direction: column;
  margin: auto 0;
  padding: 10px 27px;

  position: relative;
  --color: #224f34;

  z-index: 1;
  color: var(--color);

  text-transform: uppercase;
  align-self: center;
  white-space: nowrap;
  font: 500 20px Poppins, sans-serif;


}

.btnLogin::before {
  position: absolute;
  content: "";
  background: var(--color);
  width: 150px;
  height: 200px;
  z-index: -1;
  border-radius: 50%;
}

.btnLogin:hover {
  color: white;
}

.btnLogin:before {
  top: 100%;
  left: 100%;
  transition: .3s all;
}

.btnLogin:hover::before {
  top: -50px;
  left: -20px;
}









.box {
  width: auto;
  height: auto;
  float: left;
  transition: .5s linear;
  position: relative;
  display: block;
  overflow: hidden;
  padding: 15px;
  text-align: center;
 
  background: transparent;
  text-transform: uppercase;

  color: #224f34;
  text-transform: uppercase;
  align-self: center;
  margin: auto 0;
  font: 500 22px Poppins, sans-serif;
}

.box:before {
  position: absolute;
  content: '';
  left: 0;
  bottom: 0;
  height: 4px;
  width: 100%;
  border-bottom: 2px solid transparent;
  border-left: 2px solid transparent;
  box-sizing: border-box;
  transform: translateX(100%);
}

.box:after {
  position: absolute;
  content: '';
  top: 0;
  left: 0;
  width: 100%;
  height: 4px;
  border-top: 2px solid transparent;
  border-right: 2px solid transparent;
  box-sizing: border-box;
  transform: translateX(-100%);
}

.box:hover {
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
}

.box:hover:before {
  border-color: #224f34;
  height: 100%;
  transform: translateX(0);
  transition: .3s transform linear, .3s height linear .3s;
}

.box:hover:after {
  border-color: #224f34;
  height: 100%;
  transform: translateX(0);
  transition: .3s transform linear, .3s height linear .5s;
}

button {
  color: black;
  text-decoration: none;
  cursor: pointer;
  outline: none;
  border: none;
  background: transparent;
}
.div-2 {
  justify-content: center;
  align-items: center;
  background-color: var(--jrs, #c2efd4);
  align-self: stretch;
  display: flex;
  width: 100%;
  flex-direction: column;
  padding: 38px 20px;
}
@media (max-width: 991px) {
  .div-2 {
    max-width: 100%;
  }
}
.div-3 {
  align-self: center;
  display: flex;
  width: 100%;
  max-width: 1382px;
  align-items: flex-start;
  justify-content: space-between;
  gap: 20px;
}
@media (max-width: 991px) {
  .div-3 {
    max-width: 100%;
    flex-wrap: wrap;
    justify-content: center;
  }
}
.img {
  aspect-ratio: 1.31;
  object-fit: contain;
  object-position: center;
  width: 241px;
  overflow: hidden;
  align-self: stretch;
  max-width: 100%;
}


.img-2 {
  aspect-ratio: 1;
  object-fit: contain;
  object-position: center;
  width: 32px;
  filter: drop-shadow(1px 2px 9px rgba(0, 0, 0, 0.15));
  overflow: hidden;
  align-self: center;
  max-width: 100%;
  margin: auto 0;
}

</style>