## simplonilne.smooth_scroll

1- Tout d'abord j'ai telechargé une template sur internet[ce site est génial](http://www.opendesigns.org/website-templates/) et mon template est celui-ci](http://www.opendesigns.org/design/business-zonne/) à fin de ne pas crée une site moi-même car cela n'est pas le sujet.*(mais j'ai modifié un petit peu la page pour bien expliquer)*

2- Vous écrivez ces codes dans la balise<head> ou avant la fermetture de la balis **</body>**  ou vous écrivez dans un autre fichier.js en lui attachant à le fichier html avec cette commande
```javascript
<script src="nome de fichier.js" type="text/javascript"></script>
```
**les codes que en javascript que  vous devrez écrire** 
```javascript
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
<script>
	$(document).ready(function() {
		$('.scrollTo').click( function() { // Au clic sur un élément
			var page = $(this).attr('href'); // Page cible
			var speed = 750; // Durée de l'animation (en ms)
			$('html, body').animate( { scrollTop: $(page).offset().top }, speed ); // Go
			return false;
		});
	});
</script>
```
3-En suit sur chaque élémént qu'on veut le cliquer on ajout la **class="scrollTo"** en lui donnat un href qui est égal à **l'ID d'élement** où on veut y aller. par exmple j'ai utilisé pour la bar de navigation en cliquat sur chaque élement vous alez à l'endroit où se trouve cette élement. 

```html
  <li><a class="scrollTo" href="#Home">Home</a></li>
  <li><a class="scrollTo" href="#About">About Us</a></li>
  <li><a class="scrollTo" href="#Services">Services</a></li>
  <li><a class="scrollTo" href="#Products">Products</a></li>
  <li><a class="scrollTo" href="#Videos">Videos</a></li>
  
  <h2 id="Home">Home</h2>
  <p>...</p>
  
  <h2 id="About">Home</h2>
  <p>...</p>
  
  <h2 id="Services">Home</h2>
  <p>...</p>
  
  <h2 id="Products">Home</h2>
  <p>...</p>
  
  <h2 id="Videos">Home</h2>
  <p>...</p>
```

**en bas vous trouvez tout mon code en html  et je vous attache tous les autres fichiers sur mon guithub aussi**
```html
<!--  *********************************************** HTML***********************************************-->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
  <title>Design by YOURSITENAMEm</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
</head>

<body>
  <div class="style3">
  </div>
  <div class="style_2"><span class="style3"><a href="http://www.zonnebank-studio-vergelijk.nl" title="Zonnebank Zonnestudio"><strong>Zonnebank zonnestudio</strong></a></span>
  </div>
  <div id="wrap">
      <div id="topbar">
          <h1 id="sitename"><a href="http://www.zonnebank-studio-vergelijk.nl" target="_blank">  Zonnebank en zonnestudio</a></h1>
          <div id="menus">
              <ul id="topmenu">
                  <li class="active"><a class="scrollTo" href="#Home">Home</a></li>
                  <li><a class="scrollTo" href="#About">About Us</a></li>
                  <li><a class="scrollTo" href="#Services">Services</a></li>
                  <li><a class="scrollTo" href="#Products">Products</a></li>
                  <li><a class="scrollTo" href="#Videos">Videos</a></li>
              </ul>
          </div>
      </div>
      <div id="header">
      </div>
      <div id="content">
          <div id="mainpage">
              <h2 id="Home">Home</h2>
              <h2 id="Home">Home</h2>
              <p>Zonnebank en zonnestudios is a  "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum, Small   Businesses Website. After designing your site, we also submit  it major search engines and take due care to list them in relevant directories  and press releases.
        <br />
        <br />
"Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum,Domain name registration, Flash Animation,  Contact page with web form, Logo design, Web hosting services, Zonnebank en zonnestudios,  Traffic analysis and reporting, Navigation system creation etc. All these  services are available to you through , just login and  find out the miracles we have for you.</p>
              <h2 id="About">About Us</h2>
              <p>Zonnebank en zonnestudios is a  "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum, Small   Businesses Website. After designing your site, we also submit  it major search engines and take due care to list them in relevant directories  and press releases.
        <br />
        <br />
              <h2 id="Services">Services</h2>
              <p>Zonnebank en zonnestudios is a  "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum, Small   Businesses Website. After designing your site, we also submit  it major search engines and take due care to list them in relevant directories  and press releases.
        <br />
        <br />
"Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum,Domain name registration, Flash Animation,  Contact page with web form, Logo design, Web hosting services, Zonnebank en zonnestudios,  Traffic analysis and reporting, Navigation system creation etc. All these  services are available to you through , just login and  find out the miracles we have for you.</p>
              <h2 id="Products">Products</h2>
              <p>Zonnebank en zonnestudios is a  "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum, Small   Businesses Website. After designing your site, we also submit  it major search engines and take due care to list them in relevant directories  and press releases.
        <br />
        <br />
                <h2 id="Services">Services</h2>
              <p>Zonnebank en zonnestudios is a  "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum, Small   Businesses Website. After designing your site, we also submit  it major search engines and take due care to list them in relevant directories  and press releases.
        <br />
        <br />
"Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum,Domain name registration, Flash Animation,  Contact page with web form, Logo design, Web hosting services, Zonnebank en zonnestudios,  Traffic analysis and reporting, Navigation system creation etc. All these  services are available to you through , just login and  find out the miracles we have for you.</p>
              <h2 id="Products">Products</h2>
              <p>Zonnebank en zonnestudios is a  "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum, Small   Businesses Website. After designing your site, we also submit  it major search engines and take due care to list them in relevant directories  and press releases.
        <br />
        <br />
    "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum,Domain name registration, Flash Animation,  Contact page with web form, Logo design, Web hosting services, Zonnebank en zonnestudios,  Traffic analysis and reporting, Navigation system creation etc. All these  services are available to you through , just login and  find out the miracles we have for you.</p>
              <h2 id="Videos">Videos</h2>
              <p>Zonnebank en zonnestudios is a  "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum, Small   Businesses Website. After designing your site, we also submit  it major search engines and take due care to list them in relevant directories  and press releases.
        <br />
        <br />
"Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum,Domain name registration, Flash Animation,  Contact page with web form, Logo design, Web hosting services, Zonnebank en zonnestudios,  Traffic analysis and reporting, Navigation system creation etc. All these  services are available to you through , just login and  find out the miracles we have for you.</p>
  
          </div>
        </div>
          <div id="sidebar">
          </div>
          <div id="sidebarcontents"> 
              <ul id="menu">
                  <li><h2>Our Services</h2></li>
                  <li>
                      <ul>
                          <li><a href="#">Link a   Website</a></li>
                          <li><a href="#">Website Link B</a></li>
                          <li><a href="#">Website Link C</a></li>
                          <li> <a href="#">Small Businesses Website</a></li>
                          <li><a href="#">Flyer Website</a></li>
                      </ul>
                  </li>
              </ul>
          </div>
          <div id="sidebarbottom">
          </div>
      </div>
      <div class="clear">
      </div>
   </div>
  <div id="footer">
    <p>Copyright &copy; 2013 your sitename| <a href="#">Sitemap</a></p>
  </div>
</body>
</html>
```
