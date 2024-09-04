<script>
    import landingbg from "$lib/img/landingbg.webp"
      import Fa from 'svelte-fa'
  import { faPowerOff } from '@fortawesome/free-solid-svg-icons'
</script>

<div class="landingbg">
    <img src={landingbg} alt="landingbg" class="landingbg" />
    <div class="overlay"></div>
</div>
<div class="container rounded-lg landingcontainer mx-auto flex items-end justify-center">
    <button class="btn btn-primary glass btn-wide btn-lg mb-16 flex flex-row justify-start">
        <Fa class="flex-none w-4" icon={faPowerOff}></Fa>
        <div class="flex-1 w-64 justify-self-end">START</div>
    </button>
</div>

<style>
    .landingbg {
        object-fit: cover;
        height: 100%;
        width: 100%;
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        z-index: 0;
    }
    .overlay {
        -webkit-filter: blur();
        filter: blur();
        height: 100vh;
        z-index: 1;
        position: relative;
        background: rgb(9,9,121);
        background: linear-gradient(90deg, rgba(9,9,121,1) 14%, rgba(0,125,255,1) 100%);
        opacity:90%
    }
    .landingcontainer {
        position: relative;
        z-index: 2;
        height: 800px;
        width: 600px;
        margin-top: 200px;
        background: rgba(11, 3, 59, 0.75)
    }
</style>