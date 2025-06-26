# Chat en Tiempo Real con Node.js, Express y Socket.io

Este proyecto es una aplicación de chat sencilla desarrollada con Node.js, Express, Pug y Socket.io. Permite a varios usuarios conectarse y enviar mensajes en tiempo real a través de una interfaz web.

## Características

- Envío y recepción de mensajes en tiempo real entre todos los usuarios conectados.
- Notificación cuando un usuario se conecta o desconecta.
- Visualización del número de clientes conectados en todo momento.
- Interfaz web sencilla usando Pug como motor de plantillas.

## Requisitos

- [Node.js](https://nodejs.org/) (versión recomendada: 14.x o superior)
- [npm](https://www.npmjs.com/)

## Instalación

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/alberzh/Chat.git
   cd Chat/Chat
   ```

2. **Instala las dependencias:**

   ```bash
   npm install
   ```

## Uso

### En desarrollo

Para iniciar el servidor en modo desarrollo (con recarga automática):

```bash
npm run dev
```

### En producción

Para iniciar el servidor en modo producción:

```bash
npm start
```

El servidor se ejecutará por defecto en [http://localhost:3000](http://localhost:3000).

## Estructura del Proyecto

```
Chat/
├── bin/
│   └── www.js           # Punto de entrada del servidor
├── public/
│   └── stylesheets/
│       └── style.css    # Estilos CSS
├── routes/
│   ├── index.js         # Rutas principales
│   └── users.js         # Rutas de usuarios (ejemplo)
├── views/
│   ├── index.pug        # Vista principal del chat
│   ├── layout.pug       # Plantilla base
│   └── error.pug        # Vista de errores
├── app.js               # Configuración principal de Express
├── package.json         # Dependencias y scripts
└── .gitignore
```

## Funcionamiento

- Cuando un usuario se conecta, se muestra un mensaje informativo y se actualiza el número de clientes conectados.
- Los mensajes enviados por cualquier usuario se muestran en tiempo real a todos los conectados.
- Al desconectarse un usuario, se notifica al resto y se actualiza el contador de clientes.

## Créditos

Desarrollado como ejercicio para el curso de **Desarrollo de Aplicaciones con NodeJS y Express** en OpenWebinars.

---

¡Siéntete libre de modificar y mejorar este proyecto!
