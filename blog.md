---
title: Theo Englund - blogg
permalink: /blog.html
---

<!DOCTYPE html>
<html lang=sv>
<head>
    <meta charset=utf-8>
    <meta name=viewport content=width=device-width, initial-scale=1>
    <title>Theo Englund</title>
    <link rel=stylesheet href=style.css>
</head>
<body>

    <header>
        <h1>Theo Englund - blogg</h1>
        <p></p>
    </header>

    <hr>

    <nav>
     <table style="width: 100%;">
        <tr>
            <td>
                [ <a href="index.html">Tillbaka</a> ]
                [ <a href="blog.html">Blogg</a> ]
            </td>
            <td style="text-align: right;">
                [ <a href="feed.xml">RSS</a> ]
            </td>
        </tr>
      </table>
    </nav>


    <hr>

    <ul class="post-list">
    {% for post in site.posts %}
    <li>
        <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
    {% else %}
    <li>Bloggen är tom för tillfället...</li>
    {% endfor %}
    </ul>
    <!--

    <ul class="post-list">
    <li>
        <span class="post-date">2026-09-05</span>
        <a href="blog/sida.html">Min nya sida</a>
    </li>
    <li>
        <span class="post-date">2026-08-21</span>
        <a href="blog/test.html">Testar sidan</a>
    </li>
    </ul>

    <!--	
    <li>
        <span class="post-date">yyyy-mm-dd</span>
        <a href="blog/titel.html">Titel</a>
    </li>
    -->

    <footer>
        <hr>
        <p>senast uppdaterad: 2026-09-10</p>
        <p>Theo Englund &copy; 2026</p>
    </footer>

</body>
</html>
