# 🔒 Encrypted Chat

Un chat cifrado con End-to-End Encryption (E2EE) basado en **Python**, utilizando **Sockets** y **SSL** para una comunicación segura entre cliente y servidor.

---

## 🚀 Características

- 🔐 **Cifrado SSL** para proteger las comunicaciones.
- 🧵 **Uso de hilos** para manejar múltiples clientes simultáneamente.
- 📜 **Interfaz gráfica (GUI)** con Tkinter en el cliente.
- 📢 **Soporte de mensajes públicos**.
- 👥 **Comando para listar usuarios conectados**.
- ❌ **Manejo de desconexión de clientes**.

---

## 🛠️ Instalación y ejecución

### 1️⃣ Clonar el repositorio

```bash
git clone git@github.com:FJLdx/encrypted-chat.git
cd encrypted-chat
```

### 2️⃣ Generar los certificados SSL

Antes de iniciar, se deben generar los certificados SSL para establecer una conexión segura:

```bash
openssl req -x509 -newkey rsa:4096 -keyout server-key.key -out server-cert.pem -days 365 -nodes
```

Esto generará dos archivos:
- `server-key.key`: Clave privada del servidor.
- `server-cert.pem`: Certificado público.

### 3️⃣ Ejecutar el servidor

```bash
python3 server.py
```

### 4️⃣ Ejecutar el cliente

```bash
python3 client.py
```

Se solicitará un nombre de usuario y se abrirá una ventana de chat con las siguientes opciones:
- **Escribir y enviar mensajes**.
- **Listar los usuarios conectados** con el botón `Listar usuarios`.
- **Salir del chat** con el botón `Salir`.

---

## 🖥️ Uso

1️⃣ Inicia el **servidor** antes que los clientes.
2️⃣ Abre varios **clientes** en diferentes terminales o máquinas.
3️⃣ Ingresa un nombre de usuario cuando se te solicite.
4️⃣ ¡Empieza a chatear de manera segura! 🔏

### 📜 Comandos disponibles en el chat

| Comando        | Descripción                          |
|---------------|----------------------------------|
| `!usuarios`   | Muestra los usuarios conectados. |

---

## 📜 Código fuente

El código se encuentra en los archivos:

- `server.py` → Servidor del chat.
- `client.py` → Cliente con interfaz gráfica.
- `server-cert.pem` → Certificado SSL del servidor.
- `server-key.key` → Clave privada del servidor.
- `server.csr` → Solicitud de certificado.

---

## 📜 Licencia

Este proyecto está bajo la licencia **MIT**, lo que permite su uso, modificación y distribución sin restricciones.

📌 **Desarrollado por [FJLdx](https://github.com/FJLdx)**


