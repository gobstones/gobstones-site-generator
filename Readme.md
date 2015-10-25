# Uqbar Site Generator

## Requires:
 - [NodeJS](https://nodejs.org/)
 - [HarpJS](http://harpjs.com/) `npm install -g harp`

## Cómo agregar contenido
El html se genera a partir de templates [Jade](http://jade-lang.com/), y se utiliza [Stylus](https://learnboost.github.io/stylus/) para los estilos. Los archivos .md con markdown generan html, con lo cual el contenido de posts, descripciones, etc., pueden escribirse en Markdown.
A su vez, los archivos json sirven para guardar información, que puede ser accedida desde los templates.
Para una explicación más completa ver la [documentación de HarpJS](http://harpjs.com/docs/development/layout)

## Local Server

 En el directorio raiz
 - `harp server`       levanta un server local

## Deploy:

### Travis CI
 
 Todo lo que se suba a `master` va a ser buildeado por Travis-CI y pusheado a https://github.com/gobstones/gobstones.github.io
 El sitio estático quedará servido en http://gobstones.github.io
 
### Manual
 
 También puede usarse directamente `deploy.sh` ,  siempre y cuando se agregue al entorno la variable `GITHUB_TOKEN` con el correspondiente token de acceso.

