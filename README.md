# 🌴 Código Caribe — Landing page

Landing tipo *link-in-bio* para Moisés: asesoría de viajes a Cancún, República Dominicana, Cartagena y Guatemala basada en experiencia real.

**En vivo:** https://covertspecops.github.io/codigo-caribe/

## Funel de ventas

```
Redes sociales (IG / TikTok)
        │
        ▼
   Landing page ──────────────┐
        │                     │
        ▼                     ▼
 CTA WhatsApp (venta)   Travel Planner gratis (captura de lead)
        │                     │
        ▼                     ▼
 Conversación 1-a-1     Guías de Notion (confianza) → WhatsApp
        │
        ▼
 Servicios pagados (planeación, hoteles, tours, renta de carro…)
```

El formulario del final es captura secundaria: si hay correo configurado manda
por [formsubmit.co](https://formsubmit.co); si no, abre WhatsApp con el mensaje
ya escrito.

## Cómo completar la página

Todo se edita en **un solo lugar**: el bloque `CONFIG` al inicio del `<script>`
en `index.html`.

1. **WhatsApp**: poné el número con código de país, solo dígitos → `WHATSAPP: "50688887777"`.
2. **Formulario**: poné el correo de Moisés en `CORREO_FORMULARIO`. El primer
   envío llega con un link de confirmación de formsubmit.co — hay que darle clic
   una vez y listo.
3. **Foto**: guardá la foto en `assets/moises.jpg` y poné `FOTO: "assets/moises.jpg"`.
4. **Links de Notion y redes**: pegá cada URL en `LINKS`. Los que queden en `""`
   muestran un aviso de "próximamente" en vez de un link roto.

## Deploy

GitHub Pages sirve el sitio desde la rama `main` (raíz). Cada `git push` a
`main` publica los cambios en 1–2 minutos. No hay build: es HTML/CSS/JS puro.
