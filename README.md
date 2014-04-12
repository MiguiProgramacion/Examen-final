Examen-final
============
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>2048DBZ</title>

  <link href="style/main.css" rel="stylesheet" type="text/css">
  <link rel="shortcut icon" href="favicon.ico">
  <link rel="apple-touch-icon" href="meta/apple-touch-icon.png">
  <meta name="apple-mobile-web-app-capable" content="yes">

  <meta name="HandheldFriendly" content="True">
  <meta name="MobileOptimized" content="320">
  <meta name="viewport" content="width=device-width, target-densitydpi=160dpi, initial-scale=1.0, maximum-scale=1, user-scalable=no, minimal-ui">

  <meta property="og:title" content="Versión DBZ del juego 2048"/>
  <meta property="og:site_name" content="Versión DBZ del juego 2048"/>
  <meta property="og:description" content="¡Uní los Goku's del mismo nivel para levelearlo hasta SSJ4! Cuidado: ¡el juego es **MUY** adictivo!"/>
  <meta property="og:image" content="http://mgarciaisaia.github.io/2048dbz/meta/og_image.png"/>
</head>
<body>
  <div id="fb-root"></div>
  <div class="container">
    <div class="header">
      <div class="heading">
        <h1 class="title">2048DBZ</h1>
        <div class="scores-container">
          <div class="score-container">0</div>
          <div class="best-container">0</div>
        </div>
      </div>
      <p class="game-intro">Uní los Goku's del mismo nivel para levelearlo hasta <strong>¡SSJ4!</strong></p>
    </div>

    <div class="game-container">
      <div id="vegeta-scouter">
        <img src="img/scouter.png" >
        <div id="scouter-deco"><div id="scouter-deco-arrow-left" class="blink">◀</div><div id="scouter-deco-arrow-right" class="blink">▶</div><div id="scouter-deco-arrow-down" class="blink">▼</div><div id="scouter-deco-circle">○</div></div>
        <div id="scouter-score">0</div>
      </div>
      <div class="game-message">
        <p></p>
        <div class="lower">
          <a class="keep-playing-button">Seguir jugando</a>
          <a class="retry-button">Reintentar</a><br />
          <div class="sharing">
            <iframe src="http://ghbtns.com/github-btn.html?user=mgarciaisaia&repo=2048dbz&type=watch&count=true"
              allowtransparency="true" frameborder="0" scrolling="0" width="75" height="20"></iframe>
            <div class="fb-share-button" data-href="http://git.io/2048dbz" data-type="button_count"></div>
            <div class="score-sharing"></div>
          </div>
        </div>
      </div>

      <div class="grid-container">
        <div class="grid-row">
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
        </div>
        <div class="grid-row">
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
        </div>
        <div class="grid-row">
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
        </div>
        <div class="grid-row">
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
          <div class="grid-cell"></div>
        </div>
      </div>

      <div class="tile-container">

      </div>
    </div>

    <p class="game-explanation">
      <strong class="important">Cómo jugar:</strong> Usá <strong>las flechas</strong> (o el teclado táctil de tu teléfono) para mover las celdas. Cuando dos celdas con la misma fase de Goku chocan, se <strong>¡unen en una fase más poderosa!</strong>
    </p>
    <hr>
    <p>
    Modificado por <a href="http://github.com/dggluz" target="_blank">Gonzalo Gluzman</a>, con el trabajo de mono hecho por <a href="http://github.com/mgarciaisaia">Matias Garcia Isaia</a>. Basado en <a href="http://git.io/2048" target="_blank">2048, de Gabriele Cirulli</a>, por idea de Mariano Salerno, Pablo de Haro, Claudio Fernandez, Manu Gambino, y nosotros mismos.
    </p>
    <div class="sharing">
      <iframe src="http://ghbtns.com/github-btn.html?user=mgarciaisaia&repo=2048dbz&type=watch&count=true"
  allowtransparency="true" frameborder="0" scrolling="0" width="75" height="20"></iframe>
      <div class="fb-share-button" data-href="http://git.io/2048dbz" data-type="button_count"></div>
      <a href="https://twitter.com/share" class="twitter-share-button" data-text="Mirá 2048DBZ, un juego en que unís Goku's para subirlos de nivel! #2048dbz #dbz #2048game" data-url="http://git.io/2048dbz" data-counturl="http://git.io/2048dbz">Tweet</a>
      <script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+'://platform.twitter.com/widgets.js';fjs.parentNode.insertBefore(js,fjs);}}(document, 'script', 'twitter-wjs');</script>
    </div>
  </div>
  <script>(function(d, s, id) {
    var js, fjs = d.getElementsByTagName(s)[0];
    if (d.getElementById(id)) return;
    js = d.createElement(s); js.id = id;
    js.src = "//connect.facebook.net/es_ES/all.js#xfbml=1";
    fjs.parentNode.insertBefore(js, fjs);
  }(document, 'script', 'facebook-jssdk'));</script>

  <script src="js/classlist_polyfill.js"></script>
  <script src="js/animframe_polyfill.js"></script>
  <script src="js/keyboard_input_manager.js"></script>
  <script src="js/html_actuator.js"></script>
  <script src="js/grid.js"></script>
  <script src="js/tile.js"></script>
  <script src="js/local_score_manager.js"></script>
  <script src="js/game_manager.js"></script>
  <script src="js/application.js"></script>

</body>
</html>
