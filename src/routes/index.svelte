<script lang="ts">
  	import "../app.css";
    
</script>

<div class="banner">
	<h1 class="banner-head">
			Placeholder
			<br>
			Text
			Text
			<br>
	</h1>
</div>


<div class="content">
	<h1 class="header">Placeholder</h1>
</div>

<style>
.header{
	color: var(--green);
}

.content{
	display: flex;
  justify-content: center;
  align-items: center;
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
