# Camino hacia mi Centro

> *Un camino para volver a casa, ese hogar sagrado que habita dentro tuyo.*

---

## ✨ Sobre el proyecto
**Camino hacia mi Centro** es una página simple y amorosa que reúne prácticas de bienestar: yoga, respiración, meditaciones, alimentación consciente y una comunidad que acompaña. La estética se inspira en colores pastel y un degradé tipo atardecer.


## 🦋 Estado actual
- Página de acceso con contraseña (se solicita **siempre** al entrar).
- Animación suave de la mariposa del título.
- Secciones base: Inicio, Clases, Alimentación, Meditaciones, Comunidad, Descargables.
- Diseño “glass” con degradés pastel y detalles sutiles.


## 🧩 Estructura (mínima)
```
/
├─ index.html        # Página principal (incluye estilos básicos y script)
├─ style.css         # (opcional) estilos externos si se usan
└─ assets/
   └─ bg.svg         # patrón/ilustración de fondo (opcional)
```

> Nota: En esta versión, todo lo necesario está embebido en `index.html`. Podés mover estilos a `style.css` cuando quieras.


## 🔐 Acceso con contraseña
La contraseña se pide **siempre** al cargar el sitio (no se guarda en el navegador).  
Para cambiarla, editá en `index.html`:

```html
<script>
  document.addEventListener("DOMContentLoaded", () => {
    const PASSWORD = "Asciendetualma333";  // <-- Cambiá acá
    // ...
  });
</script>
```

> Si preferís recordar el acceso por un período (ej. 30 días), se puede reactivar el almacenamiento en `localStorage`.


## 🚀 Despliegue con Vercel + GitHub
1. Hacé commit de tus cambios en el repositorio vinculado a Vercel.
2. Vercel creará automáticamente un **Preview Deployment** para cada rama y producirá un **Production Deployment** al hacer merge/push a `main`.
3. Para reemplazar el `index.html`, subí el archivo y ejecutá:
   ```bash
   git add index.html
   git commit -m "Actualiza acceso con contraseña + animación mariposa"
   git push
   ```

### 💡 Consejos
- Usá ramas para pruebas:
  ```bash
  git checkout -b animacion-mariposa
  git push -u origin animacion-mariposa
  ```
- Revisá la **Preview URL** que te da Vercel antes de publicar.


## 🛠️ Desarrollo local
1. Cloná el repo:  
   ```bash
   git clone <URL_DE_TU_REPO>
   cd <CARPETA_DEL_REPO>
   ```
2. Abrí `index.html` en tu navegador (doble clic o con una extensión de “Live Server” en VS Code).
3. Editá y guardá; al refrescar el navegador vas a ver los cambios.


## 🎨 Personalización rápida
- **Colores y degradé:** editá las variables CSS en `:root` dentro de `index.html` (o en `style.css` si lo usás).
- **Animación de mariposa:** la clase `.butterfly` controla el “revoloteo” (`@keyframes flutter`). Podés ajustar duración o intensidad.
- **Secciones:** agregá o quitá bloques `<section>` según lo que quieras mostrar (videos, PDFs, enlaces a comunidad, etc.).


## ✅ Tecnologías
- **HTML + CSS + JavaScript** (sin frameworks).
- **Vercel** para el hosting con integración **GitHub**.


## 🧪 Checklist de calidad
- [ ] La contraseña funciona y se pide siempre al ingresar.
- [ ] Navegación clara y botones accesibles (teclas y mouse).
- [ ] Texto legible (contraste y tamaño adecuado).
- [ ] Enlaces a recursos (videos, meditaciones, PDFs) actualizados.
- [ ] Imágenes optimizadas para que cargue rápido.


## 📄 Licencia
Proyecto personal. Todo el material (textos, imágenes y estilo) pertenece a su autora.


---

Con amor, **Chechu** 💜🦋✨
