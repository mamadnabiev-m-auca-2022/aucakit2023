<script>
import { Deta } from 'deta';
import { onMount } from 'svelte';
const deta = Deta("d0dhp8hdn6k_yQ3Ensa19crVSCufhByexm3EbVYBwrzj");
const db = deta.Base('hero');

let articles = [];
  let newArticleTitle = '';
  let newArticleDescription = '';
  let newArticleImage = '';
  let newArticlePosition = 'left';
  let articleToUpdate = 'laptop1';

//let name = ""

//getArticles()

//async function getArticles() {
    //const data = await db.get('123')
   // name = data.text
  //  console.log(data);
//}

onMount(async () => {
    try {
      await fetchArticles();
    } catch (error) {
      console.error('Error fetching articles:', error);
    }
  });

  async function fetchArticles() {
    const result = await db.fetch();
    articles = result.items || [];
  }

async function addArticle() {
    const updatedArticle = {
      key: articleToUpdate,
      title: newArticleTitle,
      description: newArticleDescription,
      image: newArticleImage,
      position: newArticlePosition
    };

    await db.put(updatedArticle);
    await fetchArticles(); // Refresh the articles

    // Reset form fields
    newArticleTitle = '';
    newArticleDescription = '';
    newArticleImage = '';
    newArticlePosition = 'left';
  }

</script>

<!-- Display Articles -->
{#each articles as article}
  <section class="content-block {article.position}-background">
    {#if article.position === 'right'}
      <img src={article.image} alt={article.title}>
    {/if}
    <div class="content-text">
      <h2>{article.title}</h2>
      <p>{article.description}</p>
    </div>
    {#if article.position === 'left'}
      <img src={article.image} alt={article.title}>
    {/if}
  </section>
{/each}

<!-- Article Update Form -->
<form on:submit|preventDefault={addArticle}>
  <select bind:value={articleToUpdate}>
    <option value="laptop1">High-Performance Laptops</option>
    <option value="laptop2">Sleek and Lightweight Laptops</option>
  </select>
  <input type="text" bind:value={newArticleTitle} placeholder="Title">
  <textarea bind:value={newArticleDescription} placeholder="Description"></textarea>
  <input type="text" bind:value={newArticleImage} placeholder="Image URL">
  <select bind:value={newArticlePosition}>
    <option value="left">Left</option>
    <option value="right">Right</option>
  </select>
  <button type="submit">Update Article</button>
</form>
