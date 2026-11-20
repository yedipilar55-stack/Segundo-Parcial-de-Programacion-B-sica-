# Cafetería "El Buen Sabor" - Pedidos

## 1. Datos del estudiante
- Nombre: Maria Pilar Vessania Silvence Yedi
- Matrícula: 2025-3481
- Profesor: Gamalier del Carmen
- Asignatura: Programación Básica - Segundo Parcial

## 2. Descripción del programa
Aplicación de escritorio en C# (Windows Forms) con un solo formulario, frmPedidos, que registra los pedidos de la cafetería y calcula el total a pagar. Permite agregar varios productos a una lista, aplicar descuento a clientes frecuentes, cobrar el empaque para llevar y calcular el ITBIS.

## 3. Datos de entrada
- Cliente (txtCliente) y si es cliente frecuente (chkFrecuente)
- Fecha (dtpFecha)
- Producto (txtProducto) y precio (txtPrecio)
- Cantidad de 1 a 20 (nudCantidad)
- Tamaño: Normal o Grande, +RD$25 (rbtNormal, rbtGrande)
- Servicio: Consumir en local o Para llevar, +RD$20 (rbtLocal, rbtLlevar)
- Porción extra, +RD$30 (chkPorcionExtra)

## 4. Proceso
1. Agregar al pedido: se validan los datos. Precio unitario = precio + 25 si es grande + 30 si lleva porción extra. Total de la línea = precio unitario x cantidad. La línea se muestra en la lista y se suma al subtotal.
2. Calcular total: descuento = 10 % del subtotal si es cliente frecuente. Empaque = RD$20 una sola vez si es para llevar. Base imponible = subtotal - descuento + empaque. ITBIS = 18 % de la base. Total = base + ITBIS. Si no hay productos, muestra un mensaje y no calcula.
3. Nuevo pedido: limpia todos los campos, la lista y los totales.
4. Salir: pide confirmación con MessageBox (Sí/No) antes de cerrar.

## 5. Salida
Subtotal, descuento, empaque, ITBIS y total a pagar, con formato RD$ 0.00.

Caso de prueba: María Pérez (frecuente); Sándwich 180 grande x2 = 410; Jugo 120 con porción extra x1 = 150; para llevar.

| Concepto | Valor |
|---|---|
| Subtotal | RD$ 560.00 |
| Descuento | RD$ 56.00 |
| Empaque | RD$ 20.00 |
| Base imponible | RD$ 524.00 |
| ITBIS | RD$ 94.32 |
| Total a pagar | RD$ 618.32 |

## 6. Capturas de pantalla
Captura del programa en ejecución adjunta en
