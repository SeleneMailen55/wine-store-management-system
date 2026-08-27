# Viñesta – Sistema de Gestión y Tienda Online de Vinos y Tours

Sistema web full-stack desarrollado en **ASP.NET MVC** que combina una tienda online de venta de vinos con reserva de tours, y un panel de administración para la gestión completa del negocio (productos, stock, proveedores, compras y ventas).

## Descripción

Viñesta es una aplicación web pensada para una bodega/vinoteca de Mendoza, Argentina. Permite a los clientes navegar el catálogo de vinos, agregar productos al carrito, realizar compras y reservar tours por las bodegas. Del lado administrativo, cuenta con un sistema de gestión para controlar productos, categorías, proveedores, stock y el historial de ventas.

## Funcionalidades

### Tienda (cliente)
- Catálogo de productos con filtro por categoría
- Carrito de compras
- Registro e inicio de sesión de usuarios
- Historial de compras del cliente
- Formulario de reserva de tours
- Formulario de contacto

### Panel de gestión (administrador)
- ABM de productos, categorías, proveedores y stock
- Gestión de compras a proveedores
- Control de ventas y pedidos de clientes
- Roles diferenciados (usuario común / administrador)

## Tecnologías utilizadas

- **Backend:** ASP.NET MVC (C#)
- **Base de datos:** SQL Server
- **Frontend:** HTML5, CSS3, Bootstrap 4/5, jQuery
- **Librerías adicionales:** DataTables, SweetAlert2, Owl Carousel
- **Otros:** LINQ, ADO.NET (SqlClient)

## Cómo ejecutar el proyecto localmente

### Requisitos previos
- Visual Studio 2019 o superior
- SQL Server (Express o superior)
- .NET Framework 4.7.2 o superior

### Pasos

1. Cloná el repositorio:
```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
```

2. Restaurá la base de datos:
   - Abrí SQL Server Management Studio (SSMS)
   - Restaurá el archivo `.bak` incluido en la carpeta `/Database` (o ejecutá los scripts `.sql` de creación de tablas)

3. Configurá la cadena de conexión:
   - Abrí `Web.config` (o `Web.config.example` como referencia)
   - Actualizá el valor de `connectionString` con el nombre de tu servidor SQL local:
```xml
     <add name="CN" connectionString="SERVER=TU_SERVIDOR;DATABASE=DB_CARRITO;Integrated Security=True;TrustServerCertificate=True" />
```

4. Abrí el proyecto en Visual Studio y ejecutalo con **F5**.

## Estructura del proyecto
ProyectoTest/
├── Controllers/ # Controladores MVC
├── Views/ # Vistas Razor (.cshtml)
├── Logica/ # Capa de lógica de negocio y acceso a datos
├── Models/ # Modelos de datos
├── Content/ # CSS y estilos
├── Scripts/ # Scripts JS (jQuery, DataTables, etc.)
├── assets/ # Imágenes y recursos del template
└── Database/ # Scripts / backup de la base de datos

## Créditos

El diseño visual del sitio está basado en el template **Fruitkha**, creado por [Imran Hossain](https://imransdesign.com/), adaptado e integrado sobre una aplicación ASP.NET MVC con backend y base de datos propios.

## Licencia

Este proyecto fue desarrollado con fines educativos.

## Autor

**Bustamante Selene Mailen**
