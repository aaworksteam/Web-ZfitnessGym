# MEMORY.md — Z Fitness Gym

> Registro de decisiones, cambios y contexto acumulado del proyecto. Actualizar después de cada sesión de trabajo relevante.

---

## 📌 Estado actual del proyecto

- **Versión:** v1.0 (lanzamiento)
- **URL producción:** https://zfitnessgym.netlify.app/
- **Deploy:** Netlify (automático)
- **Última actualización registrada:** Mayo 2026

---

## 🏗️ Historial de decisiones de diseño

### Estructura de archivos
- Se optó por **una sola página** (`index.html`) en lugar de múltiples páginas. Razón: simplicidad de mantenimiento y mejor experiencia de scroll para un landing page de gym.
- Assets en la raíz del proyecto para simplificar las rutas.

### Diseño visual
- **Paleta oscura con acentos de energía** elegida para transmitir seriedad y premium.
- **Video de ambiente** (`video-gym.mp4`) incluido en sección "Así se vive Z Fitness" — refuerza el feeling del lugar sin necesidad de mucho copy.
- **Foto del coach** destacada en sección propia — decisión estratégica porque el owner es la diferenciación principal del gym (no hay instructores rotativos).

### Copy y tono
- Voz directa, en español chileno, sin frases motivacionales genéricas.
- Hero headline: *"Llegas con ganas. Sales con más."* — aprobado por el dueño.
- Sección de reseñas usa Google Reviews reales + testimonios adicionales.

---

## 🔧 Cambios realizados

<!-- Ir completando a medida que se trabaja en el proyecto -->

| Fecha       | Cambio                                    | Archivo afectado | Notas                          |
|-------------|-------------------------------------------|------------------|--------------------------------|
| Mayo 2026   | Creación inicial del sitio                | `index.html`     | Proyecto desde cero            |
| Mayo 2026   | Creación de CLAUDE.md y MEMORY.md         | `/`              | Documentación del proyecto     |

---

## ⚠️ Problemas conocidos / bugs

<!-- Ir documentando issues encontrados -->

| Estado  | Descripción                                              | Prioridad |
|---------|----------------------------------------------------------|-----------|
| Abierto | `index.html` sin separación de CSS/JS en archivos propios | Baja      |
| Abierto | Sin `memory.md` hasta ahora                              | Resuelto  |

---

## 💡 Ideas pendientes / backlog

<!-- Features o mejoras que quedaron fuera del lanzamiento -->

- [ ] Separar CSS en `styles.css` y JS en `main.js` para mejor mantenibilidad
- [ ] Agregar página de confirmación de formulario (actualmente inline)
- [ ] Considerar `sitemap.xml` y `robots.txt` para SEO básico
- [ ] Agregar meta OG tags para compartir en redes sociales con preview
- [ ] Página de política de privacidad (requerida por formularios)
- [ ] Animaciones de entrada (scroll reveal) en secciones de stats y programas
- [ ] Integrar Google Analytics o Plausible para métricas

---

## 📝 Notas de contexto del negocio

- El gym está en **Batuco** — zona periurbana de Santiago. Sirve a clientes de Batuco, Lampa y Liray.
- **Cristian Aballay** es dueño y único coach — esto es una diferenciación clave y debe comunicarse siempre.
- El **estacionamiento gratuito** es un diferenciador mencionado recurrentemente en reseñas — mantener visible.
- Precio de **prueba gratis** es el principal CTA — todos los botones del sitio apuntan ahí.
- El formulario envía por WhatsApp — el flujo de conversión es digital → WhatsApp → presencial.
- Las reseñas de Google tienen rating de **4.7/5 con 37 reseñas verificadas**.

---

## 🔗 Referencias útiles

- [Netlify Dashboard](https://app.netlify.com/) — para ver deploys y logs
- [Google Maps embed](https://www.google.com/maps?q=Z+Fitness+Batuco+Santa+Rosa+Los+Guerreros&output=embed)
- [Instagram del gym](https://instagram.com/zfitness.cl)
- [WhatsApp directo](https://wa.me/56994384312)
- [Perfil de Google Maps](https://maps.app.goo.gl/yyErUuzPCd6cGotVA)

---

*Mantener este archivo actualizado después de cada sesión de trabajo importante.*