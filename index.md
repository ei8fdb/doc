<div class="teasing-part">                                                                      

  <div class="home-logo">
    <img src="/images/ynh_logo_white_300dpi.png" width="100"/>
  </div>

  <div class="punchline">
    <p>
      <span class="yolo 1" style="color: #6699FF;">Haters gonna host</span>
      <span class="yolo 2" style="color: #66FF33;">I host myself, Yo!</span>
      <span class="yolo 3" style="color: #00FFCC;">Go host yourself!</span>
      <span class="yolo 4" style="color: #FF5050;">Get off of my cloud</span>
      <span class="yolo 5" style="color: #FF0066;">Host me I’m famous</span>
      <span class="yolo 6" style="color: #3366FF;">Try Internet</span>
      <span class="yolo 7" style="color: #FFFFFF;">How I met your server</span>
      <span class="yolo 8" style="color: #FF6600;">john@doe.org</span>
      <span class="yolo 9" style="color: #FF5050;">dude, Y U NO Host?!</span>
      <span class="yolo 10" style="color: #66FF33;">Keep calm and host yourself</span>
    </p>
    <button class="btn btn-primary btn-lg btn-block yolobtn">What?</button>
  </div>

  <div class="main-links hidden-xs">
    <a href="/whatsyunohost">About</a> <span class="colored-bar">•</span> 
    <a href="https://forum.yunohost.org/c/announcement" target="_blank">Latest news</a> <span class="colored-bar">•</span> 
    <a href="/docs">Documentation</a> <span class="colored-bar">•</span> 
    <a href="https://donate.yunohost.org/">Donate</a>
  </div>

</div><!-- teasing-part -->

<div class="boring-part" markdown="1">

  <h1><small>With</small> YunoHost<small>, you can easily manage a server for your friends, association or enterprise.</small> <a href="/whatsyunohost" style="font-size:0.6em;">Learn more</a></small></h1>

  <div class="home-panel">
    <img src="/images/home_panel.jpg" />
  </div>

  <div class="call-to-action">
    <a class="btn btn-primary btn-lg" href="/try">Try it</a>
    <a class="btn btn-success btn-lg" href="/install">Get started</a>
    <h2 style="margin-top: 0"><small><a href="https://forum.yunohost.org/c/announcement">Latest news</a></small></h2>
  </div>


  <div class="row cf">
    <div class="col-md-7 text-right">
      <h1>Setup <small>your server with ease, you already have everything at home</small></h1>
      <p><br /><a href="/hardware">See the requirements</a></p>
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
        <img src="/images/webadmin.png" />
      </div>
    </div>
    <div class="col-md-7">
      <h1>Manage <small>your server from a clean and simple web interface</small></h1>
      <p><br /><a href="/try">Try the administration</a></p>
    </div>
  </div>

  <hr />

  <div class="row cf">
    <div class="col-md-7 text-right">
      <h1>Install <small>applications to build your little corner of Internet</small></h1>
      <p><br /><a href="/apps">Browse available apps</a></p>
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
    <h1>Hey! We are humans!<br />
    <small>If you have questions, issues or if you are just an enthusiast, come and leave a message on our forum or chatroom!</small></h1>

    <div class="col-md-4 col-md-offset-4 button-list">
      <a class="btn btn-lg btn-block btn-info" href="/docs"><span class="glyphicon glyphicon-book"></span> Documentation</a>
      <a class="btn btn-lg btn-block btn-danger btn-support" href="/help_fr"><span class="glyphicon glyphicon-comment"></span> Forum and chat</a>
      <a class="btn btn-lg btn-block btn-success" href="/contribute"><span class="glyphicon glyphicon-heart"></span> Get involved</a>
      <a class="btn btn-lg btn-block btn-primary" href="https://donate.yunohost.org/" style="background-color: #ffd236; border-color: #ffd236;"><span class="glyphicon glyphicon-usd"></span> Donate</a>
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
