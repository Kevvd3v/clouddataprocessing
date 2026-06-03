# Cloud Data Processing

Portafolio de tareas y bitácora de la materia **Procesamiento de Datos en la Nube**.

## Información general

**Alumno:** Kevin Yahir Chan Caballero  
**Materia:** Procesamiento de Datos en la Nube  
**Profesor:** Dr. Ismael Jiménez Sánchez  
**Repositorio:** clouddataprocessing  

---

## Bitácora de clases

### Clase 1 - Introducción a Cloud Data Processing (01/06/2026)

En la primera clase se presentaron conceptos relacionados con el procesamiento de datos en la nube, infraestructura como código, automatización y herramientas modernas de desarrollo.

Temas mencionados:

* Branching strategy
* Cloud agnostic
* Infrastructure as Code
* Terraform
* Pulumi
* CloudFormation
* HCL
* IaaS, PaaS y SaaS
* CI/CD
* GitHub Actions
* GitLab CI/CD
* Jenkins
* FluxCD
* Colima
* Roadmap.sh

---

### Clase 2 - Git, Git Flow y trabajo colaborativo (02/06/2026)

En la segunda clase se revisaron conceptos básicos de **Git** y su importancia dentro del desarrollo colaborativo. Se explicó que Git permite llevar un control de versiones del código, registrar cambios mediante commits y trabajar con ramas para organizar mejor el desarrollo de un proyecto.

También se explicó el flujo de trabajo conocido como **Git Flow**, el cual propone el uso de diferentes ramas para separar el código estable, el desarrollo, nuevas funcionalidades y correcciones.

Ramas mencionadas:

* `main` o `master`: rama principal donde se mantiene el código estable.
* `develop`: rama de desarrollo donde se integran los cambios antes de enviarlos a producción.
* `feature`: ramas utilizadas para desarrollar nuevas funcionalidades.
* `release`: ramas usadas para preparar una versión antes de publicarla.
* `hotfix`: ramas utilizadas para corregir errores urgentes en producción.

Comandos básicos revisados:

```bash
git init
git status
git add .
git commit -m "mensaje del commit"
git push
git fetch
git pull
git clone
git branch
git checkout
git merge
```

Ejemplo de flujo básico:

```bash
git branch "998"
git checkout "998"
git add .
git commit -m "Added Evidence for 998"
git checkout main
git merge "998"
git push
```

Buenas prácticas mencionadas para trabajo colaborativo:

* No trabajar directamente sobre la rama principal.
* Crear ramas específicas para cada tarea o funcionalidad.
* Usar mensajes de commit claros y descriptivos.
* Hacer `pull` antes de comenzar a trabajar para tener los cambios más recientes.
* Revisar el estado del repositorio con `git status`.
* Mantener una organización clara entre ramas locales y remotas.
* Usar plataformas como GitHub, GitLab o Gitea para colaborar en equipo.
* Practicar los conceptos de Git mediante el juego **Oh My Git**.

---

## Tareas

### Tarea #998 - Diagrama de arquitectura de 3 capas en la nube

**Fecha de entrega:** Martes 2 de junio

**Descripción:**
Realizar un diagrama de arquitectura para una aplicación de 3 capas en la nube.

Capas solicitadas:

1. Frontend
2. Backend
3. Database

**Evidencia:**

*Enlace de Lucidchart:*
https://lucid.app/lucidchart/5a613fc3-54e4-4588-870d-0973be1fe171/edit?viewport_loc=-166%2C-267%2C1977%2C887%2C0_0&invitationId=inv_35781220-677a-4e37-97a9-ef22d39f10be

**Captura del diagrama:**

<img width="1290" height="1025" alt="Diagrama 3 capas" src="https://github.com/user-attachments/assets/21153efe-3256-4775-916f-27c76214c3e0" />

---

### Tarea #999 - Configuración inicial del entorno

**Fecha de entrega:** Miércoles 3 de junio

Actividades solicitadas:

* Crear cuenta de GitHub.
* Registrarse en GitHub Education.
* Crear repositorio de tareas con el nombre `clouddataprocessing`.
* Llevar una bitácora de clases en Markdown dentro del archivo README.
* Instalar VirtualBox.
* Instalar una máquina virtual con Linux.
* Instalar un container engine, por ejemplo Docker.
* Instalar Python 3.

**Estado:** Completado.

Se creó el repositorio `clouddataprocessing` para llevar el portafolio de tareas y la bitácora de clases en formato Markdown. Además, se instaló una máquina virtual con Ubuntu 24.04 LTS dentro de VirtualBox.

Dentro de la máquina virtual se verificó la instalación de Python 3 y Docker mediante los siguientes comandos:

```bash
python3 --version
docker --version
sudo docker run hello-world
```

Resultados obtenidos:

* Python 3.12.3 instalado correctamente.
* Docker 29.1.3 instalado correctamente.
* Docker ejecutó correctamente el contenedor de prueba `hello-world`.

**Evidencia:**

<img width="1365" height="721" alt="Instalacion-Ubuntu-Python3-Docker" src="https://github.com/user-attachments/assets/e090131d-dcd9-4a16-b25e-39e502557202" />

<img width="1365" height="726" alt="Hello-World-Docker" src="https://github.com/user-attachments/assets/27f2ddbe-da50-4cf2-84ee-821b97806fb9" />




