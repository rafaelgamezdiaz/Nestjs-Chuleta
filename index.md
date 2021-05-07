## Nestjs-Chuleta


**Índice**   
1. [Instalación](#id_instalacion)
2. [Crear un proyecto](#id_crear_proyecto)
3. [Iniciar el proyecto](#id_crear_proyecto)
4. [Modulos](#id_module)
5. [Controladores](#id_controller)
6. [Servicios](#id_service)
7. [Modelos](#id_model)



### Instalación<a name="id_instalacion"></a>

Instalar de forma global

```
 npm i –g @nestjs/cli
```


### Crear un proyecto<a name="id_crear_proyecto"></a>

```
 nest new project_name
``` 


### Iniciar el proyecto en modo desarrollador<a name="id_iniciar_proyecto"></a>

```
 npm run start:dev
```


### Modulos<a name="id_module"></a>

```
 nest g module tasks
```



### Controladores<a name="id_controller"></a>


```
 nest g controller tasks
```
### Servicios<a name="id_service"></a>


```
 nest g service tasks
```


### Modelos<a name="id_model"></a>

Podemos definir los modelos ya sea a través de una **clase** o de una **interface**. La diferencia de implementar un módelo a partir de una interface o una clase es que una interface permite establecer la estructura en el momento de la compilación, pero una ver terminada la compilación no se preservan sus cualidades como unterfaco. En cambio si se implementa a partir de una clases si se preservan sus cualidades. Es aconsejable comenzar implementando un modelo como una interfaz, y solo los caso de que se requiera de debería cambiar a implementarlo a traves de una clase.

Ejemplo de un modelo creado a partir de una interface

```
 export interface TaskModel {
  id: string;
  title: string;
  description: string;
  status: TaskStatus;
 }
```
