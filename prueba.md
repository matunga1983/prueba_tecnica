# Evaluación Técnica — Data Engineer SSR

## Esquema de referencia

```
clientes(id_cliente, nombre, ciudad, fecha_registro)
pedidos(id_pedido, id_cliente, fecha_pedido, monto_total, estado)
productos(id_producto, nombre, categoria, precio)
detalle_pedidos(id_pedido, id_producto, cantidad, precio_unitario)
```

---

## Pregunta 1

Listá el `id_pedido`, `fecha_pedido` y `monto_total` de todos los pedidos en estado `'completado'`, ordenados del más reciente al más antiguo.

---

## Pregunta 2

Calculá el monto total facturado por ciudad, considerando solo pedidos `'completado'`. Mostrá `ciudad` y `total_facturado`, ordenado de mayor a menor.

---

## Pregunta 3

Encontrá los productos que se vendieron en más de 50 unidades en total. Mostrá `nombre` del producto, `categoria` y la cantidad total vendida (`unidades_vendidas`), de mayor a menor.

---

## Pregunta 4

Para cada cliente, mostrá sus pedidos `'completado'` con el `id_pedido`, `fecha_pedido`, `monto_total` y un **monto acumulado** (`acumulado`) que sume los montos de ese cliente ordenados por fecha (running total). El resultado debe estar ordenado por cliente y luego por fecha.

---

## Pregunta 5

Escribí una función `contiene(texto, patron)` que devuelva `True` si `patron` aparece como subcadena dentro de `texto`, y `False` en caso contrario. Resolvelo sin usar el operador `in` ni métodos como `.find()` / `.index()`.

Ejemplos:

```
contiene("data engineer", "engine")  -> True
contiene("hola mundo", "mundos")     -> False
contiene("abc", "")                  -> True
contiene("", "a")                    -> False
```
