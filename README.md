# ¿Cómo afecta `<!DOCTYPE html>` en un documento HTML?

El `DOCTYPE` le indica al navegador que debe interpretar el documento HTML en **Modo Estándar**. Si no se incluye, algunos navegadores podrían activar el **Modo Quirks**, que usa una compatibilidad antigua con versiones de HTML previas.

---

## 1. Comparación de HTML con y sin `DOCTYPE`

### ✅ **Con `<!DOCTYPE html>` (Modo Estándar)**
```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Prueba de DOCTYPE</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        img {
            width: 300px;
        }
        p {
            width: 50%;
        }
    </style>
</head>
<body>
    <h1>Probando el DOCTYPE</h1>
    <p>Este es un párrafo dentro de un documento HTML.</p>
    <img src="https://via.placeholder.com/300" alt="Imagen de prueba">
</body>
</html>
```

### ❌ **Sin `<!DOCTYPE html>` (Modo Quirks)**
```html
<html>
<head>
    <meta charset="UTF-8">
    <title>Prueba sin DOCTYPE</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        img {
            width: 300px;
        }
        p {
            width: 50%;
        }
    </style>
</head>
<body>
    <h1>Probando el DOCTYPE</h1>
    <p>Este es un párrafo dentro de un documento HTML.</p>
    <img src="https://via.placeholder.com/300" alt="Imagen de prueba">
</body>
</html>
```

---

## 2. ¿Cómo verificar el modo de renderización?

1. **Abrir la herramienta de inspección del navegador**
   - En **Chrome o Firefox**, presiona `F12` o `Ctrl + Shift + I`.
   - Ve a la pestaña **Console (Consola)** o **Elements (Elementos)**.
   - Busca si el navegador está en **"Quirks Mode"** o **"Standards Mode"**.

2. **Comparar los cambios visuales**
   - En **Modo Quirks**, podrías notar diferencias como:
     - Diferente manejo de **márgenes y paddings**.
     - Imágenes mostrándose con **dimensiones incorrectas**.
     - **Diseño roto** en navegadores antiguos.

---

## 3. Conclusión
- **Usar `<!DOCTYPE html>`** garantiza que el navegador interprete el HTML correctamente en **Modo Estándar**.
- **Si lo omites**, el navegador podría usar **Modo Quirks**, lo que podría generar inconsistencias en CSS y diseño.
- Puedes verificarlo con las herramientas de inspección (`F12`).

🔍 **Realiza la prueba en tu navegador y observa las diferencias.** 🚀

