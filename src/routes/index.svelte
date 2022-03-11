<script lang="ts">
  import "../app.css";
</script>

<!-- <div class="banner">
	<h1 class="banner-head">
			Placeholder
			<br>
			Text
			Text
			<br>
	</h1>
</div> -->

<div class="content">
  <img src="image.png" alt="" />
  <!-- <h1 class="header">Placeholder</h1> -->

  <div class="contact">
    <a href="tel:+1732 209 0105">Contato: (732) 209 0105</a>
  </div>
</div>

<style>
  .contact {
    width: 180px;
    position: fixed;
    top: 80%;
    right: 5%;
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

  img {
    display: block;
    height: 100%;
  }


  @media only screen and (max-width: 800px) {
    img {
      width: 100%;
    }

    .contact{
      top: 44%;
      right: 5%;
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
