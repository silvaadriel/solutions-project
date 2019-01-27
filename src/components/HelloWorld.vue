<template>
  <div id="wrapper">
    <base-nav
      :nav-items-array="navItemsArray"
    />

    <main>
      <base-highlights
        :highlights-array="hightlightsArray"
      />
      <section id="portfolio" class="container">
        <h2 class="subtitulo">Portfólio</h2>

        <ul class="slider">
          <li>
            <input type="radio" name="img" id="radio1" checked>
            <label for="radio1"></label>
            <img src="../assets/images/daniel-chen-108577-unsplash.jpg" alt="">
          </li>
          <li>
            <input type="radio" name="img" id="radio2">
            <label for="radio2"></label>
            <img src="../assets/images/floriane-vita-88722-unsplash.jpg" alt="">
          </li>
          <li>
            <input type="radio" name="img" id="radio3">
            <label for="radio3"></label>
            <img src="../assets/images/freeman-zhou-1252466-unsplash.jpg" alt="">
          </li>
          <li>
            <input type="radio" name="img" id="radio4">
            <label for="radio4"></label>
            <img src="../assets/images/joel-filipe-171928-unsplash.jpg" alt="">
          </li>
          <li>
            <input type="radio" name="img" id="radio5">
            <label for="radio5"></label>
            <img src="../assets/images/lance-anderson-213491-unsplash.jpg" alt="">
          </li>
          <li>
              <input type="radio" name="img" id="radio6">
              <label for="radio6"></label>
            <img src="../assets/images/patrick-tomasso-1272187-unsplash.jpg" alt="">
          </li>
          <li>
            <input type="radio" name="img" id="radio7">
            <label for="radio7"></label>
            <img src="../assets/images/sean-pollock-203658-unsplash.jpg" alt="">
          </li>
      </ul>
      <div class="call">
          <a href="#" class="btn">Ver mais</a>
      </div>
      </section>

      <section id="sobre" class="container">
        <h2 class="subtitulo">Sobre</h2>
        <div class="sobre">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam expedita consequatur iste magnam obcaecati natus id itaque, sed tenetur necessitatibus dolores veritatis quas harum ut temporibus delectus a! Repellendus, libero? Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore distinctio, amet delectus accusamus ea maiores.</p>
          <img src="../assets/images/freeman-zhou-1252466-unsplash-square.jpg" alt="">
        </div>
        <div class="call">
            <a href="#" class="btn">Ver mais</a>
        </div>
      </section>

      <section id="contato" class="container">
          <h2 class="subtitulo">Contato</h2>
      </section>

    </main>

  </div>
</template>

<style>
*, *:before, *:after {
    box-sizing: inherit;
    box-sizing: inherit;
  }
  
  html {
    box-sizing: border-box;
  }
  
  body, p, ul, li, h2, h1, a {
    padding: 0px;
    margin: 0px;
  }
  
  body {
    font-family: Arial, Helvetica, sans-serif;
    background-color: #ddd;
  }
  
  img {
    max-width: 100%;
    display: block;
  }
  
  a {
    text-decoration: none;
  }
  
  ul {
    list-style: none;
  }
  
  .subtitulo {
    font-size: 1.5em;
    line-height: 1.875em;
    font-weight: bold;
    letter-spacing: .1em;
    text-transform: uppercase;
    text-align: center;
    margin-bottom: 1.5em;
  }
  
  .subtitulo:after {
    content: " ";
    display: block;
    width: 60px;
    height: 3px;
    background: #636363;
    margin: 10px auto;
  }
  
  .btn {
    border-radius: 8px;
    border: 0;
    background: rgba(44, 141, 158, 0.493);
    cursor: pointer;
    font-weight: bold;
    color: #636363;
    font-size: 1em;
    text-transform: uppercase;
    padding: 1em 1.5em;
    transition: all .3s ease;
  }
  
  .btn:hover {
    background: #2C8D9E;
    color: #fff; 
  }
  
  .call {
    text-align: center;
    padding: 2em 0 3em 0em;
  }
  
  @media screen and (max-width: 480px) {
    .subtitulo {
      font-size: 1.2em;
    }
    .btn {
      font-size: .875em;
      padding: .875em 1em;
    }
  }
  
  /* Header */
  
  #header {
    width: 100%;
    height: 40.7em;
    margin-bottom: -100px;
    background: url("../assets/images/patrick-tomasso-1272187-unsplash.jpg") no-repeat center;
    background-size: cover;
    padding: 5em 5em 1em 5em;
    text-align: center;
  }
  
  #logo h1 {
    color: #fff;
    font-weight: bold;
    font-size: 4em;
    padding-top: 100px;
    margin-bottom: 40px;
  }
  
  .quote {
    max-width: 500px;
    margin: 0 auto;
    font-size: 1em;
    line-height: 1.5em;
    color: #fff;
    font-style: italic;
    margin-bottom: 50px;
  }
  
  .quote p:before, .quote p:after {
    content: " ";
    display: block;
    width: 60px;
    height: 3px;
    background: #fff;
    margin: 14px auto 10px auto;
  }
  
  .quote cite {
    font-size: .875em;
    color: #fff;
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: .1em;
    font-style: normal;
  }
  
  @media screen and (max-width: 480px) {
    #header {
      margin-bottom: 0;
      padding: 4em 2em 1em 2em;
    }
  
    .quote {
      font-size: 1em;
    }
  }
  
  /* Wrapper */
  
  #wrapper {
    width: 74em;
    max-width: calc(100% - 4em);
    margin: 0 auto;
    border-radius: 0.25em;
    background-color: #fff;
    box-shadow: 0px 0px 6px 2px rgba(0, 0, 0, .1);
  }
  
  @media screen and (max-width: 480px) {
    #wrapper {
      max-width: 100%;
      border-radius: 0;
    }
  }
  /* Main */
  
  main {
    color: #636363;
    border-radius: 0.25em;
  }
  
  .container {
    max-width: calc(100% - 4em);
    padding: 4em 2em 2em 2em;
    margin: 0 auto;
    border-top: 1px #ccc solid;
  }
  
  @media screen and (max-width: 480px) {
    .container {
      padding: 2em 0 1em 0;
    }
  }
  
  .container:first-child, footer.container {
    border-top: none;
  }
  
  #destaque {
    padding-top: 8em;
  }
  
  #destaque li {
    margin: 0 .1em;
    font-size: 1em;
    text-align: center;
    padding: 1em;
    border-radius: 0.25em;
    transition: all .3s ease;
  }
  
  #destaque li img {
    border-radius: 0.25em;
  }
  
  #destaque li h3:after {
    content: " ";
    display: block;
    width: 60px;
    height: 3px;
    background: #636363;
    margin: 8px auto;
  }
  
  #destaque li:hover {
    background: rgba(44, 141, 158, 0.493);
    color: #fff;
  }
  
  #destaque li:hover h3:after {
    background: #fff;
  }
  
  /* Features */
  
  .features {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 0;
  }
  
  .features li {
    width: calc(33% - 2em);
    margin-left: 2em;
    margin-top: 3em;
    padding: 0;
  }
  
  @media screen and (max-width: 480px) {
    .features {
      display: block;
    }
  
    .features li {
    width: 100%;
    margin-left: 0;
    margin-top: 3.5em;
    }
  
    #destaque {
      padding-top: 4em;
    }
  } 
  
  /* Portfolio */
  
  .slider {
    display: block;
    height: 30.5em;
    max-height: calc(100% - 4em);
    width: 54em;
    max-width: calc(100% - 4em);
    margin: auto;
    margin-top: 60px;
    position: relative;
  }
    
   .slider li {
    list-style: none;
    position: absolute;
  }
  
   .slider img {
    margin: auto;
    height: 100%;
    width: 100%;
    vertical-align: top;
    border-radius: 0.25em;
  } 
  
  .slider input {
    display: none;
  }
  
  .slider label {
    background-color: #000;
    bottom: 10px;
    border-radius: 50px;
    box-shadow: 0px 2px 3px 2px rgba(0, 0, 0, .5);
    opacity: .8;
    cursor: pointer;
    display: block;
    height: 2.5em;
    position: absolute;
    width: 2.5em;
    z-index: 10;
    transition: all .3s ease;
  }
  
  .slider li:nth-child(1) label {
    background: url(../assets/images/daniel-chen-108577-unsplash-thumb.jpg) no-repeat center;
    background-size: cover; 
    left: 10px;
    top: -30px;
  }
  
  .slider li:nth-child(2) label {
    background: url(../assets/images/floriane-vita-88722-unsplash-thumb.jpg) no-repeat center;
    background-size: cover; 
    left: 60px;
    top: -30px;
  }
  
  .slider li:nth-child(3) label {
    background: url(../assets/images/freeman-zhou-1252466-unsplash-thumb.jpg) no-repeat center;
    background-size: cover; 
    left: 110px;
    top: -30px;
  } 
  
  .slider li:nth-child(4) label {
    background: url(../assets/images/joel-filipe-171928-unsplash-thumb.jpg) no-repeat center;
    background-size: cover; 
    left: 160px;
    top: -30px;
  } 
  
  .slider li:nth-child(5) label {
    background: url(../assets/images/lance-anderson-213491-unsplash-thumb.jpg) no-repeat center;
    background-size: cover; 
    left: 210px;
    top: -30px;
  } 
  
  .slider li:nth-child(6) label {
    background: url(../assets/images/patrick-tomasso-1272187-unsplash-thumb.jpg) no-repeat center;
    background-size: cover; 
    left: 260px;
    top: -30px;
  } 
  
  .slider li:nth-child(7) label {
    background: url(../assets/images/sean-pollock-203658-unsplash-thumb.jpg) no-repeat center;
    background-size: cover; 
    left: 310px;
    top: -30px;
  } 
  
  .slider img {
    opacity: 0;
    visibility: hidden;
    transition: all .3s ease;
  }
  
  .slider li input:checked ~ label {
    opacity: 1;
    width: 42px;
    height: 42px;
  }
  
  .slider li input:checked ~ img {
    opacity: 1;
    visibility: visible;
    z-index: 10;
  } 
  
  @media screen and (max-width: 480px) {
    .slider {
      display: block;
      height: 10em;
      max-width: 100%;
      margin: auto;
      margin-top: 60px;
      position: relative;
    }
  
    .slider label {
      height: 1.5em;
      width: 1.5em;
    }
  
    .slider li:nth-child(1) label {
      left: 1em;
    }
    
    .slider li:nth-child(2) label {
      left: 3.5em;
    }
    
    .slider li:nth-child(3) label {
      left: 6em;
    } 
    
    .slider li:nth-child(4) label {
      left: 8.5em;
    } 
    
    .slider li:nth-child(5) label {
      left: 11em;
    } 
    
    .slider li:nth-child(6) label {
      left: 13.5em;
    } 
    
    .slider li:nth-child(7) label {
      left: 16em;
    } 
  
    .slider li input:checked ~ label {
      width: 1.875em;
      height: 1.875em;
    }
    
  }
  
  /* Sobre */
  
  #sobre img {
    width: 20em;
    max-width: calc(100% - 4em);
    height: 20em;
    max-height: calc(100% - 4em);
    margin-left: 4em;
    padding: 0.65em;
    border-radius: 100%;
    border: solid 1px;
  }
  
  #sobre p {
    font-size: 1.2em;
    line-height: 1.8em;
    padding-top: 4em;
  }
  
  #sobre .sobre {
    display: flex;
  }
  
  #sobre .subtitulo {
    text-align: left;
    margin-bottom: 0;
  }
  
  #sobre .subtitulo:after {
    margin: 10px 0;
  }
  
  #sobre .call {
    text-align: left;
    padding-top: 0;
  }
  
  @media screen and (max-width: 480px) {
    #sobre .sobre {
      display: block;
    }
  
    #sobre img {
      width: 12em;
      height: 12em;
      margin: 1em auto;
    }
  
    #sobre p {
      font-size: .875em;
      padding-top: 1em;
    }
  
    #sobre .call {
      text-align: center;
      padding: 2em 0;
    }
  }
</style>

<script>
import BaseNav from '@/components/BaseNav';
import BaseHighlights from '@/components/highlights/BaseHighlights';

export default {
  name: 'HelloWorld',
  components: {
    BaseNav,
    BaseHighlights,
  },
  data () {
    return {
      navItemsArray: [
        { name: 'Item 1', link: '/link-1' },
        { name: 'Item 2', link: '/link-2' },
        { name: 'Item 3', link: '/link-3' },
        { name: 'item 4', link: '/link-4' },
      ],
      hightlightsArray: [
        { 
          name: 'Highlight 1',
          description: 'hightlight description 1',
          image: '@/assets/images/floriane-vita-88722-unsplash.jpg',
          imageDescription: 'description 1',
        },
        { 
          name: 'Highlight 2',
          description: 'highlight description 2',
          image: '@/assets/images/floriane-vita-88722-unsplash.jpg',
          imageDescription: 'Description 2',
        },
      ],
    };
  },
}
</script>
