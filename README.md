# README

Ayudantia gem votable

1. gem 'acts_as_votable'

2. bundle install

3. rails generate acts_as_votable:migration

4. rails db:migrate

5. acts_as_votable

6. Prueba en consola opcional (

post = Post.first

post.liked_by User.first

post.voter_for.size

Post.downvote_by User.first. (para votos negativos)

post.voter_for.size)

7. vamos a implementar la funcionalidad con Ajax

   7.1 ir al controlador de post y crear nueva funcionalidad o método unvote para que los usuarios puedan votar a favor

   7.2 crear vista en posts vote.js.erb
   7.3 crear parcial upvote_link.html.erb

8. acts_as_voter (hacer que el usuario pueda votar)

9. en index de post crear el header de la tabla “voting” y su contenido render

10. generar ruta para upvote

11. ahora creamos funcionalidad para ver el conteo de votos

    11.1 agregamos columnas a la tabla post con almacenamiento de votos

12. Rails db:migrate

13. crear header en tabla mas contenido del conteo

14. crear parcial para el conteo \_votes score

15. representar el parcial en vote.js.erb

16. ordenar por cantidad de votos nuestras publicaciones
    .order(cached_votes_score: :desc)

17. crear votos negativos opcional
