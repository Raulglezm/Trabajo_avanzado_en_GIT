# Trabajo_avanzado_en_GIT

### PASO NECESARIO:

Lo primero de todo es clonar el repositorio: 

```bash 
git clone https://github.com/jpexposito/libro.git
cd libro
```
### EJERCICIO 1:
###### En este ejercicio tendremos que mostrar el historial de cambios de un repositorio:
1. Empezaremos viendo el historial con el comado ```git log```

![image](https://user-images.githubusercontent.com/91153605/140663628-f8400ec4-c83b-414e-8977-1cdbf8b3ee4a.png)

2. Crear la carpeta capítulos: 
###### Para ello usaremos el comando ```mkdir``` y el nombre de la carpeta ```capitulos```.
![image](https://user-images.githubusercontent.com/91153605/140663669-6a3a67ca-632f-4dda-8115-a8daa5b62de3.png)

3. Ahora añadiremos un fichero dentro de la capeta llamado capitulo1.txt:
###### Para ello usaremos el comando cat > capitulos/capitulo1.txt.
![image](https://user-images.githubusercontent.com/91153605/140663744-897d6d70-0f62-4dce-bf45-2283368ac317.png)

4. Añadiremos el texto:
 ```Git es un sistema de control de versiones ideado por Linus Torvalds```:
![image](https://user-images.githubusercontent.com/91153605/140663907-75befe8a-ba16-467e-a7dc-95823a51d46f.png)

5. En este paso Añadiremos los cambios a una zona temporal y los mismo les realizaremos un commit con el mensaje: ```Añadido capítulo 1.```
###### Para ello utilizaremos los comandos: ```git add . ```y ``` git commit -m "Añadido capítulo 1```.
![image](https://user-images.githubusercontent.com/91153605/140663938-5a5f4cf8-84bb-48e3-a7fb-4bcb3cec3bd8.png)

6. Por último volveremos a mostrar los el historial de cambio con el comando ```git log```
![image](https://user-images.githubusercontent.com/91153605/140664060-040c06f5-e3cd-4ed5-b992-f959f1e76b80.png)

### EJERCICIO 2:

###### En este ejercicio tendremos que mostrar las diferencias entra la última versión y dos versiones anteriores.

1. Primero crearemos un nuevo fichero y añadiremos el texto ```El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal. 3- Hacer un commit de los cambios. ```

###### Para ello usaremos:
```
 cat > capitulos/capitulo2.txt
 
 El flujo de trabajo básico con Git consiste en:
 1- Hacer cambios en el repositorio.
 2- Añadir los cambios a la zona de intercambio temporal.
 3- Hacer un commit de los cambios.
 ```


![image](https://user-images.githubusercontent.com/91153605/140664201-c13340cb-c8d8-435d-bee0-1625b54b585d.png)

2. Ahora añadiremos los cambios y crearemos un commit con el mensaje ```Añadido capítulo 2.```

###### Utilizaremos los comandos: ```git add .``` y ```git commit -m "Añadido capítulo 2.".

![image](https://user-images.githubusercontent.com/91153605/140664211-fa0c9b37-d9c8-41ee-8604-44a0c168ac0a.png)

3. Por últimos mostraremos las diferencias con el comando: ```git diff HEAD~2..HEAD```

![image](https://user-images.githubusercontent.com/91153605/140664225-66f51cf8-f943-4240-8206-5a0bb5e75d74.png)




### EJERCICIO 3

### EJERCICIO 4

### EJERCICIO 5

### EJERCICIO 6

### EJERCICIO 7

### EJERCICIO 8

