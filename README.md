# Lista-comandos

## Clonar ramas remotas Github

1. Clonar el repositorio
  ```bash
  git clone url_repositorio  
  ```

2. Ver ramas remotas
  ```bash
  git branch -r   
  ```

3. Crear una rama local a partir de una rama remota
```bash
git checkout -b nombre_rama origin/nombre_rama_remota   
```

4. Hacer commit y subir cambios a la rama remota
```bash
  git add .
  git commit -m "mi commit"
  git push origin nombre_rama_remota 
```

5. Actualizar rama local desde rama remota
```bash
  git pull origin nombre_rama
```

## Combinar ramas (Merge)
```bash
git branch
git checkout -b nombre-de-tu-rama
git add .
git commit -m "Mensaje de tu commit"
git push origin nombre-de-tu-rama
git fetch
git merge origin/nombre_rama
Solucionar los conflictos manualmente*
git add .gitignore mysite/settings.py (Agregar cambios en donde se soluciono los conflictos)
git commit -m "Merch con cambios"
git merge --continue (Solo para asegurar si ya no hay un merge)
Checar viendo en el local los cambios y hacer migraciones y comprobar el funcionamiento
```

## Carga de datos json en Django
En el proyecto de django en la carpeta de la app se crea una carpeta llamada "fixtures", 
en esta carpeta se colocaran todos los archivos a importar para la base de datos en formato
json

La estructura que sigue el archivo json para cargar datos en la BD es la siguiente:
```bash
[
    {
        "model": "nombre_del_modelo",
        "pk": 1, #la llave primaria
        "fields": { # los campos del modelo
            "nombre":"Wilson",
            "edad":40,
            "dirrecion":Avenue #1930
        }
    },
```

## Crear el entorno Virtual en Django
1. Crear el entorno virtual
```bash
python -m venv env
```

2. Para ejecutar el entorno virtual 
```bash
.\env\Scripts\Activate
```

3. Instalar Django
```bash
   pip install django
```

4. Actualizar el pip
```bash
pip install --upgrade pip
```

5- Ejecutar el servidor
```bash
python manage.py runserver
```

## gitignore
El archivo .gitignore se crea en la raiz del proyecto
se cololan los archivos que no se quieren subir al repositorio
y por lo tanto seran ignorados al hacer commit. 

```bash
.gitignore

/env
_pycache_/
*.pyc

**/settings.py 
  
```








