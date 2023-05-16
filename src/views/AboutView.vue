<script setup lang="ts">
</script>

<template>
  <main>
    <div class="about">
      <div class="about-section">
        <h1>About Us Page</h1>
        <img alt="Vue logo" class="logo" src="@/assets/team1.jpg" style="width:45%;margin: 20px;" />
        <p>Lorem ipsum dolor sit amet. Ut recusandae assumenda eum voluptas veniam in sunt perferendis est voluptatem aperiam id cumque Quis. Aut ipsum odit ut laboriosam voluptatem ut sequi perferendis ut architecto dolores eum odio corporis ad obcaecati voluptas eum ipsam repellat.</p>
        <p>Non distinctio dolorum est ipsam consectetur id aliquid asperiores qui voluptate vero. Et vero consectetur est laboriosam eius sed architecto consequatur est totam atque.</p>
        <p>Est omnis tenetur sed doloribus similique aut molestias distinctio et omnis consequatur aut blanditiis magni id galisum voluptate? Ut libero illum sit libero exercitationem non optio pariatur sit quia maiores. Cum asperiores explicabo et perspiciatis recusandae quo nihil aspernatur ea harum omnis ex rerum magnam. Rem esse tempore et maxime similique eos veniam obcaecati aut velit totam aut dignissimos atque.</p>
      </div>
    </div>
  </main>
</template>

<style>
  p{
    font-size: 20px;
    font-weight: bold;
  }
  .about-section {
    text-align: center;
    color: rgb(61, 60, 60);
    width: 100%;
    margin-right: 20px;
    font-family: 'Courier New', Courier, monospace;
  }
  h1 {
    text-align: center;
    width: 100%;
    color: rgb(6, 154, 165);
    font-weight: bold;
  }

@media (min-width: 1024px) {
  p{
    font-size: 20px;
    font-weight: bold;
  }
  .about-section {
    text-align: center;
    color: rgb(61, 60, 60);
    width: 100%;
    margin-right: 20px;
    font-family: 'Courier New', Courier, monospace;
  }
  h1 {
    text-align: center;
    width: 100%;
    color: rgb(6, 154, 165);
    font-weight: bold;
  }
  main{
    padding-left: 50px;
  }
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
  }
  body {
    display: flex;
    place-items: center;
  }

  #app {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 0 2rem;
  }

  
}
</style>
