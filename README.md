# Solemne 3 Aplicaciones y tecnologias WEB - Sistema de Gestión de Citas Médicas.

Este proyecto es una aplicación web sencilla construida con Django, como parte del marco evaluativo de la universidad San Sebastián que simula la gestión de citas médicas. Permite registrar pacientes, médicos y citas, además de gestionar el estado de cada cita.  

---

## 🚀 Tecnologías utilizadas

- Python 3.9
- Django.
- PostgreSQL (para despliegue con Docker).
- Docker y Docker Compose.

---

## 📥 Instalación y ejecución local

1. **Clonar el repositorio**
   git clone https://github.com/Benjvvv10/Solemne_3.git
   cd Solemne_3
2. **Crear un entorno virtual**
  python -m venv venv
  source venv/bin/activate  # En Windows: venv\Scripts\activate
3. **Instalar dependencias**
  pip install -r requirements.txt
4. **Aplicar migraciones**
  python manage.py migrate
5. **Crear un superusuario**
  python manage.py createsuperuser
6. **Ejecuta el servidor**
  python manage.py runserve

Accede a la aplicación en: http://127.0.0.1:8000/

**🐳 Ejecución con Docker**
1. **Construir y levantar los contenedores**
  docker-compose up -d
2. **Crear un superusuario**
  docker-compose exec web python manage.py createsuperuser
3. **Acceder a la aplicación**
  Aplicación: http://localhost:8000/appointments/
4. **Detener los contenedores**
  docker-compose down
