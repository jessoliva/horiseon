# Challenge 1 - Code Refactor Starter Code

## Purpose

The purpose of this project was to review an existing code for a website for the client Horiseon and refactor it. The codebase had to follow accessibility standards, and be consolidated and efficient. 

## Built With
- HTML ![html percentage](https://img.shields.io/badge/html-49.9%25-9cf)
- CSS ![css percentage](https://img.shields.io/badge/css-50.1%25-ff69b4)

## Table of Contents

- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Website Link](#website-link)
- [Code Refactor](#code-refactor)
    - [HTML](#html)
    - [CSS](#css)
- [Credits](#credits)

## User Story

AS A marketing agency I WANT a codebase that follows accessibility standards SO THAT our own site is optimized for search engines.


## Acceptance Criteria

The following criteria for the codebase had to be met:

- GIVEN a webpage meets accessibility standards
- WHEN I view the source code
- THEN I find semantic HTML elements
- WHEN I view the structure of the HTML elements
- THEN I find that the elements follow a logical structure independent of styling and positioning
- WHEN I view the image elements
- THEN I find accessible alt attributes
- WHEN I view the heading attributes
- THEN they fall in sequential order
- WHEN I view the title element
- THEN I find a concise, descriptive title

## Website Link

[Horiseon](https://jessoliva.github.io/horiseon/)

## Code Refactor
### HTML
I made the following edits to the HTML code:

#### Within <head>
- changed <title>website</title> to <title>Horiseon</title>

#### Header Section
- changed &lt;div class="header"&gt; to <header>
- changed <div> to <nav>

#### Hero section
- changed <div> to <section>

#### Content section
- changed <div class="content"> to <section class="content">

#### Search Engine Optimization Section
- changed <div class="search-engine-optimization"> to <article id="search-engine-optimization">
    - changed <div> to <article>
    - removed class="search-engine-optimization"
    - added id="search-engine-optimization"
- changed <img src="./assets/images/search-engine-optimization.jpg" class="float-left" /> to <img src="./assets/images/search-engine-optimization.jpg" alt="notebook page displaying factors that affect search engine optimization" class="float-left" />
    - added alt=" " attribute

#### Online Reputation Section
- changed  <div id="online-reputation-management" class="online-reputation-management"> to <article id="online-reputation-management">
    - changed <div> to <article>
    - removed class="online-reputation-management"
- changed <img src="./assets/images/social-media-marketing.jpg" class="float-left" /> to  <img src="./assets/images/online-reputation-management.jpg" alt="laptop with presentation on screen showing slide displaying improving reputation"  class="float-right" />
    - added alt=" " attribute

#### Social Media Marketing Section
- changed <div id="social-media-marketing" class="social-media-marketing"> to <article id="social-media-marketing">
    - changed <div> to <article>
    - removed class="social-media-marketing"
- changed <img src="./assets/images/social-media-marketing.jpg" class="float-left" /> to <img src="./assets/images/social-media-marketing.jpg" alt="image displaying icons that represent factors that affect social media marketing" class="float-left" />
    - added alt=" " attribute

#### Benefits Section
- changed <div class="benefits"> to <section class="benefits">

#### Lead Generation Section
- changed <div class="benefit-lead"> to <div>
    - deleted class
- changed <img src="./assets/images/lead-generation.png" /> to <img src="./assets/images/brand-awareness.png" alt="" />
    - added alt="" attribute

#### Brand Awareness Section
- changed <div class="benefit-awareness"> to <div>
    - deleted class
- changed <img src="./assets/images/brand-awareness.png" /> to <img src="./assets/images/brand-awareness.png" alt="" />
    - added alt="" attribute

#### Cost Management Section
- changed <div class="benefit-cost"> to <div>
    - deleted class
- changed <img src="./assets/images/cost-management.png"></img> to <img src="./assets/images/cost-management.png" alt="" />
    - removed </img> and added />
    - added alt="" attribute

#### Footer Section
- changed <div> to <footer>
- changed <p>&copy; 2019 Horiseon Social Solution Services, Inc.</p> to &copy; 2019 Horiseon Social Solution Services, Inc.
    - removed <p>

### CSS
I made the following edits to the HTML code:

#### Body Styles
- deleted p {font-size: 16px;} and moved font-size: 16px to body { }

#### Header Styles

- header { } styles
    - changed .header { } to header { }
    - font-family: changed Arial and sans-serif to 'Arial' and 'sans-serif'
        - added ' '
- changed .header h1 { } to header h1 { }
- changed .header h1 seo { } to header h1 seo { }
- changed .header div { } to header nav { }
- changed .header div ul { } to header nav ul { }
- changed .header div ul li { } to header nav ul li { }
- changed a { } to header nav ul li a { }

#### Content Section Styles
- moved CONTECT SECTION STYLES before BENEFITS SECTION STYLES to follow semantic order
- .content article { }
    - deleted the following styles with classes and changed to .content article { }
    ![image 1](./assets/images/readme1-.contentarticle{}new.png) 
    - font-family: changed Calibri and sans-serif to 'Calrbri' and 'sans-serif'
        - added ' '
- deleted the following styles with classes and changed to .content img { }
    INSERT IMAGES
- deleted the following styles with classes and changed to .content h2 { }

#### Benefits Styles
- moved font-family from .benefits { } to .benefits div { }
- .benefits div { }
    - deleted the following styles with classes and changed to .benefits div { }
    INSERT IMAGES
    - font-family: changed Calibri and sans-serif to 'Calibri' and 'sans-serif'
        - added ' '
- deleted the following styles with classes and changed to .benefits div h3 { }
    INSERT IMAGES
- deleted the following styles with classes and changed to .benefits div img { }
    INSERT IMAGES

#### Footer Styles
- footer { }
    - changed .footer { } to footer { }
    - font-family: changed Arial and sans-serif to 'Arial' and 'sans-serif'
        - added ' '
- changed .footer h2 { } to footer h2 { }

## Credits
- Katherine Peterson - [readme.so](https://readme.so/)
- Kend Dodds - [badges](https://egghead.io/lessons/javascript-how-to-write-a-javascript-library-adding-badges-to-your-readme)
- [Shields.io](https://shields.io/)