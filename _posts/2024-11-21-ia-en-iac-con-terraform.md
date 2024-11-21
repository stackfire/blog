<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Stackfire Blog</title>
</head>
<body>
  <h1>Blog de Stackfire</h1>
  <ul>
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> - <span>{{ post.date | date: "%d de %B de %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</body>
</html>
