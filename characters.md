---
title: Characters & Groups
layout: page
description: Who are The Sisters? Read all about Mietti.
landing-title: Who is Who in The Freak Show
show-in-nav: true
order: 3
---

You are in the Freak Show because you have no other option. Even if you're not visibly different, there is something that sets you aside from normal society. Maybe you made yourself different on the outside too even though you weren’t like that to start with.
{:.lead}

<img src="assets/images/barnum-bailey.jpg" class="image fit" alt="Barnum Bailey Gang"/>


Read through the roles listed here. When you've chosen one or more roles you like, go ahead and <a href="apply.html">apply to take part!</a>. The roles are quite open to interpretation and we will work together with you to flesh them out. Some of the roles have <strong>special requirements</strong> in the form of makeup, props or other preparations. Information about these requirements are listed with the character.

<div class="row">
    <div class="6u 12u$(small)">
        <h2>The Freaks</h2>
        <p>
            <em>The Freaks</em>, all have some clearly visible factor that makes them unfit to normal society. They are the star performers of the Freak Show.
        </p>
        <p>
            <ul class="characters">
                {% for character in site.characters %}
                    <li>
                        {% if character.image != empty and character.image != nil %}
                            <img class="image" src="{{ site.baseurl }}/{{ character.image }}" alt="" />
                        {% endif %}
                        <div class="name">{{ character.title }}</div>
                        <div class="role">{{ character.role }}</div>
                        <div class="content">
                            {{ character.content }}
                        </div>
                    </li>
                {% endfor %}
            </ul>
        </p>
    </div>
    <div class="6u 12u$(small)">
        <h2>The Circus Folk</h2>
        <p>
            <em>The Circus Folk</em> travel and work with the circus, but are not visibly different. All of them are not performers, but all are somehow not normal.
        </p>
    </div>
</div>
