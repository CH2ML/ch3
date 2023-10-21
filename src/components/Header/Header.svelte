<script>
  let links = ['Home', 'Services', 'Blog', 'Launch Pad'];
</script>

<style>
header {
  display: flex;
  justify-content: center; 
  align-items: center;
  background-color: transparent;
  width: 100%; /* Ensures the header takes the full width */
  height: 100px; /* Or any other height you prefer for the header */
  position: relative;
  padding: 10px 30px;
}

nav {
  display: flex;
  justify-content: center; /* Center the items inside the nav bar */
  align-items: center;
  background-color: rgba(40,40,40,1);
  padding: 10px 30px;
  border-radius: 30px;
  box-shadow: 0 3px 6px rgba(0,0,0,0.1);
}

nav a {
  margin: 0 15px;
  text-decoration: none;
  color: white;
  font-size: 16px;
  font-weight: bold;
  transition: color 0.3s;
}

nav a:hover {
  color: green;
}

.logo {
  display: flex;
  align-items: center;
  margin-right: 20px; /* Space between the logo and the navbar */
}

.logo img {
  height: 40px;
  width: auto;
}

.logo a {
  text-decoration: none;
}
</style>

<header>
  <!-- CH3 logo outside of the nav bar -->
  <div class="logo">
    <a href="/">
      <img src="assets/favicon_ch3.svg" alt="ch3 logo" />
    </a>
  </div>
  <nav>
    {#each links as link}
      <a href="home">{link}</a>
    {/each}
  </nav>
</header>
