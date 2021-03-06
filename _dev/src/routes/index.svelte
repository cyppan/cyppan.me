<svelte:head>
	<title>
		@cyppan | Hello 👋, I’m Cyprien Pannier, a freelance developer based near Montpellier in France. I like strength training and reading. I also grow wine grapes and vegetables.
	</title>
	<link rel="canonical" href="https://cyppan.me/">
	<meta property="og:title" content="@cyppan">
	<meta property="og:locale" content="en_US">
	<meta name="description" content="Hello 👋, I’m Cyprien Pannier, a freelance developer based near Montpellier in France. I like strength training and reading. I also grow wine grapes and vegetables.">
	<meta property="og:description" content="Hello 👋, I’m Cyprien Pannier, a freelance developer based near Montpellier in France. I like strength training and reading. I also grow wine grapes and vegetables.">
	<meta property="og:url" content="https://cyppan.me/">
	<meta property="og:site_name" content="@cyppan">
	<script type="application/ld+json">
		{"@type":"WebSite","url":"https://cyppan.me/","headline":"@cyppan","name":"@cyppan","description":"Hello 👋, I’m Cyprien Pannier, a freelance developer based near Montpellier in France. I like strength training and reading. I also grow wine grapes and vegetables.","@context":"https://schema.org"}
	</script>
</svelte:head>

<script>
	const articles = [
		{
			link: "https://medium.com/@cyppan/vers-un-nouveau-mode-dorganisation-du-travail-81ad33d26cb",
			title: "Vers un nouveau mode d'organisation du travail",
			source: "medium",
			category: "work"
		},
		{
			link: "https://medium.com/@cyppan/pens%C3%A9es-dun-millennial-14f43b13c629",
			title: "Pensées d'un millennial",
			source: "medium",
			category: "life"
		},
		{
			link: "https://medium.com/@cyppan/dealing-with-long-term-future-for-the-high-functioning-anxious-7910a467f977",
			title: "Dealing with long-term future for the high functioning anxious",
			source: "medium",
			category: "life"
		},
		{
			link: "https://medium.com/@cyppan/the-fair-enough-strategy-in-life-80ef9dfd0f1b",
			title: 'The "fair enough" strategy in life',
			source: "medium",
			category: "life"
		},
		{
			link: "https://medium.com/@cyppan/how-clojure-helps-you-build-powerful-abstractions-a89c25ba573e",
			title: "How Clojure helps you build powerful abstractions",
			source: "medium",
			category: "tech"
		}
	];
	const categories = [...new Set(articles.map(a => a.category))];
	console.log("categories", categories);
</script>

<section class="section">
  <div class="container">
    <article class="media">
      <figure class="media-left">
        <p class="image is-128x128">
          <img src="https://avatars2.githubusercontent.com/u/1446201?s=400&u=92132a6e30f38aa03abb8c2e72b76d39639a2104&v=4">
        </p>
      </figure>
      <div class="media-content">
        <h1 class="title">
          Hello 👋, I’m Cyprien, a freelance developer based near Montpellier in France.
        </h1>
        <h2 class="subtitle">
          I like strength training and reading. I also grow wine grapes and vegetables (do you know about <a href="https://farm.bot/" target="_blank">farmbot</a>?)
        </h2>
        <h2 class="subtitle">
          My skills evolve around <strong>backend</strong> (Javascript, Clojure), <strong>architecture</strong> (highly available services, large scale volumetry) and <strong>devops</strong> (CI/CD, Docker, AWS, GCP) stuff, feel free to <a href="mailto:contact@cyppan.me">contact me</a> for professional collaboration or thought-provoking discussions about life & cosmos.
        </h2>

        <p class="buttons">
          <a class="button is-primary" href="https://www.linkedin.com/in/cyprien-pannier-01a64582">
            <span class="icon">
              <i class="fab fa-linkedin"></i>
            </span>
            <span>LinkedIn</span>
          </a>
          <a class="button is-primary" href="https://github.com/cyppan">
            <span class="icon">
              <i class="fab fa-github"></i>
            </span>
            <span>GitHub</span>
          </a>
          <a class="button is-primary" href="https://twitter.com/cyppan">
            <span class="icon">
              <i class="fab fa-twitter"></i>
            </span>
            <span>Twitter</span>
          </a>
          <a class="button is-primary" href="https://medium.com/@cyppan">
            <span class="icon">
              <i class="fab fa-medium"></i>
            </span>
            <span>Medium</span>
          </a>
        </p>

        <h2 class="subtitle">
          You can have a look at some of my <a href="#code">(open source) code ⬇️</a> and <a href="#articles">articles ⬇️</a>. There is more to come, stay tuned.
        </h2>
      </div>
    </article>
  </div>
</section>

<section class="section">
  <div class="container">
    <h1 class="title"><a id="code"></a># Code</h1>
  </div>
  <div class="tile is-ancestor" style="margin-top:10px">
    <div class="tile is-parent is-vertical">
      <article class="tile is-child notification box is-light">
        <p class="title">Grape</p>
        <p class="subtitle">
          An opinionated, data-first, graphy Clojure library to build HTTP APIs
        </p>
        <div class="content">
          Combine Clojure efficiency and APIs best practices to ease developers' life. A slightly modified version of it is used in production at BeOp.
          <br />
          <a href="https://github.com/cyppan/grape">
            <span class="icon"><i class="fab fa-github"></i></span>
            <span>See more</span>
          </a>
        </div>
        <span class="tag is-dark">clojure</span>
        <span class="tag is-dark">mongodb</span>
      </article>
    </div>
    <div class="tile is-parent">
      <article class="tile is-child notification box is-light">
        <p class="title">
          serve-sequelize
        </p>
        <p class="subtitle">For quick node.js REST API prototyping</p>
        <div class="content">
          Make use of the great ORM sequelize and expose schema-defined resources safely to the web.
          I've used this one to do some API prototypes for quick POC at Koba.
          <br />
          <a href="https://github.com/cyppan/serve-sequelize">
            <span class="icon"><i class="fab fa-github"></i></span>
            <span>See more</span>
          </a>
        </div>
        <span class="tag is-dark">javascript</span>
        <span class="tag is-dark">node.js</span>
        <span class="tag is-dark">sql</span>
      </article>
    </div>
    <div class="tile is-parent">
      <article class="tile is-child notification box is-light">
        <div class="content">
          <p class="title">validate-data-tree</p>
          <p class="subtitle">declarative json validation library used in serve-sequelize.</p>
          <div class="content">
            This library aims to validate data structures (input object, possibly with nested objects and arrays), by the mean of data structures (the schema).
            <br />
            <a href="https://github.com/cyppan/validate-data-tree">
              <span class="icon"><i class="fab fa-github"></i></span>
              <span>See more</span>
            </a>
          </div>
          <span class="tag is-dark">javascript</span>
        </div>
      </article>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <h1 class="title"><a id="articles"></a># Articles</h1>
    <div class="content">
      <h3>
        <a href="https://medium.com/@cyppan/vers-un-nouveau-mode-dorganisation-du-travail-81ad33d26cb">
          Vers un nouveau mode d'organisation du travail
          <span class="icon"><i class="fab fa-medium"></i></span>
        </a>
      </h3>
      <h3>
        <a href="https://medium.com/@cyppan/pens%C3%A9es-dun-millennial-14f43b13c629">
          Pensées d'un millennial
          <span class="icon"><i class="fab fa-medium"></i></span>
        </a>
      </h3>
      <h3>
        <a href="https://medium.com/@cyppan/dealing-with-long-term-future-for-the-high-functioning-anxious-7910a467f977">
          Dealing with long-term future for the high functioning anxious
          <span class="icon"><i class="fab fa-medium"></i></span>
        </a>
      </h3>
      <h3>
        <a href="https://medium.com/@cyppan/the-fair-enough-strategy-in-life-80ef9dfd0f1b">
          The "fair enough" strategy in life
          <span class="icon"><i class="fab fa-medium"></i></span>
        </a>
      </h3>
      <h3>
        <a href="https://medium.com/quidli/about-fair-multi-party-compensations-in-early-stage-projects-3aebb94a6cd">
          About fair multi-party compensation in early-stage projects
          <span class="icon"><i class="fab fa-medium"></i></span>
        </a>
      </h3>
      <h3>
        <a href="https://medium.com/@cyppan/how-clojure-helps-you-build-powerful-abstractions-a89c25ba573e">
          How Clojure helps you build powerful abstractions
          <span class="icon"><i class="fab fa-medium"></i></span>
        </a>
      </h3>
    </div>
  </div>
</section>