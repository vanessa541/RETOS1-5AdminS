# RETOS1-5AdminS
## 0 Reto cambio de inicio por defecto:
- Descripción: Verifica cual es el modo en que inicia tu Linux por defecto, cambia el modo y
comprueba el cambio. Deja por defecto el modo que prefieras.
- Objetivo: Aprender a cambiar el modo por defecto en SystemD.
  
  me encuntro en modo gráfico 
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/339ff5dd-addb-4561-8d3b-41185c5a264e)



pasare al mod multi-user
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/7d70918a-b6ff-4630-8376-09234f854065)


al reiniciar entra al modo multi user sin interfaz gráfica
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/6d1f017f-7278-4c79-b5f6-d0e9cf2034ff)


volver al modo gráfico 

sudo systemctl set-default graphical.target 

![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/d516a572-b80e-4f3f-b6b3-fca011779940)

# 1 Reto del Servidor Web Personalizado:
- Descripción: Crea un servicio para el servidor web instalado desde código fuente.
- Objetivo: Aprender a configurar servicios personalizados en ubicaciones no estándar.

- archivo miapache.service
- ![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/a625a033-3704-4666-b96f-6dd30fa82768)


- cambiar el archivo a acarpeta systemd ![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/7700b74e-3292-4b42-bda7-1c43cbd6f8d7)

- ![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/264dd8a9-0e05-4e95-8d94-7f13c48b7898)

Habilita el servicio para que se inicie en el arranque:

![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/c6cd3242-522b-49f6-90cd-6946b254cf67)


verificacion del status

![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/6f006a2c-ea2f-4aef-8169-aa8aa650ac6f)



 # Reto 2 temporizador

 script para archivo 
 ![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/56f1fb58-aa59-42f2-99cd-18b6ce808ee5)
 
ejecucion manual de script 
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/206ed1cf-962a-4f17-935e-f2041a521d43)

comprobacion de la creacion del archivo

![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/5c7414b8-d0b1-455d-91fd-3d8bacaf2420)

creación de mi-log.service, servicio para ejecutar el script milog.sh
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/f55ed2b8-1301-4547-b2ad-068c5c64d1ff)

crwacion de archivo mi-log.timer, para ejecutar el servicio cada 5min
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/000afbd9-fc80-432f-8da3-51a0845ef0f4)



despues de realizar estos archivos .service y .timer , iniciarlos

![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/9f92bb57-df01-4d48-a0f2-f61c9cc47f73)

![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/d3a2ca8c-09e7-4c16-a2e1-438696f44562)

en el archivo /var/log/mi-log.log comprobamos si el servicio corre cada 5minutos
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/ba858995-a809-43d6-b607-ce355af4a4b8)

# Reto dependencias
servicio apache corriendo 
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/29e1b3b9-3389-45de-8141-f36fc9ca009d)

servicio B corriendo 
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/ca2e694d-4081-4b9b-a569-3e6102dd0a73)


se detiene el servicio apache 
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/e2abb6b9-5d8f-430a-aa47-782687ac4139)


iniciamos nuevamente el sercio B y ya no corre
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/ef6ba1ac-930c-4a15-9072-4cfd19f5f068)

ultima ejecucion
![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/7c21fc20-f0d8-4c47-9e77-08ccf4984470)

![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/dbb3480b-930c-47b7-aeba-4b76d844bc3a)

