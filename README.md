# Pasos para ejecutar una aplicación de Django desde un repositorio usando un entorno virtual (venv)

1. **Clona el repositorio**  
    ```bash
    git clone <URL-del-repositorio>
    cd <nombre-del-repositorio>
    ```

2. **Crea un entorno virtual con venv**  
    ```bash
    python3 -m venv venv
    ```

3. **Activa el entorno virtual**  
    En Linux/Mac:
    ```bash
    source venv/bin/activate
    ```

4. **Instala las dependencias**  
    ```bash
    pip install -r requirements.txt
    ```

5. **Configura la base de datos**  
    Ajusta la configuración en `settings.py` si es necesario.

6. **Realiza migraciones**  
    ```bash
    python manage.py migrate
    ```

7. **Crea un superusuario (opcional)**  
    ```bash
    python manage.py createsuperuser
    ```

8. **Ejecuta el servidor de desarrollo**  
    ```bash
    python manage.py runserver
    ```

¡Listo! Ahora puedes acceder a tu aplicación en `http://localhost:8000/`.