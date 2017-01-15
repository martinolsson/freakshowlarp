---
title: Characters & Groups
layout: page
description: Who are The Sisters? Read all about Mietti.
landing-title: Who is Who in The Freak Show
show-in-nav: true
order: 3
---

You are in the Freak Show because you have no other option. Even if you're  not visibly different, there is something that sets you aside from normal society. Maybe you made yourself different on the outside too even though you weren’t like that to start with. .. .... ..... .......... ..........
{:.lead}

<div class="row">
    <div class="6u 12u$(small)">
        <h2>The Freaks</h2>
        <p>
            _The Freaks_, who have some clearly visible factor that makes them unfit to normal society. They are the star performers.
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
            _The Circus Folk_, who travel and work with the circus, but are not visibly different. All of them are not performers, but all are somehow not normal.
        </p>
    </div>
</div>
