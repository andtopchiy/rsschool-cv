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
jQuery(function($){
	$(document).mouseup(function (e){ // событие клика по веб-документу
		var div = $(".menu-wrap.menu-show, .mob-menu>.toggle-button, #menu"), // тут указываем ID элемента
			$menuWrap = $('.menu-wrap'),
			$toggleButtonMenu = $('.toggle-button');
		if (!div.is(e.target) // если клик был не по нашему блоку
			&& div.has(e.target).length === 0) { // и не по его дочерним элементам
			$menuWrap.removeClass('menu-show');
			$('.toggle-button.close-mob-btn').removeClass("showbtn");
			$toggleButtonMenu.removeClass('button-open');
		}
	});
});

$(document).ready(function() {
	var $searchBlock = $('#div_search'),
		$searchRow = $('#search-row');
	$searchBlock.on('click', function() {
		$($searchRow).addClass('hover-search');
	});
	$(".phone-mobhead-btn img, .xs-menu-hidden .arr-grey").on('click', function() {
		$('.xs-menu-hidden').slideToggle(360).toggleClass('on-phone-mob');
	});
	$(".search-mobhead-btn img, .close-search img").on('click', function() {
		$('.search-mob-head').toggleClass('search-on');
		$('.search-mob-head #search-header').focus();
	});
});

jQuery(function($){
	$(document).mouseup(function (e){
		var div = $("#div_search"),
			$searchRow = $('#search-row');

		if (!div.is(e.target)
			&& div.has(e.target).length === 0) {
			$searchRow.removeClass('hover-search');
		}

	});
});
$(document).ready(function() {
	$('.option .input label').html(function(_, oldHtml) { return oldHtml.replace(/:/g, ''); });
});
$(document).ready(function() {
	$('.seotext').click(function() {
		$('.opentext').addClass('act');
	});
});

$(function() {
	$(".opentext").click(function(e) {
		$('.seotext').toggleClass('active');
	});
	$("#on-filter-category, .close-filtr, .show-all-filtrmob").click(function(e) {
		$('#main_content').toggleClass('active');
		$('#sortir-panel').toggleClass('active');
	});

/*sorting-category*/
	if($("span").is(".actv.dwntoup")){
		$(".actv").parent(".active-sort").addClass('acv-sort');

	}

	if($("span").is(".actv.uptodwn")){
		$(".actv").parent(".active-sort").addClass('acv-sort');
	}

	if($("span").is(".actv.uptodwn")){

		$('.sort-btn').on('click', function (e) {
			var link = $(".actv.uptodwn").parent(".active-sort.acv-sort")[0];
			var linkEvent = document.createEvent('MouseEvents');
			linkEvent.initEvent('click', true, true);
			link.dispatchEvent(linkEvent);
			e.preventDefault();
		});
	} else if($("span").is(".actv.dwntoup")){
		$('.sort-btn').on('click', function (e) {
			var link = $(".actv.dwntoup").parent(".active-sort.acv-sort")[0];
			var linkEvent = document.createEvent('MouseEvents');
			linkEvent.initEvent('click', true, true);
			link.dispatchEvent(linkEvent);
			e.preventDefault();
		});
	} else {
		$('.sort-btn').on('click', function (e) {
			var link = $('.sort-price-lnk a')[0];
			var linkEvent = document.createEvent('MouseEvents');
			linkEvent.initEvent('click', true, true);
			link.dispatchEvent(linkEvent);
			e.preventDefault();
		});
	}

	if($("span").is(".dwntoup")){
		$('.sort-btn').addClass('rotate-img');
	}
});
``` 


#### Working Experience
Working about 7 years on freelance Here link on my profile on ukrainian freelance freelance exchange https://freelancehunt.com/freelancer/Andrux.html

####Education
* Admiral Makarov National University of Shipbuilding (Computer science)
* Open International University of Human Development “Ukraine” (Law)
* Computer Training Center “Specialist” (html, css. js)