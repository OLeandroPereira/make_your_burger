<template>
  <div id="main-banner">
    <h1>Make Your Burger</h1>
  </div>
</template>

<script>
export default {
  name: "Banner"
}
</script>

<style scoped>

#main-banner {
  background-image: url('/public/img/burger_1.jpg');
  background-position: 0 -360px;
  background-size: cover;
  height: 600px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  position: relative;
}

#main-banner::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: 1;
}

#main-banner h1 {
  color: #FFFFFF; 
  text-align: center;
  font-size: 60px;
  background-color: #8B0000;
  padding: 20px 40px;
  box-shadow: 3px 3px 3px #555;
  position: relative;
  transform: translate(-50%, -50%);
  z-index: 2;
  transform: translateY(0px);
  animation: float 5s ease-in-out infinite;
  margin: auto;
}

@keyframes float {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-30px);
  }
  100% {
    transform: translateY(0px);
  }
}

</style>