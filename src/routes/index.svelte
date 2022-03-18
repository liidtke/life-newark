<script lang="ts">
  import "../app.css";
  import Courses from "$lib/Courses.svelte";
</script>

<div class="content">
    <img class="img" src="image.png" alt="">
</div>

  <!-- <img class="image" src="image.png" alt="" /> -->
  <!-- <h1 class="header">Placeholder</h1> -->

  <div class="contact">
    <a href="tel:+1732 209 0105">Contato: (732) 209 0105</a>
  </div>

<Courses></Courses>

<footer>
  <svg viewBox="0 -20 700 110" width="100%" height="110" preserveAspectRatio="none">
    <path transform="translate(0, -20)" d="M0,10 c80,-22 240,0 350,18 c90,17 260,7.5 350,-20 v50 h-700" fill="#CEB964" />
    <path d="M0,10 c80,-18 230,-12 350,7 c80,13 260,17 350,-5 v100 h-700z" fill="#1f3d24" />
  </svg>
</footer>

<style>
  .contact {
    text-align: center;
    width: 180px;
    width: 100%;
    border: 1px solid;
    padding: 8px;
    background: var(--green);
    border-radius: 2px;
    opacity: 0;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    -webkit-animation-name: fadeIn;
    animation-name: fadeIn;
    animation-duration: 2s;
    animation-delay: 1s;
    animation-fill-mode: both;
    border: none;
    -webkit-animation-fill-mode: both;
    cursor: pointer;
  }

  .contact:hover{
    filter: brightness(1.3);
  }

  @-webkit-keyframes fadeIn {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }

  @keyframes fadeIn {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }

  .contact > a {
    color: #fff;
    text-decoration: none;
    font-weight: 500;
    font-size:16px
  }

  .header {
    color: var(--green);
  }

  .content {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .img {
    display: block;
    height: 100%;
  }


  @media only screen and (max-width: 800px) {
    .img {
      width: 100%;
    }
  }

  .banner {
    background: transparent
      url("https://24.media.tumblr.com/ccb268832580ac12951828a1c179de69/tumblr_mo2xbk8JUK1st5lhmo1_1280.jpg")
      0 0 no-repeat fixed;
    text-align: center;
    background-size: cover;

    height: 200px;
    width: 100%;
    margin-bottom: 3em;
    display: table;
  }

  .banner-head {
    display: table-cell;
    vertical-align: middle;
    margin-bottom: 0;
    font-size: 2em;
    color: white;
    font-weight: 500;
    text-shadow: 0 1px 1px black;
  }
</style>
