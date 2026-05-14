# AUTOMATIZACION-EN-N8N

## Descripción

Este proyecto fue desarrollado en n8n con el objetivo de automatizar el proceso de solicitud y análisis de préstamos bancarios sin intervención manual, exceptuando el ingreso inicial de información por parte del solicitante.

El usuario únicamente debe proporcionar los documentos y datos requeridos por el sistema. Posteriormente, n8n se encarga automáticamente del análisis de información, validación de riesgos, evaluación de viabilidad del préstamo y generación de resultados.

Finalmente, el sistema notifica al cliente el resultado de su solicitud mediante correo electrónico.

## Tecnologías utilizadas

- n8n
- Docker Desktop
- PostgreSQL
- GitHub

## Requisitos

- Docker Desktop
- PostgreSQL
- Git

## Instalación

Clonar el repositorio:

```bash
git clone https://github.com/daniel43-cod/AUTOMATIZACION-EN-N8N.git
```

Entrar a la carpeta del proyecto:

```bash
cd AUTOMATIZACION-EN-N8N
```

Levantar n8n con Docker:

```bash
docker compose up -d
```

## Base de Datos

El proyecto utiliza PostgreSQL instalado localmente.

Debe existir una base de datos llamada:

```txt
postgres
```

Además, deben existir las siguientes tablas:

- clientes
- creditos
- datos_laborales
- referencias_familiares

## Acceso a n8n

Abrir en el navegador:

```txt
http://localhost:5679
```

## Workflows incluidos

- Workflow 1: Automatización principal del proceso de préstamos
- Workflow 2: Integración y validación con PostgreSQL

Los archivos JSON exportados se encuentran en la carpeta:

```txt
workflows/
```

## Documentación

La documentación y diagramas del proyecto se encuentran en:

```txt
docs/
```

## Ejecución de pruebas

1. Iniciar Docker Desktop
2. Ejecutar `docker compose up -d`
3. Abrir n8n en el navegador
4. Importar los workflows
5. Ejecutar las pruebas del sistema

## Autor

Daniel Javier Iqui Coy