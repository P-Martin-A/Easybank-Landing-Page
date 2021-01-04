<template>
  <nav class="navigation">
    <img @click="toggle" class="image menu active" src="@/assets/images/icon-hamburger.svg" alt="Menu">
    <img @click="toggle" class="image close inactive" src="@/assets/images/icon-close.svg" alt="Close">
    <ul class="list">
      <li class="item">
        <a class="link" href="#">Home</a>
        </li>
      <li class="item">
        <a class="link" href="#">About</a>
        </li>
      <li class="item">
        <a class="link" href="#">Contact</a>
        </li>
      <li class="item">
        <a class="link" href="#">Blog</a>
        </li>
      <li class="item">
        <a class="link" href="#">Careers</a>
        </li>
    </ul>
    <a class="btn" href="#">Request Invite</a>
  </nav>
</template>

<script>
  export default {
    name: 'Navigation',
    methods: {
      toggle() {
        const $IMAGE = document.querySelector('.image'),
              $MENU  = document.querySelector('.menu'),
              $CLOSE = document.querySelector('.close'),
              $LIST  = document.querySelector('.list'),
              $ALT   = $IMAGE.getAttribute('alt')

        if($IMAGE) {
          $MENU.classList.toggle('active')
          $MENU.classList.toggle('inactive')
          $CLOSE.classList.toggle('inactive')
          $CLOSE.classList.toggle('active')
          $LIST.classList.toggle('active')
        }
      }
    },
  }
</script>