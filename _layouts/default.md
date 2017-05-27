<!DOCTYPE html>
  <html>
    <head>
      <title>{{ page.title }}</title>
      <!-- link to main stylesheet -->
      <link rel="stylesheet" type="text/css" href="/css/main.css">
    </head>
    <body>
      <nav>
          <ul>
              <li><a href="/">Home</a></li>
              <li><a href="/about">About</a></li>
              <li><a href="/codes">Code</a></li>
              <li><a href="/resume">Resume</a></li>
              <li><a href="/revision">Revision</a></li>
          </ul>
      </nav>
      <div class="container">
      {{ content }}
      </div><!-- /.container -->
      <footer>
          <ul>
              <li><a href="mailto:jlenriquez@gmail.com">email</a></li>
              <li><a href="https://github.com/jlenriquez">github.com/jlenriquez</a></li>
        </ul>
      </footer>
    </body>
  </html>