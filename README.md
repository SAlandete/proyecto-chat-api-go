# Chat App en Go

Proyecto de chat en tiempo real desarrollado en Go, utilizando WebSocket para permitir la comunicación instantánea entre múltiples usuarios conectados desde el navegador.

## Descripción

La aplicación permite que varios usuarios ingresen a una sala de chat y puedan enviar y recibir mensajes en tiempo real sin necesidad de recargar la página.

El proyecto utiliza un Hub central encargado de administrar las conexiones, registrar usuarios, detectar desconexiones y distribuir los mensajes a los clientes conectados.

## Tecnologías utilizadas

- Go
- WebSocket
- Gorilla WebSocket
- HTML
- CSS
- JavaScript
- Git y GitHub

## Conceptos aplicados

- Goroutines
- Channels
- Select
- Comunicación cliente-servidor
- Conexiones persistentes con WebSocket
- Manejo de múltiples usuarios conectados

## Estructura del proyecto

```text
chat-app/
├── cmd/
│   └── main.go
├── internal/
│   ├── hub/
│   │   ├── hub.go
│   │   ├── client.go
│   │   └── helpers.go
│   ├── handlers/
│   │   └── ws.go
│   └── models/
│       └── models.go
├── static/
│   └── index.html
├── go.mod
├── go.sum
└── README.md