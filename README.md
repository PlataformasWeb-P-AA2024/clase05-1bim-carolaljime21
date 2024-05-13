# Clase05-1bim

## Consumo de información de CouchDB desde flask
### Datos de CouchDB
* Tomar la información de https://gist.github.com/reroes/a7d0a43e2578336a64bd366caa244000 y crear una base de datos en CouchDB
* Crear las siguientes vistas

``` js
# vista 1

function (doc) {
  if(doc.lenguaje){
    emit(doc.lenguaje, doc);  
  }

}

# vista 2
function (doc) {
  if(doc.lenguaje){
    emit(doc._id, doc);
  }
}

```

### Pasos para ejecutar

* Instalar la librería **flask**
  * Opción 1: en un entorno ejecutar
  ```
    pip install flask
  ```
  * Opción 2:
  ```
    pip install -r requirements.txt
  ```

flask run o flask run --port 9000
* Ingresar a la carpeta **ejemplo-flask**
* Ejecutar los siguientes comandos
```
  python app.py
```
link de video: https://www.canva.com/design/DAGFENpyZ0U/VOk_WApaPBQ-NC0figmxFg/watch?utm_content=DAGFENpyZ0U&utm_campaign=designshare&utm_medium=link&utm_source=editor

<hr>

**Repositorio con fines educativos**
