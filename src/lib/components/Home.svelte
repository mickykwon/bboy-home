<script>
  import Header from './Header.svelte';
  import Footer from './Footer.svelte';

</script>

<Header />
<main class='container'>
  <video 
    autoplay loop muted
    src="video/title.mp4"
  ></video>
</main>
<Footer />

<style>
  video {
    width: 100%;
    aspect-ratio: 2.35/1;
    object-fit: cover;
    object-position: center;
    display: block;
  } 

 .container {
    display: flex;
    justify-content: center;
    align-items: center;
    /* height: 100vh; */
    background: #fff;
  }

  @media (max-width: 516px) {
    main {
      height: calc(100vh - 138px - 66px);
    }
    video {
      width: 100%;
      height: 100%;
      /* aspect-ratio: 2.35/1; */
      object-fit: cover;
      object-position: center;
      display: block;
    } 
  }
</style>