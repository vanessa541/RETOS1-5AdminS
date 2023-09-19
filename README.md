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
- ![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/adb2f640-38d3-4c16-a53c-15768f7d9925)

- cambiar el archivo a acarpeta systemd ![imagen](https://github.com/vanessa541/RETOS1-5AdminS/assets/111407329/7700b74e-3292-4b42-bda7-1c43cbd6f8d7)

 
