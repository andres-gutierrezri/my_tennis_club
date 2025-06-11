
# Proyecto: Ejemplo inicial para Django

## Requisitos
| Software | Versión recomendada |
|----------|--------------------|
| Python   | 3.10 o superior |
| Dependencias de Python | Ver `requirements.txt` |

## Instalación

# Habilitar la Ejecución de Scripts en PowerShell
```powershell
# Directiva de ejecución para el usuario actual
Set-ExecutionPolicy -Scope CurrentUser Unrestricted -Force

# Comprobar la directiva de ejecución
# Debe mostrar Unrestricted
Get-ExecutionPolicy -List
```

# Verificar la instalación de Python y pip
```bash
# comprobar la versión de Python
python --version

# Verificar la instalación de pip
pip --version

# Actualizar pip
pip install --upgrade pip
```

# Instalar dependencias de Python
```bash
# Instalar entorno virtual de Python
python -m venv .venv

# Windows
.\.venv\Scripts\activate

# Linux
source .venv/bin/activate

# Comprobar que el entorno virtual está activado
# Debe mostrar la ruta del entorno virtual
python -c "import sys; print(sys.prefix)"

# Actualizar pip dentro del entorno virtual
python -m pip install --upgrade pip --no-cache-dir
```

# Instalar dependencias
```bash
# Comprobar la versión de pip
pip --version

# Instalar las dependencias del proyecto
pip install -r requirements.txt --no-cache-dir

# Comprobar que las dependencias se han instalado correctamente
pip check

# Verificar la instalación de dependencias

# Comprobar las dependencias instaladas con sus versiones
pip list

# Comprobar si hay actualizaciones disponibles
pip list --outdated

# Comprobar la versión de Django
django-admin --version
```

## Uso inicial
Para iniciar el proyecto, primero asegúrese de que el entorno virtual está activado. Luego, debe correr las siguientes instrucciones:

```bash
# Correr migraciones
python manage.py migrate

# Ejecutar el servidor de desarrollo
python manage.py runserver
```

## Control de versiones

```bash
git init
git add .
git commit -m "feat: Ejemplo inicial para Django"
git remote add origin https://github.com/USUARIO/my_tennis_club.git
git push -u origin main
```

Para GitLab sustituya la URL de *remote*.

## Mensajes de Commit Recomendados

Para mantener un historial de commits claro y conciso, se recomiendan los siguientes formatos de mensaje:

*   **feat**: Nueva característica

---

© 2025 · Licencia MIT
