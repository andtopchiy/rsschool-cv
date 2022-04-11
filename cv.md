# Andrii Topchii
### Contacts
* E-mail: and.topchiy@gmail.com

* Phonenumber: +380633036206

## Objective
### Skills
##### Computer skills:
* html,css
* basic knowledge of php
* basic knowledge of js
* skills work whith Adobe Photoshop, Figma
* Have skills on Joomla, Wordpress, Opencart

#### Language skills:
* Russsian
* Ukrainian
* English А2


#### Example of latest code:
 For now I am working with Opencart, make layout and integration of layout on the site.

``` 
import i18Obj from './translate.js';

const hamburger = document.querySelector('.hamburger');
const menuMob = document.querySelector('.nav');
const navLinks = document.querySelectorAll('.nav-link');

const portfolioImages = document.querySelectorAll('.photo-item-img');
const portfolioBtns = document.querySelectorAll('.btn-black_gold');
const seasons = ['winter', 'spring', 'summer', 'autumn'];

if (2 % 2 == 0) {
  console.log('true');
}
else {
  console.log('false');
}

// mob-menu
const toggleMenu = () => {
  hamburger.classList.toggle('actv');
  menuMob.classList.toggle('actv');
};
hamburger.addEventListener('click', toggleMenu);

const closeMenu = (event) => {
  if (event.target.classList.contains('nav-link')) {
    hamburger.classList.remove('actv');
    menuMob.classList.remove('actv');
  }
};

navLinks.forEach((el) => el.addEventListener('click', closeMenu));


document.addEventListener('DOMContentLoaded', () => {
  window.addEventListener('click', e => {
    const target = e.target;
    if (!target.closest('.nav') && !target.closest('.hamburger')) {
      hamburger.classList.remove('actv');
      menuMob.classList.remove('actv');
    }
  });
});

//slider
const changeImage = (event) => {
  portfolioBtns.forEach((el) => el.classList.remove('actv'));
  event.target.classList.add("actv");
  if (event.target.classList.contains('btn-black_gold')) {
    console.log(event.currentTarget.dataset.season);
    portfolioImages.forEach((img, index) => img.src = `./assets/img/${event.currentTarget.dataset.season}/${index + 1}.jpg`);
  }
};
portfolioBtns.forEach((el) => el.addEventListener('click', changeImage));

//slider-cashe
function preloadSummerImages() {
  seasons.forEach(folder => {
    for (let i = 1; i <= 6; i++) {
      const img = new Image();
      img.src = `./assets/img/${folder}/${i}.jpg`;
    }
  });
}
preloadSummerImages();
``` 


#### Working Experience
Working about 9 years on freelance Here link on my profile on ukrainian freelance freelance exchange https://freelancehunt.com/freelancer/Andrux.html

####Education
* Admiral Makarov National University of Shipbuilding (Computer science)
* Open International University of Human Development “Ukraine” (Law)
* Computer Training Center “Specialist” (html, css. js)
