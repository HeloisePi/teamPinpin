<script>
  import FilAriane from '../../Componante/utilities/FilAriane.svelte';
  import GridImage from '../../Componante/utilities/GridImage.svelte';
  import { lesnoirsetblancs } from '/src/routes/imagesList.js' 
</script>
  
<FilAriane 
pageName = "Les créations de Serge"
pageSrc = "/creationSerge">
<p>></p>
<a href="/creationSerge/lesnoirsetblancs">les noirs et blancs</a>
</FilAriane>
<h1>Les noirs et blancs</h1>

<div>
<GridImage>
  {#each lesnoirsetblancs as src  }
  <img src="{src}" alt="tableau Serge Pingitore sur le théme du noir et blanc"> 
  {/each}
</GridImage>

</div>
<style>
  div{
    margin-bottom: 10rem;
  }
  h1{
    margin-top: 5rem;
    text-align: center;
  }
img{
        width: 15rem;
        height: auto;
        transition: 500ms;

    }
  img:hover{
    transform: scale(110%);
  }
</style>