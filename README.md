Usamos laravel 8 para construir la api
el metodo de seguridad que usamnos es sanctum
Permite registrarse, logearse y añadir un articulo al blog

Registrarse
http://localhost:8000/api/register  
{
    "name":"tu nombre",
    "email": "tucorreo@gmail.com",
    "password":"tu pass",
    "confirm_password":"tu pass"
}
Logearse
http://localhost:8000/api/login  
{
    
    "email": "tucorreo@gmail.com",
    "password":"tu pass",
    
}

Esto te dara un token que debes guardar para luego tener acceso 
en postman Authorization 
va Bearer Token y a la derecha pegas tu token ej 2|NUHKeUWnhty6BgfiEgs69RJVv3cnuQD

Listo ahora puedes ir a blogs
post: http://localhost:8000/api/blogs
{
  "title": "titulo del blog",
 "description": "Articulo del blog",
}




