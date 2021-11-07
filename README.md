# Trabajo_avanzado_en_GIT
![image](https://user-images.githubusercontent.com/91153605/140666793-e06902e4-2315-469a-a483-8d57f4ae9215.png)

### PASO NECESARIO:

Lo primero de todo es clonar el repositorio: 

```bash 
git clone https://github.com/jpexposito/libro.git
cd libro
```
### EJERCICIO 1:
###### En este ejercicio tendremos que mostrar el historial de cambios de un repositorio:
1. Empezaremos viendo el historial con el comando ```git log```

![image](https://user-images.githubusercontent.com/91153605/140664896-86ec1acd-2cff-4e97-944b-145ee6a98139.png)

2. Crear la carpeta capítulos: 
###### Para ello usaremos el comando ```mkdir``` y el nombre de la carpeta ```capitulos```.
![image](https://user-images.githubusercontent.com/91153605/140664907-6b7ddadc-acc7-4634-9358-071a0e18e6e1.png)

3. Ahora añadiremos un fichero dentro de la capeta llamado capitulo1.txt:
###### Para ello usaremos el comando cat > capitulos/capitulo1.txt.
![image](https://user-images.githubusercontent.com/91153605/140664916-749a1d08-74af-47c6-a42c-2da72f4c2b6e.png)

4. Añadiremos el texto:
 ```Git es un sistema de control de versiones ideado por Linus Torvalds```:
 ######
![image](https://user-images.githubusercontent.com/91153605/140664979-87274214-de47-4673-89fb-3f7348f9fffd.png)

5. En este paso Añadiremos los cambios a una zona temporal y los mismo les realizaremos un commit con el mensaje: ```Añadido capítulo 1.```
###### Para ello utilizáremos los comandos: ```git add . ```y ``` git commit -m "Añadido capítulo 1```.
![image](https://user-images.githubusercontent.com/91153605/140663938-5a5f4cf8-84bb-48e3-a7fb-4bcb3cec3bd8.png)
![image](https://user-images.githubusercontent.com/91153605/140664930-20c90584-cd07-45f6-869e-eb4331d40c43.png)

6. Por último, volveremos a mostrar los el historial de cambio con el comando ```git log```
######
![image](https://user-images.githubusercontent.com/91153605/140665000-b394a6a1-0268-4829-bf20-de745481cda8.png)

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


![image](https://user-images.githubusercontent.com/91153605/140664838-6aa68680-fc78-4578-84df-c54f11567e84.png)

2. Ahora añadiremos los cambios y crearemos un commit con el mensaje ```Añadido capítulo 2.```

###### Utilizáremos los comandos: ```git add .``` y ```git commit -m "Añadido capítulo 2.".

![image](https://user-images.githubusercontent.com/91153605/140664820-c99910ed-a42c-4fd1-b502-440ebb796e7b.png)

3. Por últimos mostraremos las diferencias con el comando: ```git diff HEAD~2..HEAD```

![image](https://user-images.githubusercontent.com/91153605/140664812-5b6f63a8-d1e2-4ff6-9a0a-495c48334f32.png)


### EJERCICIO 3
###### En este ejercicio tendremos que mostrar la diferecncia entre la última y la primera versión del repositorio:

1. Primero crearemos el nuevo fichero con el mensaje: ```Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.```
###### Para esto utilizáremos el comando ```cat > capitulos/capitulo3.txt```.

![image](https://user-images.githubusercontent.com/91153605/140664503-cf8f5c56-468d-4250-92a8-1d716e61550e.png)

2. Ahora añadiremos los cambios y realizaremos un commit con el mensaje ```Añadido capítulo 3.```

###### Utilizáremos los comandos: ```git add .``` y ```git commit -m "Añadido capítulo 3.".

![image](https://user-images.githubusercontent.com/91153605/140664770-7b9c1dfe-c49d-4c1e-abce-24091836d56b.png)

3. Mostraremos los cambios con el comando ```git diff <>..HEAD ```
######
![image](https://user-images.githubusercontent.com/91153605/140665138-4c93e477-9d2a-4989-9381-5da12ca3a6c1.png)

### EJERCICIO 4

###### En este ejercicio mostraremos quién ha hecho cambios sobre el fichero índice:

1. Crearemos el fichero ```idicie.txt``` con el texto : ```Indice de los cápitulos, con conceptos avanzados de git```
###### 
![image](https://user-images.githubusercontent.com/91153605/140665210-fcb7145a-ff01-4cf5-a6c5-da2e0cadcfbb.png)

2. Ahora añadiremos los cambios y realizaremos un commit con el mensaje ```"Indice de los cápitulos, con conceptos avanzados de git."```

###### Utilizáremos los comandos: ```git add .``` y ```git commit -m "Indice de los cápitulos, con conceptos avanzados de git.".

![image](https://user-images.githubusercontent.com/91153605/140665288-81ebf56d-d084-4373-abb9-a3a0ed6a62e0.png)
![image](https://user-images.githubusercontent.com/91153605/140665294-a19a25f9-feea-4c92-a0dc-f2dbb28fdfc3.png)

3. Ahora mostraremos quien ha realizado cambios.

###### Para esto usaremos los comandos: 
```
  echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.txt
  git add .
  git commit -m "Añadido el índice ."
  git annotate indice.txt
```
![image](https://user-images.githubusercontent.com/91153605/140665389-ad7ab1cc-15ef-4138-a5e9-b40255be2b33.png)

### EJERCICIO 5

###### En este ejercicio crearemos una rama y mostraremos las ramas creadas: 

1. Usaremos únicamente dos comandos: 

```
  git branch bibliografia
  
  git branch -av
```
![image](https://user-images.githubusercontent.com/91153605/140665472-4ddeea69-3102-4de5-a496-cb66d6ba1ae9.png)


### EJERCICIO 6

###### En este ejercicio mostraremos el historial de repositorios y ramas: 

1. Primero crearemos un fichero con el comando: 

```cat > capitulos/capitulo4.txt ```

###### Y le añadiremos el mensaje: 

``` En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto. ```
![image](https://user-images.githubusercontent.com/91153605/140665561-7ab48166-bd25-4a30-8e15-71fa93108075.png)

2. Ahora añadiremos los cambios y realizaremos un commit con el mensaje ```"Añadido capítulo 4."```

###### Utilizáremos los comandos: ```git add .``` y ```git commit -m "Añadido capítulo 4.".

![image](https://user-images.githubusercontent.com/91153605/140665585-48a18f57-dc34-40a4-b697-31da1276c76c.png)

3. Por último mostraremos el historial de repositorio y las ramas: 
###### 
![image](https://user-images.githubusercontent.com/91153605/140665625-a4b3fe7f-d69e-433d-86ba-4c7e617ede3d.png)

### EJERCICIO 7

###### En este ejercicio mostraemos trabajaremos en la rama bibliografía: 

1. Primero nos situaremos en la rama bibliografía: 

###### Usaremos el comando: 
```
git checkout bibliografia
```
![image](https://user-images.githubusercontent.com/91153605/140665714-84bf257d-7ec9-46d0-a2ba-f4cc388713a1.png)

2. Crearemos un fichero y le añadiremos texto: 
###### Usaremos los comandos: 
```
cat > bibliografia.txt
Chacon, S. and Straub, B. Pro Git. Apress.
Ctrl+D
```
![image](https://user-images.githubusercontent.com/91153605/140665775-818bcbbb-ed63-43cd-91a3-841cf3e1a09b.png)

3. Ahora añadiremos los cambios y realizaremos un commit con el mensaje ```"Añadida primera referencia bibliográfica."```

###### Utilizáremos los comandos: ```git add .``` y ```git commit -m "Añadida primera referencia bibliográfica.".
![image](https://user-images.githubusercontent.com/91153605/140665852-52449d58-ff60-451d-a073-fd65dd46a81d.png)

4. Por último, mostraremos el historial con el comando: 

```git log --graph --all --oneline ```
![image](https://user-images.githubusercontent.com/91153605/140665904-337f8d17-89fe-450f-aa91-9d938088d7b6.png)


### EJERCICIO 8
###### En este ejercicio fusionaremos ramas: 

1. Nos situamos en la rama main y realizamos un merge de la rama bibliografia: 

2. MOstramos el historial del repositorio. 

3. Eliminamos la rama bibliografia:

4. Y volvemos a mostrar el historial:
###### 
![image](https://user-images.githubusercontent.com/91153605/140666206-0ff2605a-2b69-4b37-b671-f854ef918672.png)

```
git checkout main
git merge bibliografia
git log --graph --all --oneline
git branch -d bibliografia
git log --graph --all --oneline
```


###### Al no copiarse al completo la rama bibliografía, no la terminé de borrar por desconocimiento de lo que faltaba por copiar, pero posteriormente fue borrada para poder realizar el ejercicio 9.

### EJERCICIO 9

1. Crearemos la rama bibliografia, nos posicionamos en ella y le añadimos texto: 

```
> git branch bibliografia
> git checkout bibliografia
> cat > bibliografia.txt
Scott Chacon and Ben Straub. Pro Git. Apress.
Ryan Hodson. Ry's Git Tutorial. Smashwords (2014)
```
![image](https://user-images.githubusercontent.com/91153605/140666324-49c39b2a-775b-419f-857b-fabe25fa7348.png)

2. realizamos commit y no movemos a la rama main donde crearemos un txt: 

```
git commit -a -m "Añadida nueva referencia bibliográfica."
> git checkout main
> cat > bibliografia.txt
- Chacon, S. and Straub, B. Pro Git. Apress.
- Loeliger, J. and McCullough, M. Version control with Git. O'Reilly.
Ctrl+D
```
![image](https://user-images.githubusercontent.com/91153605/140666382-d4032995-b52c-4276-b6d2-c9bbca68403f.png)

3. Ahora añadiremos los cambios y fusionaremos las ramas.

```
git commit -a -m "Añadida nueva referencia bibliográfica."
git merge bibliografia
```
![image](https://user-images.githubusercontent.com/91153605/140666443-2e5d0c19-fdfe-4e8e-b86a-ff7e77409980.png)





































