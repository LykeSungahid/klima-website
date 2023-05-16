<script setup lang="ts">
</script>

<template>
  <main>
    <div class="contact">
      <div class="contact-section">
        <h1>Contact Us</h1>
        <p>Have any inquiries? We'd love to hear from you!</p>
      </div>
      <div class="contact-section">
        <div class="card">
          <img src="@/assets/locationlogo.png" alt="Avatar" style="width:10%">
          <div class="container">
            <h4><b>907 Borja Bldg. Jakosalem Street,</b></h4> 
            <h4><b>Barangay Zapatera, Cebu Citiy</b></h4> 
            <p>Non distinctio dolorum est ipsam consectetur id aliquid asperiores qui voluptate vero. Et vero consectetur est laboriosam eius sed architecto consequatur est totam atque.</p> 
          </div>
        </div>

        <div class="card">
          <img src="@/assets/emaillogo.png" alt="Avatar" style="width:10%">
          <div class="container">
            <h4><b>klimaengg@gmail.com</b></h4> 
            <p>Non distinctio dolorum est ipsam consectetur id aliquid asperiores qui voluptate vero. Et vero consectetur est laboriosam eius sed architecto consequatur est totam atque.</p> 
          </div>
        </div>

        <div class="card">
          <img src="@/assets/phonelogo.png" alt="Avatar" style="width:10%">
          <div class="container">
            <h4><b>(032) 343 - 4716</b></h4> 
            <p>Non distinctio dolorum est ipsam consectetur id aliquid asperiores qui voluptate vero. Et vero consectetur est laboriosam eius sed architecto consequatur est totam atque.</p> 
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style>
  h4{
    font-weight: bold;
  }
  .card {
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;
    width: 75%;
    min-height: 200px;
    margin-bottom: 25px;
    margin-left: auto;
    margin-right: auto;
  }
  .container {
    width: 100%;
  }
  .contact-section {
    text-align: center;
    align-items: center;
    color: rgb(61, 60, 60);
    width: 100%;
    margin-right: 20px;
    font-family: 'Courier New', Courier, monospace;
  }
  p{
    font-size: 20px;
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
  .contact {
    min-height: 100vh;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
  }
@media (min-width: 1024px) {
  h4{
    font-weight: bold;
  }
  .card {
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    transition: 0.3s;
    width: 75%;
    min-height: 200px;
    margin-bottom: 25px;
    margin-left: auto;
    margin-right: auto;
  }
  .container {
    width: 100%;
  }
  .contact-section {
    text-align: center;
    align-items: center;
    color: rgb(61, 60, 60);
    width: 100%;
    margin-right: 20px;
    font-family: 'Courier New', Courier, monospace;
  }
  p{
    font-size: 20px;
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
  .contact {
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