# Diagramas UML

## Diagrama de Clases

El **Diagrama de Clases** muestra las clases necesarias para el sistema y las relaciones entre ellas. Las principales clases son:

- **Cliente**: Gestiona clientes, incluyendo el registro, modificación, eliminación y consulta de clientes.
- **FacturaCliente**: Gestiona facturas, incluyendo la creación, modificación, eliminación y consulta de facturas.
- **DetalleFactura**: Gestiona los detalles de las facturas, incluyendo agregar, modificar, eliminar y consultar detalles.
- **Producto**: Gestiona productos, incluyendo el registro, modificación, eliminación y consulta de productos.
- **Inventario**: Gestiona inventarios, incluyendo registrar entradas y salidas, modificar, eliminar y consultar inventarios.

![Diagrama de Clases](/Imagenes/clase.png)

## Diagrama de Casos de Uso

El **Diagrama de Casos de Uso** muestra las interacciones entre los usuarios (actores) y el sistema para realizar diferentes tareas. Los casos de uso principales son:

- **Gestión de Clientes**: Registrar, modificar, eliminar y consultar clientes.
- **Gestión de Facturas**: Crear, modificar, eliminar y consultar facturas.
- **Gestión de Detalles de Factura**: Agregar, modificar, eliminar y consultar detalles de facturas.
- **Gestión de Productos**: Registrar, modificar, eliminar y consultar productos.
- **Gestión de Inventario**: Registrar entradas, registrar salidas, modificar, eliminar y consultar inventario.

![Diagrama de Casos de Uso](/Imagenes/casos%20de%20uso.png)

## Diagrama de Secuencia

El **Diagrama de Secuencia** muestra la interacción entre los objetos para un caso de uso específico, como registrar un cliente. Los pasos principales son:

1. **Cliente** envía los datos de registro al **Sistema**.
2. **Sistema** solicita al **ClienteDAO** que guarde los datos.
3. **ClienteDAO** inserta los datos en la **Database**.
4. **Database** confirma la inserción exitosa a **ClienteDAO**.
5. **ClienteDAO** confirma la operación exitosa al **Sistema**.
6. **Sistema** informa al **Cliente** que el registro se ha completado.

![Diagrama de Secuencia](/Imagenes/secuencia.png)
