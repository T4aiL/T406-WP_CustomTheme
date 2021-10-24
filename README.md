# T406 - HTML/CSS/JS - powtórzenie
## -------INFO

1. Layout strony (Figma)
2. CSS - selektory
3. CSS - Pozycjonowanie elementów
4. Animacje

#### Custom template

1. Minimal files

* style.css (
/*
Template Name: My theme
*/
* index.php

2. Typical files

* comments.php
* comments-popup.php
* footer.php
* header.php
* sidebar.php

3. Includes

* get_header().
* get_sidebar().
* get_footer().
* get_search_form().

4. Inserts

* the_title();
* the_time();
* the_category();
* the_author();
* the_permalink();

5. Loop
```php
<?php 
if ( have_posts() ) {
	while ( have_posts() ) {
		the_post(); 
		//
		// Post Content here
		//
	} end while
} end if
?>
```

6. theme_support
```php
function sro_theme_support(){
    add_theme_support( 'custom-logo' );
    add_theme_support( 'custom-background' );
    add_theme_support( 'custom-header' );  
    add_theme_support( 'menus' );  
}
```
6. enqueue
```php
function wpdocs_theme_name_scripts() {
    wp_enqueue_style( 'style-name', get_stylesheet_uri() );
    wp_enqueue_script( 'script-name', get_template_directory_uri() . '/js/example.js', array(), '1.0.0', true );
}
add_action( 'wp_enqueue_scripts', 'wpdocs_theme_name_scripts' );
```

### --------ZAD
``` 
T40501 - Przygotuj projekt strony w Figma

T40502 - Przygotuj stronę WWW przeznaczoną do konwersji na szablon Wordpressa. 
Przygotuj co najmniej trzy strony statyczne (Home, O nas, Blog).
Na Home umieść Menu w Header, Footer z sekcją ikon social mediów,
oraz listę najnowszych wpisów, a także sekcję testimonials zbudowaną 
z trzech kart wyposażonych w zdjęcie użytkownika.
Maksymalna ocena wymaga slidera wyposażonego w strzałki nawigacji oraz autoodtwarzanie pokazującego najnowsze wpisy.
```
### --------Links
https://github.com/T4aiL/T406-CSS-recap

Layout inspirations: https://drive.google.com/drive/folders/13lyoR2wH2LrDdUcLWojNBxd6DyDRQ_e_

GOOGLE DRIVE: https://drive.google.com/drive/folders/1FCn1K3AvZdta3JRNnfCFUlSqAyMWgxNe?usp=sharing

### --------Tutorials
[Real Glassmorphism Card Hover Effects | Html CSS Glass morphism Effects](https://youtu.be/hv0rNxr1XXk)

[Build Glass Website with HTML and CSS Tutorial](https://youtu.be/O7WbVj5apxU)

### --------Info
https://www.w3.org | https://validator.w3.org | https://www.php.net/manual/en/
### --------Repositiories
https://www.w3schools.com | https://stackoverflow.com | https://css-tricks.com |
### --------On line editors
https://codepen.io/ | https://codesandbox.io/ | https://jsfiddle.net/ |
### ---------Assets
https://cdnjs.com/ | https://fontawesome.com | http://fontello.com/ | https://fonts.google.com/ |
### ---------Placeholders
https://pl.lipsum.com/ | https://logoipsum.com/ | https://placeholder.com/
### ---------Stock Img
https://www.pexels.com/ | https://unsplash.com | https://pixabay.com
### ---------Tuts
JavaScript ES6 Modules : https://youtu.be/cRHQNNcYf6s

[Tutorial WordPress – od szablonu HTML do dynamicznego motywu WP)[https://wpadmin.pl/tutorial-wordpress-od-szablonu-html-do-dynamicznego-motywu](https://wpadmin.pl/tutorial-wordpress-od-szablonu-html-do-dynamicznego-motywu-wp/#:~:text=Tutorial%20WordPress%20%E2%80%93%20od%20szablonu%20HTML%20do%20dynamicznego,Loop%20%E2%80%93%20p%C4%99tla%20wy%C5%9Bwietlaj%C4%85ca%20wpisy%20w%20WP.%20)
### ---------License
[MIT](https://choosealicense.com/licenses/mit/)
