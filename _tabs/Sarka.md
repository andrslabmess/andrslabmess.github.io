---
layout: post
toc: true
icon: fas fa-duotone fa-solid fa-dna
order: 6
author: Sarka
---


<div class="codepen" data-height="500" data-theme-id="light" data-default-tab="result" data-slug-hash="wBwLVqq" data-pen-title="Martin" data-user="-rka-Salajkov-"  data-prefill='{"title":"Martin","tags":[],"scripts":[],"stylesheets":[]}'>
  <pre data-lang="html">&lt;article class="gallery">
  &lt;img src="https://raw.githubusercontent.com/andrslabmess/andrslabmess.github.io/refs/heads/main/uploads/galery/pic-1.jpg" alt="guitar player at concert" />
  &lt;img src="https://assets.codepen.io/1506195/unsplash-music-1.avif" alt="duo singing"/>
  &lt;img src="https://assets.codepen.io/1506195/unsplash-music-2.avif" alt="crowd cheering" />
  &lt;img src="https://assets.codepen.io/1506195/unsplash-music-3.avif" alt="singer performing" />
  &lt;img src="https://assets.codepen.io/1506195/unsplash-music-4.avif" alt="singer fistbumping crowd" />
  &lt;img src="https://assets.codepen.io/1506195/unsplash-music-5.avif" alt="man with a guitar singing" />
  &lt;img src="https://assets.codepen.io/1506195/unsplash-music-6.avif" alt="crowd looking at a lighted stage" />
  &lt;img src="https://assets.codepen.io/1506195/unsplash-music-7.avif" alt="woman singing on stage" />
&lt;/article></pre>
  <pre data-lang="css">body {
  margin: 0;
  min-height: 100vh;
  display: grid;
  place-items: center;
}

.gallery {
  --size: 100px;
  display: grid;
  grid-template-columns: repeat(6, var(--size));
  grid-auto-rows: var(--size);
  margin-bottom: var(--size);
  place-items: start center;
  gap: 5px;
  
  &:has(:hover) img:not(:hover),
  &:has(:focus) img:not(:focus){
    filter: brightness(0.5) contrast(0.5);
  }

  & img {
    object-fit: cover;
    width: calc(var(--size) * 2);
    height: calc(var(--size) * 2);
    clip-path: path("M90,10 C100,0 100,0 110,10 190,90 190,90 190,90 200,100 200,100 190,110 190,110 110,190 110,190 100,200 100,200 90,190 90,190 10,110 10,110 0,100 0,100 10,90Z");
    transition: clip-path 0.25s, filter 0.75s;
    grid-column: auto / span 2;
    border-radius: 5px;

    &:nth-child(5n - 1) { 
      grid-column: 2 / span 2 
    }

    &:hover,
    &:focus {
      clip-path: path("M0,0 C0,0 200,0 200,0 200,0 200,100 200,100 200,100 200,200 200,200 200,200 100,200 100,200 100,200 100,200 0,200 0,200 0,100 0,100 0,100 0,100 0,100Z");
      z-index: 1;
      transition: clip-path 0.25s, filter 0.25s;
    }
    
    &:focus {
      outline: 1px dashed black;
      outline-offset: -5px;
    }
  }
}</pre></div>
<script async src="https://public.codepenassets.com/embed/index.js"></script>




# Šárka Andrš Salajková, Ph.D.
<br>
[<img src="uploads/buttons_png/contact.png" width="130" alt="email"/>](#contact)


## Brief introduction
<p align="justify">
 A science enthusiast and she hopes to become a scientist. In her free time, she likes just hanging around and she enjoyes creating simple drawings and artwork mainly from wires, beads and resin. She loves scientific discussion with her husband in nature. 
</p>
🧬 🤸‍♀️ 🤘

<!--
## Bio
[More info](https://www.linkedin.com/in/%C5%A1%C3%A1rka-andr%C5%A1-salajkov%C3%A1-4ab582246/)

## Resources
<!--
### Just for fun
[OSEL](https://osel.cz/)<br>
[Compound Interest](https://www.compoundchem.com/)<br>
[The Charismatic Voice](https://www.youtube.com/@TheCharismaticVoice)<br>


### Favorite authors
[Robert Holdstock](https://cs.wikipedia.org/wiki/Robert_Holdstock)<br>
[Ben Aaronovitch](https://en.wikipedia.org/wiki/Ben_Aaronovitch)<br>
[Terry Pratchett](https://en.wikipedia.org/wiki/Terry_Pratchett)<br>
[Robert Fulghum](https://cs.wikipedia.org/wiki/Robert_Fulghum)<br>


### Active relax
[Origin: Artistics gymnastics Cheb](https://www.gymnastikacheb.cz/)<br>
[How it’s going - current coach: Eva Baggenstos](https://www.aerialhoop.ch/kontakt)<br>
[Aerial sport: Karin Odermatt](https://www.youtube.com/@karinodermattcoach)<br>
[Aerial sport:Cara Chapman](https://www.youtube.com/@cchapman1896)<br>
[Mobility training: Nina Strojnik](https://www.youtube.com/@NinaStrojnik)<br>
[Fitness: Maddie Lymburner](https://www.youtube.com/@MadFit)<br>
-->

### “Help will always be given at Hogwarts to those who ask for it.” - Dumbledore
[Dr Zoë J Ayres: Analytical scientist, Mental health advocate](https://www.zjayres.com/)<br>
[How are you?](https://www.how-are-you.ch/)<br>
[UZH: Advice & Support](https://www.students.uzh.ch/en/advice.html)<br>
[Mark Manson: The Subtle Art of Not Giving a F*ck](https://markmanson.net/)<br>



## Jekyll - The Static Site Generator: Chirpy
[Chirpy](https://chirpy.cotes.page/)<br>
[Chirpy-starter](https://github.com/cotes2020/chirpy-starter)<br>
[Techno Tim](https://technotim.live/posts/jekyll-docs-site/#creating-a-post)<br>




<!--
[Gerald Tuimaleali'ifano](https://geraldtui.com/)<br>
[Denise Case: Embedding a Calendar in a GitHub Pages Website](https://denisecase.github.io/web%20development/2015/07/10/add-calender-to-site/)
[Jinchao Li](https://jinchaoli.com/)<br>
[lazy Ren](https://lazyren.github.io/about/)


#### Chirpy: Change the Home page from Blog to Page
The life is too short to make it difficult ... but there are most likely better ways .... 

I made changes in `index.html`.

Original:
```bash
---
layout: home
# Index page
---
```

Current:
```bash
---
layout: page
# Index page
---

<!DOCTYPE html>

<div class="container">
    <img src="uploads/ProfilePic/Untitled-2.png" alt="Description of image" class="center">
</div>

<html>
  <head>
    <title>Landing Page</title>
  </head>
  <body>
    <h1></h1>
    
  </body>
</html>
```
-->

### Get in touch 
{: #contact }


{% include contact-form.html %}