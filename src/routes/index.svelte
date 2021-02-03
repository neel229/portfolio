<script lang="ts">
  let name: string = "";
  console.log(name);
  const stayAnonymous = () => {
    name = "abc";
  };
</script>

<main>
  <div class="name-box">
    <h1>Enter Your Name! <span>(It won't be stored &#128517;)</span></h1>
    <input type="text" bind:value={name} />
    <p>Your name is {name}</p>
    <a href="about">Proceed</a>
    <button on:click={stayAnonymous}>Stay anonymous</button>
  </div>
  <img src="background.jpg" alt="background" />
</main>

<style>
  main {
    height: 100vh;
    width: 100%;
  }

  span {
    font-size: 16px;
  }

  img {
    height: 100%;
    width: 100%;
  }

  div.name-box {
    align-items: center;
    justify-content: center;
    display: flex;
    flex-direction: column;
    position: fixed;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
  }

  div.name-box h1 {
    text-align: center;
  }

  input {
    font-size: 24px;
  }

  a {
    font-size: 18px;
  }

  button {
    size: 1.2em;
    background-color: #222;
    color: lightblue;
    border-radius: 12px;
    padding: 0.75rem 0.75rem;
    text-align: center;
    text-decoration: none;
    margin-top: 10px;
    font-size: 20px;
    border: none;
  }
</style>
