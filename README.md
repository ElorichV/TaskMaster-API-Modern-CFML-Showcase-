# TaskMaster API (Modern CFML Showcase)

Backend RESTful para una aplicación de gestión de tareas, diseñado para demostrar las capacidades modernas del lenguaje CFML en 2025.

Este proyecto sirve como evidencia de dominio de arquitectura de software, seguridad y sintaxis moderna (Script) sobre el motor Lucee.

## 🚀 Objetivo Técnico
El propósito principal de este repositorio es ilustrar la transición de "ColdFusion Legacy" a **Modern CFML**, implementando:

* **Sintaxis 100% CFScript:** Cero uso de etiquetas tradicionales para lógica.
* **Arquitectura Orientada a Componentes:** Separación clara de responsabilidades (Service Layer Pattern).
* **API REST JSON:** Endpoints que consumen y retornan datos JSON estandarizados.
* **Seguridad:** Implementación estricta de `QueryExecute` con parámetros (`cfsqltype`) para prevenir Inyección SQL.
* **Entorno Portable:** Configuración basada en **CommandBox** para despliegue inmediato sin dependencias de instalación global.

## 🛠️ Stack Tecnológico

* **Lenguaje:** CFML (ColdFusion Markup Language)
* **Motor:** Lucee 6.x (Open Source)
* **Servidor/CLI:** CommandBox
* **Base de Datos:** H2 (Embebida para demo) / MySQL (Compatible)
* **Formato de Datos:** JSON

## 🔌 API Endpoints

| Método | Endpoint | Descripción |
| :--- | :--- | :--- |
| `GET` | `/api/tasks` | Obtiene todas las tareas. |
| `GET` | `/api/tasks/{id}` | Obtiene una tarea específica. |
| `POST` | `/api/tasks` | Crea una nueva tarea. |
| `PUT` | `/api/tasks/{id}` | Actualiza una tarea existente. |
| `DELETE` | `/api/tasks/{id}` | Elimina una tarea. |

## ⚡ Instalación y Despliegue Local

Este proyecto no requiere instalar Adobe ColdFusion ni configurar IIS/Apache.

1.  **Requisitos:** Tener instalado [CommandBox](https://www.ortussolutions.com/products/commandbox).
2.  **Clonar:** `git clone https://github.com/TU_USUARIO/modern-cfml-task-api.git`
3.  **Iniciar:** Navegar a la carpeta y ejecutar:
    ```bash
    box server start
    ```
4.  **Probar:** El navegador se abrirá automáticamente.

---
*Desarrollado por Axel Alberto Linares Lorrabaquio - 2025*
