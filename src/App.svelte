

<main>
  <h1>Hello world</h1>
  <input type="file" />
  <button on:click={() => {
    const now = Date.now().toString();
    localStorage.setItem("name", now)
    alert(now);
  }}>Save</button>
  <button on:click={() => {
    alert(localStorage.getItem("name"))
  }}>Get</button>
</main>