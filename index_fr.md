<div class="teasing-part">                                                                      

  <div class="home-logo">
    <img src="/images/ynh_logo_white_300dpi.png" width="100"/>
  </div>

  <div class="punchline">
    <p>
      <span class="yolo 1" style="color: #FF3399;">Viens chez moi, je suis hébergé chez une copine</span>
      <span class="yolo 2" style="color: #FF0066;">Ils s’hébergèrent et eurent beaucoup d’enfants</span>
      <span class="yolo 3" style="color: #3366FF;">Internet, lecture et écriture</span>
      <span class="yolo 4" style="color: #FFFFFF;">monsieur@michu.fr</span>
      <span class="yolo 5" style="color: #CC66FF;">J’ai rien à cacher</span>
      <span class="yolo 6" style="color: #FF6600;">How I met your server</span>
    </p>
    <button class="btn btn-primary btn-lg btn-block yolobtn">Pardon ?</button>
  </div>

  <div class="main-links hidden-xs">
    <a href="/whatsyunohost_fr">À propos</a> <span class="colored-bar">•</span> 
    <a href="https://forum.yunohost.org/c/announcement" target="_blank">Dernières nouvelles</a> <span class="colored-bar">•</span> 
    <a href="/docs_fr">Documentation</a> <span class="colored-bar">•</span> 
    <a href="https://donate.yunohost.org/">Faire un don</a>
  </div>

</div><!-- teasing-part -->

<div class="boring-part" markdown="1">

  <h1><small>Avec</small> YunoHost<small>, gères facilement un serveur pour tes amis, ton asso, ton entreprise.</small> <a href="/whatsyunohost" style="font-size:0.6em;">En savoir plus</a></small></h1>

  <div class="home-panel">
    <img src="/images/home_panel.jpg" />
  </div>

  <div class="call-to-action">
    <a class="btn btn-primary btn-lg" href="/try_fr">Essayer</a>
    <a class="btn btn-success btn-lg" href="/install_fr">Installer</a>
    <h2 style="margin-top: 0"><small><a href="https://forum.yunohost.org/c/announcement">Dernières nouvelles</a></small></h2>
  </div>

  <hr />

  <div class="row cf">
    <div class="col-md-7 text-right">
      <h1>Installez <small>votre serveur simplement, vous avez déjà tout ce qu’il faut à la maison</small></h1>
      <p><a href="/hardware_fr">Voir les prérequis</a></p>
    </div>
    <div class="col-md-4">
      <div class="feature-pic">
        <img src="/images/home_install.png" />
      </div>
    </div>
  </div>

  <hr />

  <div class="row cf">
    <div class="col-md-4">
      <div class="feature-pic">
        <img src="/images/webadmin_fr.png" />
      </div>
    </div>
    <div class="col-md-7">
      <h1>Gérez <small>votre serveur depuis une interface web simple et propre</small></h1>
      <p><br /><a href="/try_fr">Essayez l’interface d’administration</a></p>
    </div>
  </div>

  <hr />

  <div class="row cf">
    <div class="col-md-7 text-right">
      <h1>Construisez <small>votre petit bout d'Internet en ajoutant des applications en quelques clics</small></h1>
      <p><br /><a href="/apps">Parcourir les applications disponibles</a></p>
    </div>
    <div class="col-md-4">
      <div class="feature-pic">
        <img src="/images/home_enjoy.jpg" />
      </div>
    </div>
  </div>

  <hr />

  <div class="row cf">
    <div class="text-center">
    <h1>Hey ! Nous sommes humains !<br />
    <small>Si vous avez une question, un problème, ou que vous êtes tout simplement intéressé, passez dire « Bonjour » sur notre forum ou le chat!</small></h1>

    <div class="col-md-4 col-md-offset-4 button-list">
      <a class="btn btn-lg btn-block btn-info" href="/docs"><span class="glyphicon glyphicon-book"></span> Documentation</a>
      <a class="btn btn-lg btn-block btn-danger btn-support" href="/help_fr"><span class="glyphicon glyphicon-comment"></span> Forum et chat</a>
      <a class="btn btn-lg btn-block btn-success" href="/contribute"><span class="glyphicon glyphicon-heart"></span> Contribuer</a>
      <a class="btn btn-lg btn-block btn-primary" href="https://donate.yunohost.org/" style="background-color: #ffd236; border-color: #ffd236;"><span class="glyphicon glyphicon-usd"></span> Faire un don</a>
     </div>
  </div>

</div><!-- boring-part -->

<script type="text/javascript">
    jQuery('.teasing-part').css({
        marginTop: '0',
        display: 'block'
    });
    jQuery('.boring-part').css({
        marginTop: jQuery(window).height() + 100
    });
    jQuery( window ).resize(function() {
        jQuery('.boring-part').css({
            marginTop: jQuery('.teasing-part').height() + 100
        });
    });
    jQuery('.yolo').hide();
    randomNumber = Math.floor((Math.random()*jQuery('.yolo').length)+1);
    color = jQuery('.yolo.' + randomNumber).css('color');
    jQuery('.yolo.' + randomNumber).fadeIn();
    document.title = jQuery('.yolo.' + randomNumber).text();
    jQuery('.colored-bar').css({
      color: color,
      fontWeight: 'bold',
      padding: '1%'
    });
    jQuery('.yolobtn').css({
      background: color,
      borderColor: color
    }).on('click', function() {
      jQuery('html, body').animate({
        scrollTop: jQuery(window).height() + 80
      }, 500);
    });

</script>

