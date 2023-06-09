# taller09-refuerzo

## Importar usuario en Django

1. Crear un proyecto en Django llamada **miproyecto**

  1.1. Crear un super usuario
  1.2. Probar el ingreso al admin

2. Ingresar a la consola de Django

```
python manage.py shell
```

3. Leer el archivos .csv

3.1. Agregar la lógica necesaria para generar los usuarios en función de la archivos.

4. Analizar como usar las siguiente líneas de código que en su conjunto permiten agregar usuarios a Django.

```
from django.contrib.auth.models import User
user = User.objects.create_user(user_name, user_correo, user_clave)
user.is_active = True
user.is_staff = False
user.last_name = last_name
user.first_name = first_name
user.save()
```

**Importante**
* Probar el proceso en sqlite
