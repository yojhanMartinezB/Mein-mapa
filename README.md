<div align="center">

# 🗺️ MEIN MAPA

### Explorando la movilidad urbana a través de los datos

**Prototipo web interactivo para consultar información histórica de movilidad en La Candelaria (Comuna 10), Medellín, Colombia.**

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**Proyecto académico · Ingeniería en Ciencias de Datos · ITM**

</div>

---

## 📌 ¿Qué es Mein Mapa?

**Mein Mapa** es un prototipo de aplicación web desarrollado para facilitar la exploración y visualización de **datos históricos de movilidad vehicular** en el sector de **La Candelaria, Comuna 10 de Medellín**.

Su propósito es transformar registros de movilidad en información más accesible mediante una interfaz que combina un **mapa interactivo**, la **selección de origen y destino** y la **consulta de indicadores por hora y corredor vial**.

El proyecto integra desarrollo web, bases de datos y procesamiento de información, sentando las bases para una evolución futura hacia **modelos predictivos de congestión** y **recomendación de rutas**.

> **Estado del proyecto:** prototipo funcional en desarrollo. Los indicadores actuales se basan en datos históricos; no representan tráfico en tiempo real ni predicciones validadas.

## 🎯 Objetivo

Desarrollar una plataforma web que permita consultar y visualizar información histórica de movilidad de La Candelaria, utilizando un mapa interactivo y herramientas de procesamiento de datos para apoyar la comprensión de las condiciones de circulación vehicular.

## ✨ Funcionalidades

- 🔐 **Registro e inicio de sesión:** acceso mediante usuarios almacenados en MySQL.
- 👥 **Consulta de usuarios:** visualización de registros desde el panel administrativo del prototipo.
- 🗺️ **Mapa interactivo:** selección de dos puntos sobre una imagen para indicar origen y destino.
- 🕒 **Consulta por hora:** exploración de indicadores históricos según la hora seleccionada.
- 📊 **Panel lateral de movilidad:** barras que representan indicadores relativos de congestión por corredor.
- 📁 **Integración de CSV:** procesamiento de registros históricos desde el servidor.
- 🔄 **Reinicio de selección:** posibilidad de elegir nuevamente los puntos del mapa.

## 🛠️ Tecnologías utilizadas

| Tecnología | Uso en el proyecto |
|---|---|
| **HTML5** | Estructura de páginas y formularios |
| **CSS3** | Diseño y distribución visual de la interfaz |
| **JavaScript** | Interactividad del mapa y actualización de consultas |
| **PHP** | Sesiones, lógica del servidor y lectura de datos |
| **MySQL / MariaDB** | Almacenamiento de usuarios |
| **XAMPP** | Entorno de desarrollo local con Apache y base de datos |
| **CSV / JSON** | Fuente de datos históricos e intercambio de resultados |

## ⚙️ ¿Cómo funciona?

1. **Acceso:** el usuario se registra o inicia sesión.
2. **Selección:** desde el mapa, marca un punto de origen y otro de destino.
3. **Consulta:** selecciona la hora del viaje para consultar datos históricos.
4. **Visualización:** el sistema muestra indicadores por corredor en un panel lateral.

### Arquitectura general

```text
Usuario
   │
   ▼
Interfaz web (HTML + CSS + JavaScript)
   │
   ▼
Servidor local (Apache + PHP)
   ├── MySQL: usuarios y autenticación
   └── CSV: registros históricos de movilidad
   │
   ▼
Respuesta JSON y visualización en el navegador
```

## 🚀 Instalación local

### Requisitos

- XAMPP con **Apache** y **MySQL/MariaDB**.
- Navegador web moderno.
- Archivos del proyecto y respaldo SQL de la base de datos, si se distribuye por separado.

### Pasos

1. Clona el repositorio en la carpeta `htdocs` de XAMPP:

   ```bash
   cd C:\xampp\htdocs
   git clone https://github.com/TU_USUARIO/mein-mapa.git
   ```

2. Inicia **Apache** y **MySQL** desde el panel de XAMPP.
3. Crea la base de datos e importa el archivo `.sql` correspondiente, **si está incluido en el repositorio**.
4. Configura las credenciales locales en `app/config/database.php` según tu entorno. **No publiques contraseñas reales.**
5. Verifica que los recursos del mapa y el CSV estén en las rutas que utiliza la aplicación.
6. Abre en el navegador:

   ```text
   http://localhost/mein-mapa/app/public/
   ```

> **Nota:** reemplaza `TU_USUARIO` por tu nombre de usuario de GitHub. Si tu repositorio tiene otro nombre o estructura, adapta la ruta de instalación.

## 📂 Organización principal del proyecto

```text
mein-mapa/
└── app/
    ├── config/
    │   └── database.php
    └── public/
        ├── index.php          # Inicio de sesión
        ├── registro.php       # Registro de usuarios
        ├── principal.php      # Panel principal
        ├── candelaria_mapa.png
        └── movilidad_candelara.csv
```

*Estructura de referencia: puede variar según los archivos que se suban finalmente.*

## 📈 Próximas mejoras

- [ ] Georreferenciar los corredores viales y sustituir el mapa estático por una solución cartográfica.
- [ ] Construir una red vial para calcular recorridos entre puntos.
- [ ] Entrenar y evaluar modelos predictivos con datos de movilidad.
- [ ] Comparar alternativas de ruta según origen, destino y hora.
- [ ] Incorporar nuevas fuentes de información y mejorar la calidad de los datos.
- [ ] Fortalecer la seguridad y preparar la aplicación para un despliegue fuera del entorno local.

## ⚠️ Alcance y limitaciones

Mein Mapa es un **prototipo académico**. Los datos consultados son históricos; las barras de congestión son indicadores exploratorios basados en velocidades relativas. **No equivalen a mediciones en tiempo real, predicciones validadas ni recomendaciones automáticas de rutas óptimas.**

## 👨‍💻 Autor

**Yojhan Martínez Betancourth**  
Ingeniería en Ciencias de Datos  
Grupo **810506006-3**  
**Instituto Tecnológico Metropolitano (ITM)** · Medellín, Colombia

---

<div align="center">

**MEIN MAPA — Datos, movilidad y tecnología para comprender mejor nuestra ciudad.** 🚦

</div>
