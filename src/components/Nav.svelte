<script>
  export let segment;

  const handleClick = () => {
    console.log(segment);
  };
</script>

<nav>
  <div>
    <a class:current={segment === undefined} href=".">Neel Modi</a>
    <ul>
      <li>
        <a class:current={segment === "contact"} href="contact">Contact Me</a>
      </li>
      <li><a class:current={segment === "about"} href="about">About</a></li>
      <li><a class:current={segment === "jobs"} href="blog">Blogs</a></li>
    </ul>
  </div>
</nav>

<style>
  nav {
    height: 70px;
    background: #222;
    color: lightgreen;
  }
  nav div {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
  }
  ul {
    text-align: right;
  }
  li {
    display: inline-block;
    padding: 0.7rem 2rem;
  }
  a {
    text-decoration: none;
    display: block;
    padding-left: 2rem;
  }
  a:hover {
    color: salmon;
  }
</style>
