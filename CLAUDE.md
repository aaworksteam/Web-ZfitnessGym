# CLAUDE.md — Z Fitness Gym

> Guía de contexto para Claude Code. Léela completa antes de tocar cualquier archivo.

---

## 🏋️ ¿Qué es este proyecto?

Landing page de **Z Fitness**, un gimnasio premium ubicado en **Batuco, Chile** (Santa Rosa con Los Guerreros, al lado de la iglesia de piedra). Sitio web de una sola página (`index.html`) desplegado en **Vercel** → [zfitnessgym.vercel.app](https://zfitnessgym.vercel.app).

El sitio fue creado por **AA Works** (Alonso Aballay) → 

---

## 🗂️ Estructura del proyecto

```
/
├── index.html          ← Toda la UI vive acá (HTML + CSS + JS inline o en tags)
├── logo.webp           ← Logo principal del gym
├── video-gym.mp4       ← Video de ambiente del gym (sección "Así se vive Z Fitness")
├── fotos/
│   └── zfit-coach.png  ← Foto de Cristian Aballay (coach y dueño)
└── CLAUDE.md           ← Este archivo
```

> ⚠️ **index.html es largo.** Antes de editar, identifica la sección exacta usando los comentarios HTML o los IDs de las secciones. No reescribas bloques que no necesitas tocar.

---

## 🧭 Secciones del sitio (IDs de navegación)

| ID / Anchor     | Contenido                                              |
|-----------------|--------------------------------------------------------|
| `#top`          | Navbar + Hero                                          |
| `#programas`    | Cards de programas (Hyrox, CrossFit, GAP, etc.)        |
| `#horario`      | Tabla/grilla de horario semanal                        |
| `#planes`       | Pricing cards + tabla multimensual                     |
| `#equipo`       | Sección del coach Cristian Aballay                     |
| `#faq`          | Preguntas frecuentes (accordion)                       |
| `#contacto`     | Formulario + mapa + datos de contacto                  |

---

## 🎨 Identidad visual y diseño

- **Estética:** Premium, dark, moderno. Gym serio con personalidad cercana.
- **Tipografía:** Sans-serif de alto contraste — no cambiar sin consenso.
- **Paleta:** Oscura con acentos de energía (confirmar valores exactos en el CSS del `index.html`).
- **Tono de copy:** Directo, sin adornos, en español chileno. Evitar frases genéricas de gym ("sé la mejor versión de ti mismo"). El copy actual tiene identidad — respetarla.
- **Logo:** `logo.webp` — no escalar distorsionado, siempre mantener ratio.

---

## 🏟️ Programas que ofrece el gym

### Clases grupales
- **Hyrox** — Fitness híbrido: running + estaciones de fuerza/resistencia
- **CrossFit** — Funcional de alta intensidad con coach certificado
- **GAP** — Glúteos, Abdomen y Piernas
- **Levantamiento** — Halterofilia olímpica (Clean & Jerk, Snatch)

### Servicios individuales
- **Bodybuilding** — Hipertrofia con método científico
- **Personal Trainer** — 1 a 1 con coach, plan personalizado
- **Nutricionista** — Asesoría nutricional integrada al entrenamiento

---

## 📅 Horario de clases

| Día       | Horario apertura          | Clases destacadas                        |
|-----------|---------------------------|------------------------------------------|
| Lunes     | 07:00–13:00 / 16:00–22:00 | CF Metcon (08:30, 19:30, 20:30) + GAP (18:30) |
| Martes    | 07:00–13:00 / 16:00–22:00 | Hyrox (18:30) + Levantamiento (19:30)    |
| Miércoles | 07:00–13:00 / 16:00–22:00 | CF Gymnastics (08:30, 19:30, 20:30) + GAP (18:30) |
| Jueves    | 07:00–13:00 / 16:00–22:00 | Hyrox (18:30) + Levantamiento (19:30)    |
| Viernes   | 07:00–13:00 / 16:00–22:00 | Levantamiento (08:30, 19:30) + GAP (18:30) |
| Sábado    | 09:00–14:00               | Open gym (09:00)                         |
| Domingo   | Cerrado                   | —                                        |

---

## 💰 Tarifas actuales

> Todos los precios en CLP y con IVA incluido. Matrícula anual: **$20.000**.

| Plan              | Precio mensual | Notas                                      |
|-------------------|----------------|--------------------------------------------|
| Solo Máquinas     | $35.000        | Sala ilimitada · Dupla: $60.000           |
| 12 Clases         | $48.000        | + sala libre · Dupla: $90.000             |
| 24 Clases         | $58.000        | Mejor valor por clase · + sala libre       |
| Pase diario       | $7.000         | Sin mensualidad                            |

| Multimensual Solo Máquinas | Precio        |
|----------------------------|---------------|
| 3 meses                    | $96.000       |
| 6 meses                    | $164.000      |
| 12 meses                   | $290.000      |

| Multimensual 12 Clases     | Precio        |
|----------------------------|---------------|
| 3 meses                    | $130.000      |
| 6 meses                    | $230.000      |
| 12 meses                   | $420.000      |

---

## 👤 El coach

**Cristian Aballay** — Fundador y Head Coach. Dueño del gym. Es el único instructor (sin rotativos). Especialidades: Hyrox, CrossFit, Fuerza, Bodybuilding. Foto en `/fotos/zfit-coach.png`.

> Nunca referirse a "instructores" en plural — hay un solo coach.

---

## 📞 Datos de contacto

- **WhatsApp:** +56 9 9438 4312
- **Instagram:** [@zfitness.cl](https://instagram.com/zfitness.cl)
- **Email:** hola@zfitness.cl
- **Dirección:** Santa Rosa con Los Guerreros, Batuco — costado iglesia de piedra, al lado de Empanadas Erick
- **Google Maps embed:** `https://www.google.com/maps?q=Z+Fitness+Batuco+Santa+Rosa+Los+Guerreros&output=embed`

---

## ⚙️ Stack técnico

- **Frontend:** HTML + CSS + JS vanilla (todo en `index.html`)
- **Deploy:** Vercel (automático desde GitHub — push a main despliega)
- **Sin frameworks:** No hay React, Vue, ni bundlers
- **Sin backend:** El formulario de contacto redirige a WhatsApp (no usa Netlify Forms)
- **Assets:** `.webp` para imágenes (optimizado), `.mp4` para video, `.png` para foto del coach

---

## 📏 Reglas de desarrollo

1. **No refactorizar sin pedirlo.** Si hay que editar una sección, edita solo esa sección.
2. **Mantener el HTML semántico.** Usar las etiquetas correctas (`<section>`, `<nav>`, `<article>`, etc.).
3. **Mobile-first.** El sitio debe verse perfecto en móvil. Confirmar breakpoints antes de tocar media queries.
4. **Performance primero.** Las imágenes ya están en `.webp`. No agregar imágenes sin optimizar.
5. **No cambiar precios ni copy de ventas** sin confirmación explícita del dueño. Son datos de negocio reales.
6. **Los IDs de secciones son contratos.** El `#horario`, `#planes`, etc. están linkeados en el nav — no renombrar sin actualizar todas las referencias.
7. **Deploy en Vercel.** Cualquier cambio en `index.html` se despliega al hacer push a GitHub (rama `main`). Probar localmente antes.
8. **El formulario tiene honeypot.** El campo "No llenar" es anti-spam — no borrarlo.

---

## 🚧 Deuda técnica conocida

- `index.html` es muy largo y no está modularizado (sin componentes, sin includes).          (ver `MEMORY.md` adjunto).
- Posiblemente sin separación de CSS en archivo externo.

> Si se va a refactorizar el HTML en múltiples archivos, hacerlo con cuidado: Vercel sirve archivos estáticos igual que Netlify para este proyecto, no hay server-side rendering.

---

## ✅ Checklist antes de cada cambio

- [ ] ¿Afecta mobile o solo desktop?
- [ ] ¿Cambia algún ID o anchor del nav?
- [ ] ¿Modifica precios, horarios o copy real del negocio?
- [ ] ¿Agrega dependencias externas (CDN, scripts)?
- [ ] ¿Funciona el formulario de contacto después del cambio?

---

*Última actualización del CLAUDE.md: junio 2026 — migrado de Netlify a Vercel*