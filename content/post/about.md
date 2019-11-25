---
title: "About"
date: 2015-11-24T23:39:34-02:00
draft: false
---

<script>
    var avatars = [
        'images/a/1.jpg',
        'images/a/2.PNG',
        'images/a/3.png',
        'images/a/4.png',
        'images/a/5.jpg',
        'images/a/6.png'
    ]

    function getSource()
    {
        return avatars[Math.floor(Math.random()*avatars.length)];
    }

    document.write('<img src="/'+getSource()+'">');
</script>


