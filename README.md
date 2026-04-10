# La Vuelta a México en 80 Tacos

Landing page para presentar el proyecto a socios potenciales.

**Live:** https://vuelta-mexico-80-tacos.vercel.app
**Repo:** https://github.com/tacotios-wq/vuelta-mexico-80-tacos

---

## Stack

- Single-file HTML (`index.html`) — sin frameworks, sin dependencias
- CSS custom properties (design tokens)
- Vanilla JS (IntersectionObserver, counters animados, video modal)
- Helvetica Neue como unica tipografia
- Deploy: Vercel (auto-deploy desde `npx vercel --prod`)

## Estructura del proyecto

```
deploy/
  index.html          ← TODO el codigo (CSS + HTML + JS en un archivo)
  abrazo.jpg           ← Foto: Aniol abrazando a una cocinera (og:image)
  aniol-comal.jpg      ← Foto: Aniol cocinando en comal
  aniol-telefono.jpg   ← Foto: Aniol con telefono (no usada actualmente)
  dona-comal.jpg       ← Foto: Dona cocinando (story Araceli)
  dona-retrato.jpg     ← Foto: Retrato dona (no usada actualmente)
  mexico-magico.mp4    ← Video hero background (NO en git, solo en Vercel)
  vercel.json          ← Config de deploy
```

## Videos (Google Drive)

Los videos de las historias se cargan desde Google Drive via iframe embed:

| Historia | Drive ID |
|----------|----------|
| Araceli | `141Jo13Y6IdcMQ-AegLhif3JrGRQLtsee` |
| Los Kumiai | `16PQll0Ocob9UeHgDSA_gOnzXp1p5vAm0` |
| Dona Humo | `19NiME9oaEYngkx-xq7eIL4Dkcup78_8x` |
| Dona Esthela | `1XNSWJA7MM6BPMepeyh8jcX04B6GFBLjv` |
| Mexico Magico (final) | `1uI0GPAKezLE2xlZW8JVDyeM8CSTB3s3Y` |

Formato embed: `https://drive.google.com/file/d/{ID}/preview`

**Importante:** Los videos de Drive deben tener permisos de "Cualquier persona con el enlace puede ver" para que el embed funcione.

## Secciones de la landing (en orden de scroll)

1. **Hero** — Hook paradoja + frase Mexico
2. **Counter** — 2,100,000 personas
3. **El filtro** — Quote nietos (two-col)
4. **Las dos monedas** — Asociacion + Atencion
5. **Foto abrazo** — Full-width pattern break
6. **Audiencia** — Grid datos (720K IG, 670K FB, 620K TT, 90K YT) + engagement + views
7. **Historias** — Araceli featured + 3 compact, cada una con video modal
8. **Micro-CTA** — "Si esto ya resuena..."
9. **Foto Aniol comal** — Full-width pattern break
10. **El sistema** — 3 escalones con links a sub-proyectos
11. **La ventana** — Counter 64 dias + Mundial FIFA 2026
12. **El equipo** — 8 roles con nombres reales
13. **Calendario** — 4 fechas (abril 14 → junio 11)
14. **Finale** — Video Mexico Magico (vertical) + "Vamos por tacos? Tengo hambre."

## Links a sub-proyectos

- Guia Espanoles: https://guia-espanoles.vercel.app
- La Seleccion del Taco: https://la-seleccion-del-taco.vercel.app

## Pendientes para quien continue

- [ ] Datos de geolocalizacion de audiencia (% Mexico, USA, LATAM)
- [ ] Mejorar calidad de fotos (las actuales son capturas)
- [ ] Foto dona-retrato.jpg y aniol-telefono.jpg no estan en uso — evaluar si integrar
- [ ] Testing en dispositivo movil real (iPhone + Android)
- [ ] Verificar que los videos de Drive cargan correctamente (permisos)
- [ ] Video mexico-magico.mp4 no esta en git (24MB) — solo en Vercel

## Design tokens

```css
--bg: #ffffff
--bg-alt: #f5f5f7
--text: #1d1d1f        (negro Apple)
--text-secondary: #6e6e73
--text-tertiary: #86868b
--line: rgba(0,0,0,0.08)
--link: #06c            (azul Apple)
--font: 'Helvetica Neue', Helvetica, Arial, sans-serif
```

## Deploy

```bash
cd deploy
npx vercel --prod
```

## Principios de diseno (NO negociables)

1. **Helvetica** — unica tipografia. Nunca otra.
2. **Fondo blanco** — los silencios pesan mas que las palabras.
3. **Informacion justa** — si puedes quitarlo sin perder sentido, quitalo.
4. **Nunca decir "pitch"** — es "proyecto" o simplemente el nombre.
5. **Fotos rompen el Apple** — solo en 2 momentos, como contraste deliberado.
6. **Mobile first** — el ejecutivo lo abre en WhatsApp.
