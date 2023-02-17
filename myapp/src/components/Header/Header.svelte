<script>
</script>


<h2>Les bases du dev web</h2>
<nav>
  <ul>
    <li><a href="/">Accueil</a></li>
    <li><a href="/publier">Publier</a></li>
    <li><a href="/articles">Articles</a></li>
    <li><a href="/meteo">Meteo</a></li>
  </ul>
</nav>

<style>
    header {
        padding-bottom: 1rem;
        border-bottom: 1px solid black;
    }

    figcaption {
        font-size: 2rem;
        font-weight: bold;
        text-align: center;
        margin: 1rem;
    }

    nav ul {
        display: flex;
        margin: 0 auto;
        padding: 0;
        list-style-type: none;
        justify-content: center;
    }

    nav li {
        padding: 0 1rem 0 1rem;
    }

    nav li:not(:last-child) {
        border-right: 1px solid black;
    }

    nav a {
        color: blue;
    }

</style>
