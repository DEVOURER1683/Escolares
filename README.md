# Escolares DockerLabs

1. Escaneo de puertos con Nmap
   
   ![1  Nmap](https://github.com/DEVOURER1683/Escolares/assets/84418941/cf099a77-ebe1-4e6c-ab19-8e19ab98afad)


2. Análisis del codigo fuente de la pagina web

  ![2  Source Code](https://github.com/DEVOURER1683/Escolares/assets/84418941/5ab8a007-cd4d-401f-b50d-415d79b017bb)

Se encuentran 6 usuarios en la ruta

  ![2 1  Usuarios](https://github.com/DEVOURER1683/Escolares/assets/84418941/924acd1c-09e5-4aaf-a7ad-2e3ae875af14)

Se observa que el usuario Luis es admin de WordPress

3. Enumeración con Gobuster

  ![3  Gobuster](https://github.com/DEVOURER1683/Escolares/assets/84418941/753426a9-348f-4cd6-885c-7baec9ce2190)

Tenemos un WordPress y un usuario admin de WordPress

4. Creación de diccionario con los datos que aparecen del usuario de Luis

  ![4  Cupp](https://github.com/DEVOURER1683/Escolares/assets/84418941/258eddb3-4a13-48a2-9092-e7ddb27e79ff)

5. Ataque de diccionario con wpscan al usuario luisillo

  ![5  wpscan](https://github.com/DEVOURER1683/Escolares/assets/84418941/f31a085f-456d-4781-a59e-5e5c185499d1)

6. Se accede al WordPress, se crea una reverse shell para cargarla como plugin y obtener el acceso a la maquina

  ![6  Reverse Shell](https://github.com/DEVOURER1683/Escolares/assets/84418941/9d1c43fa-d2a4-4801-9cf7-2b48ed5a14ef)

7. Se carga el archivo .zip como plugin, se pone el puerto a la escucha con NetCat y se activa el plugin

  ![7  Caparazón](https://github.com/DEVOURER1683/Escolares/assets/84418941/fac55cb6-62f9-47b3-adbd-d63e1748ec7e)

8. Se encuentra un archivo con la contraseña del usuario luisillo y se ingresa como luisillo

  ![8  Escalado de Privilegios](https://github.com/DEVOURER1683/Escolares/assets/84418941/3e979602-67cb-46b5-a58d-b683775267bc)

9. Se lista los binarios con permisos SUID

  ![9  Binarios](https://github.com/DEVOURER1683/Escolares/assets/84418941/557aa53c-e539-4cf3-95b5-5643b6383bdf)

10. Búsqueda del binario en GTFOBins

  ![10  GTFOBins](https://github.com/DEVOURER1683/Escolares/assets/84418941/2918e3aa-2a57-4597-9a93-09dcf5f95186)

11. Ejecución del binario con sudo

  ![11  Escalado de privilegios](https://github.com/DEVOURER1683/Escolares/assets/84418941/a5dad25f-d5ca-4c21-9142-cc64e7d88c89)
