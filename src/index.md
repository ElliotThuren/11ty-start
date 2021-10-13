---
title: "Testsida med 11ty och sass kombonerat"
layout: "base.njk"
templateEngineOverride: njk, md
---

<body>
    <nav class="navbar">
    <div class="navbar-inner container">
        <img src="../sass/sassimg/school_black_36dp.svg" alt="">
        <a class="navbar-brand" href="#">LOREM-IPSUM</a>
        <ul class="nav">
            <li class="nav-item"><a href="#" class="nav-link">Home</a></li>
            <li class="nav-item"><a href="#" class="nav-link">About</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Contact</a></li>
        </ul> 
    </div>
    </nav>
    <main class="container">
        <header class="cta">
            <div class="cta-filter"></div>
            <h1>Beatae Magni!</h1>
            <div class="cta-right">
                <p>Expedita deserunt libero accusantium!</p>
                <p>Praesentium earum alias?</p>
                <button>
{% for article in collections.articles %}
<li><a href="{{ article.url }}">{{ article.data.title }}</li>
{% endfor %}
</button>
            </div>
        </header>
          <div class="card-group">
        <div class="card card1">
            <img src="https://picsum.photos/370/101" alt="" class="img">
            <h1 class="card-text">Illo quasi enim</h1>
            <p class="card-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus at eaque officia blanditiis voluptate error obcaecati ipsa dolorem quas? Aperiam voluptatem fugiat delectus vero harum quasi quisquam suscipit, consectetur velit?</p>
            <button class="card-text card-button">{% for post in collections.post | randomPost %}
<a href="{{ post.url }}">{{ post.data.title }}</a>
{% endfor %}</button>
        </div>
        <div class="card card2">
            <img src="https://picsum.photos/371/101" alt="" class="img">
            <h1 class="card-text">Consectetur sit</h1>
            <p class="card-text">Lorem ipsum dolor sit amet consectetur, adipisicing elit aut. Sit, suscipit. Illo quasi enim inventore perspiciatis. Sed quos voluptas nam nisi dolorem sunt eveniet tenetur magni nulla, voluptatum voluptatibus doloremque impedit.</p>
            <button class="card-text card-button">{% for post in collections.post | randomPost %}
<a href="{{ post.url }}">{{ post.data.title }}</a>
{% endfor %}</button>
        </div>
          </div>
        <div class="card-group">
        <div class="card card3">
            <img src="https://picsum.photos/370/100" alt="" class="img">
            <h1 class="card-text">Incidunt labore</h1>
            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione ex quaerat ea natus, voluptatum officiis, molestiae quos nam quam aliquam beatae maxime nostrum illum consequuntur alias, facilis incidunt labore quidem?</p>
            <button class="card-text card-button">{% for post in collections.post | randomPost %}
<a href="{{ post.url }}">{{ post.data.title }}</a>
{% endfor %}</button>
        </div>
        <div class="card card4">
            <img src="https://picsum.photos/371/100" alt="" class="img">
            <h1 class="card-text">Necessitatibus</h1>
            <p class="card-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quibusdam iste assumenda quas odit expedita minima nemo necessitatibus aut. Quas ullam rerum nihil sunt perferendis? Commodi necessitatibus est nobis dicta adipisci.</p>
            <button class="card-text card-button">{% for post in collections.post | randomPost %}
<a href="{{ post.url }}">{{ post.data.title }}</a>
{% endfor %}</button>
        </div>
    </div>
    </main>
    <footer class="footer">
        <div class="container">
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Numquam iure odio similique magni dicta quibusdam pariatur error voluptatum? Optio iusto aliquid cum molestias, deleniti ipsa temporibus necessitatibus eligendi quas eaque?Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil tempore officia asperiores, ex culpa, minus, quo odio ab officiis harum similique dolorum! Amet nisi, et laudantium illum alias provident inventore?Lorem ipsum dolor sit amet consectetur, adipisicing elit. Praesentium eius ipsam repellat quisquam dolore? Officiis quo vero accusamus nostrum?</p>  
        </div>
    </footer>
</body>