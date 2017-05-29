<!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8">
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <meta name="viewport" content="width=device-width, initial-scale=1">
      <meta name="description" content="Personal website of Joel Legaspi Enriquez">
      <meta name="author" content="Joel Legaspi Enriquez">
      <link rel="icon" href="../../favicon.ico">
      <title>{{ page.title }}</title>
      <!-- Bootstrap -->
      <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
      <!-- Google Fonts -->
      <link href='https://fonts.googleapis.com/css?family=Raleway:400,300' rel='stylesheet' type='text/css'>
      <!-- Custom styles for this template -->
      <link href="{{ page.css_dir }}font.css" rel="stylesheet">
      <link href="{{ page.css_dir }}pastie.css" rel="stylesheet">
      <link href="{{ page.css_dir }}sticky-footer.css" rel="stylesheet">
    <body>
    <nav class="navbar navbar-default">
      <div class="container-fluid">
        <!-- Brand and toggle get grouped for better mobile display -->
        <div class="navbar-header">
          <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          <a class="navbar-brand" href="#">Joel Enriquez</a>
        </div>
        <!-- Collect the nav links, forms, and other content for toggling -->
        <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
          <ul class="nav navbar-nav">
            <li class="{{ page.active1 }}"><a href="/">Home <span class="sr-only">(current)</span></a></li>
            <li class="{{ page.active2 }}"><a href="/about">About</a></li>
            <li class="{{ page.active3 }}"><a href="/resume">Resume</a></li>
            <li class="{{ page.active4 }}"><a href="/codes">Code</a></li>
            <li class="{{ page.active5 }}"><a href="/revision">Revision</a></li>
          </ul>
          <form class="navbar-form navbar-left">
            <div class="form-group">
              <input type="text" class="form-control" placeholder="Search">
            </div>
            <button type="submit" class="btn btn-default">Submit</button>
          </form>
          <ul class="nav navbar-nav navbar-right">
            <li class="dropdown">
              <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Connect <span class="caret"></span></a>
              <ul class="dropdown-menu">
                <li><a href="#">Facebook</a></li>
                <li><a href="#">Github</a></li>
                <li><a href="#">HackerRank</a></li>
                <li><a href="#">LinkedIn</a></li>
                <li><a href="#">StackOverflow</a></li>
                <li role="separator" class="divider"></li>
                <li><a href="#">Send me an email...</a></li>
              </ul>
            </li>
          </ul>
        </div><!-- /.navbar-collapse -->
      </div><!-- /.container-fluid -->
    </nav>
      <div class="container">
      <p>{{ content }}</p>
      </div><!-- /.container -->
      <footer class="footer">
        <div class="container">
          <p class="text-muted">Copyright (C) 2017. Joel Enriquez. Developer of stuff.</p>
        </div>
      </footer>
      <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
      <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
      <!-- JS -->
      <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
    </body>
  </html>
