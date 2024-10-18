
# Root Config - svelte-react-vue-angular-spa

Este proyecto es el **root-config** del ecosistema de microfrontends de la **Facultad FIIS - UNAS**. Fue creado utilizando el siguiente comando:

```bash
npm init single-spa
```

El **root-config** utiliza `single-spa-router` para gestionar y orquestar las rutas entre las diferentes aplicaciones microfrontend.

## Propósito del Proyecto

El **root-config** es el núcleo del sistema y tiene las siguientes responsabilidades:

- Orquestar las rutas entre las aplicaciones **React**, **Angular** y **Vue**.
- Gestionar la navegación dinámica sin recarga de página para proporcionar una experiencia fluida.
- Renderizar los microfrontends en un modal flotante de manera modular.
- Facilitar la integración de aplicaciones que incluyen **IoT**, gestión de estudiantes e importaciones tecnológicas en un ecosistema unificado.

## Aplicaciones Microfrontend

- **React**: Sistema de registro de estudiantes.
- **Vue**: Gestión de importaciones tecnológicas.
- **Angular**: Monitoreo de sistemas IoT.
- **Svelte**: Navbar central.

## Cómo Ejecutar el Root Config

### Requisitos

Asegúrate de tener **Node.js** versión 16:

```bash
nvm install 16
```

Instala las dependencias del proyecto:

```bash
npm install
```

### Iniciar el Root Config

Para ejecutar el servidor de desarrollo:

```bash
npm start
```

El **root-config** estará disponible en:  
[http://localhost:9000/](http://localhost:9000/)

## Navegación y Rutas

El **single-spa-router** controla las rutas para cada microfrontend:

- **Inicio**: `/`
- **React (Registro de Estudiantes)**: `/react`
- **Vue (Gestión de Importaciones)**: `/vue`
- **Angular (Monitoreo IoT)**: `/angular`

Cada ruta abre la aplicación correspondiente dentro de un modal flotante, mejorando la experiencia del usuario.

## Estructura del Proyecto

- **root-config**: Define la configuración central del sistema.
- **SystemJS**: Carga dinámicamente los microfrontends desde sus servidores.
- **Import Maps**: Gestiona las dependencias compartidas y la ubicación de los microfrontends.

## Scripts Disponibles

- **npm start**: Inicia el servidor de desarrollo del **root-config**.
- **npm run build**: Compila la configuración raíz para producción. Los archivos compilados se guardarán en la carpeta `dist/`.

## Cómo Funciona el Sistema

El sistema utiliza **modales flotantes** para cargar cada microfrontend de manera dinámica. Esto permite:

- Navegación fluida sin recargar toda la página.
- Modularidad completa, ya que cada aplicación se desarrolla de forma independiente.
- Fácil mantenimiento y escalabilidad, con aplicaciones aisladas y gestionadas por el **root-config**.

## Conclusión

Este **README.md** cubre los pasos necesarios para ejecutar y mantener la configuración raíz del sistema **FIIS** basado en **Single-SPA**. El **root-config** es esencial para integrar múltiples aplicaciones en un ecosistema modular, proporcionando una experiencia eficiente para estudiantes y docentes de la **Facultad FIIS - UNAS**.
