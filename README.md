# SmartQuiz

Plataforma web de evaluación académica tipo quiz interactivo, con roles de profesor y alumno, partidas en tiempo real, ranking y creación de cuestionarios (incluyendo importación desde Excel).

## Tecnologías

- **Backend:** Python 3, Flask
- **Base de datos:** MySQL (PyMySQL)
- **Autenticación:** Flask-Login con hash SHA-256
- **Correo:** Flask-Mail (verificación de cuenta y recuperación de contraseña)
- **Frontend:** HTML5, CSS3, JavaScript
- **Importación de quizzes:** pandas + openpyxl

## Requisitos

- Python 3.10 o superior
- MySQL

## Instalación local

1. Clona el repositorio:
   ```bash
   git clone https://github.com/AlonsoUSAT/SmartQuiz.git
   cd SmartQuiz
   ```

2. Crea y activa un entorno virtual:
   ```bash
   python -m venv venv
   # Windows
   venv\Scripts\activate
   # Linux / Mac
   source venv/bin/activate
   ```

3. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

4. Configura las variables de entorno:
   ```bash
   cp .env.example .env
   ```
   Luego edita `.env` con tus credenciales reales de base de datos y correo.

5. Ejecuta la aplicación:
   ```bash
   python app.py
   ```

## Variables de entorno

Ver `.env.example` para la lista completa. Nunca subas el archivo `.env` al repositorio.

## Estructura

```
SmartQuiz/
├── app.py                  # Aplicación principal Flask (rutas)
├── conexionBD.py           # Conexión a MySQL
├── controlador*.py         # Lógica de negocio por módulo
├── static/                 # CSS, JS, imágenes
├── templates/              # Plantillas HTML
├── requirements.txt        # Dependencias
└── .env.example            # Plantilla de variables de entorno
```
## Link de web desplegada

https://fhernandezleonusat.pythonanywhere.com/

```
Usuarios de prueba
```

-Para crear quizzes como docente: profesor1
-Ingresar con contraseña: Profesor123

-Para jugar a quizzes como alumno: alumno1
-Ingresar con contraseña: Alumno123

Solo acepta el registro de correos electrónicos de la Universidad Católica Santo Toribio de Mogrovejo.
