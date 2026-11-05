# 🎁 Promo Gana – Canje de Vouchers

Aplicación web para participar de una promoción: el usuario ingresa un código de voucher, el sistema lo valida, el usuario elige un premio del catálogo, completa sus datos y recibe un email de confirmación.

> Trabajo Práctico de **Programación III** de la Tecnicatura Universitaria en Programación (UTN), desarrollado por el **Equipo 10A**.

## ✨ Flujo de la aplicación

1. **Ingreso del voucher** → se valida que el código exista y no haya sido canjeado.
2. **Selección de premio** → catálogo dinámico de artículos con imágenes, en cards de Bootstrap.
3. **Registro del cliente** → si el DNI ya existe se autocompletan los datos, y hay validaciones en todos los campos.
4. **Confirmación** → se registra el canje y se envía un **email de confirmación**.
5. Hay pantallas de **canje exitoso** y de **voucher rechazado**.

## 🧱 Arquitectura

```
TPWeb-Equipo-10A/
├── Dominio/          → Entidades: Articulo, Voucher, Cliente, Marca, Categoria, Imagen
├── Negocio/          → VoucherNegocio, ClienteNegocio, ArticuloNegocio, EmailsService, AccesoDatos
└── TPWeb-Equipo10A/  → Páginas ASP.NET Web Forms con MasterPage
```

## 🛠️ Tecnologías

C# · ASP.NET Web Forms · .NET Framework · SQL Server · Bootstrap · SMTP (Mailtrap para pruebas)

## 👨‍💻 Mi aporte

- Creé la página **CanjearVoucher** y su formulario.
- Diseñé la página de **Premios** con cards de Bootstrap y estilos propios.
- Desarrollé la **selección y visualización del premio** elegido.
- Agregué las **validaciones del registro** (`RequiredFieldValidator`) y el guardado del cliente.
- Implementé el **envío de email de confirmación** de participación, probado con sandboxes de Mailtrap.

## ▶️ Cómo ejecutarlo

1. Restaurar la base de datos `PROMOS_DB` en SQL Server.
2. Abrir la solución con Visual Studio y configurar el connection string y las credenciales SMTP.
3. Ejecutar con `F5`.

## 👥 Equipo

[Marisel Alarcón](https://github.com/AlarconMarisel) · [Claudio Gobbi](https://github.com/ClaudioCesarGobbi) · [Lautaro Figueroa](https://github.com/Lautaro-Figueroa)
