<script setup lang="ts">
import Instagram from '@/assets/icons/Instagram.svg'
import Discord from '@/assets/icons/Discord.svg'
import Twitter from '@/assets/icons/Twitter.svg'
</script>

<template>
  <div class="card">
    <div class="background"></div>
    <div class="logo">Socials</div>

    <a href="#">
      <div class="box box1">
        <span class="icon">
          <Instagram />
        </span>
      </div>
    </a>

    <a href="##">
      <div class="box box2">
        <span class="icon">
          <Discord />
        </span>
      </div>
    </a>

    <a href="###">
      <div class="box box3">
        <span class="icon">
          <Twitter />
        </span>
      </div>
    </a>

    <di class="box box4"></di>
  </div>
</template>

<style scoped>
.card {
  position: relative;
  width: 200px;
  height: 200px;
  background: lightgrey;
  border-radius: 30px;
  overflow: hidden;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
  transition: all 1s ease-in-out;
  border: 2px solid rgb(255, 255, 255);
}

.background {
  position: absolute;
  inset: 0;
  background-color: #4158d0;
  background-image: linear-gradient(43deg, #4158d0 0%, #c850c0 46%, #ffcc70 100%);
}

.logo {
  position: absolute;
  right: 50%;
  bottom: 50%;
  transform: translate(50%, 50%);
  transition: all 0.6s ease-in-out;
  font-size: 1.3em;
  font-weight: 600;
  color: #fff;
  letter-spacing: 3px;
}

.card:hover {
  transform: scale(1.1);
}

.card:hover .logo {
  transform: translate(70px, -52px);
  letter-spacing: 0px;
}

.box {
  position: absolute;
  padding: 10px;
  text-align: right;
  background: rgba(255, 255, 255, 0.389);
  border-top: 2px solid rgb(255, 255, 255);
  border-right: 1px solid white;
  border-radius: 10% 13% 42% 0%/10% 12% 75% 0%;
  box-shadow: rgba(100, 100, 111, 0.364) -7px 7px 29px 0px;
  transform-origin: bottom left;
  transition: all 1s ease-in-out;
}

.box::before {
  content: '';
  position: absolute;
  inset: 0;
  border-radius: inherit;
  opacity: 0;
  transition: all 0.5s ease-in-out;
}

.card:hover .box {
  bottom: -1px;
  left: -1px;
}

.box:hover .svg {
  fill: white;
}

.box1 {
  width: 70%;
  height: 70%;
  bottom: -70%;
  left: -70%;
}

.box1::before {
  background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #ff53d4 60%, #62c2fe 90%);
}

.box1:hover::before {
  opacity: 1;
}

.icon .svg {
  fill: rgba(255, 255, 255, 0.797);
  width: 100%;
  transition: all 0.5s ease-in-out;
}

.icon {
  display: inline-block;
  width: 20px;
  height: 20px;
}

.box1:hover .icon .svg {
  filter: drop-shadow(0 0 5px white);
}

.box2 {
  width: 50%;
  height: 50%;
  bottom: -50%;
  left: -50%;
  transition-delay: 0.2s;
}

.box2::before {
  background: radial-gradient(circle at 30% 107%, #91e9ff 0%, #00acee 90%);
}

.box2:hover::before {
  opacity: 1;
}

.box2:hover .icon .svg {
  filter: drop-shadow(0 0 5px white);
}

.box3 {
  width: 30%;
  height: 30%;
  bottom: -30%;
  left: -30%;
  transition-delay: 0.4s;
}

.box3::before {
  background: radial-gradient(circle at 30% 107%, #969fff 0%, #b349ff 90%);
}

.box3:hover::before {
  opacity: 1;
}

.box3:hover .icon .svg {
  filter: drop-shadow(0 0 5px white);
}

.box4 {
  width: 10%;
  height: 10%;
  bottom: -10%;
  left: -10%;
  transition-delay: 0.6s;
}
</style>
