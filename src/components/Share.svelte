<style>
  .Share {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 4px;
    background-color: white;
    margin: 0 0 2em 0;
    width: 300px;
    height: 80px;
    position: fixed;
    top: 50%;
    left: 50%;
    z-index: 9;
    padding: 1em;
    transform: translate(-50%, -50%);
  }
  .Share-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .Share-head h2 {
    font-size: 16px;
  }
  .Share-head i {
    cursor: pointer;
  }
  .Share-content a {
    display: flex;
    align-items: center;
    text-decoration: none;
    color: black;
    font-size: 14px;
    margin: 2em 0 0 0;
  }

  .Share-content span {
    font-family: "Lato", sans-serif;
    font-size: 14px;
    margin-left: 10px;
  }

  .Share-content i {
    color: #3b5998;
    margin: 0 0.5em 0 0;
    font-size: 20px;
  }
</style>

<div class="Share">
  <div class="Share-head">
    <h2>Compartir</h2>
    <i class="fas fa-times-circle" on:click />
  </div>
  <div class="Share-content">
    <a target="_blank" rel="noopener" href="https://www.facebook.com/sharer/sharer.php?u=https://pugstagram.co">
      <i class="fab fa-facebook-square">
      <span>Compartir en Facebook</span> 
    </a>
  </div>
</div>