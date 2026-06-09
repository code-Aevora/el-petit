# El Petit — Demo Web · Resum de sessió
**Data:** 8 de juny de 2025  
**Entrega:** 9 de juny de 2025  
**Client:** Carlus (propietari de Can Carlus i El Petit, Tossa de Mar)  
**Responsable:** Alex (Aevora)  
**Director de codi:** Claude  
**Implementació:** Kimi  

---

## Context

Carlus, client existent de Can Carlus, ha demanat una demo de web per al seu altre local: **El Petit**, restaurant situat a les muralles de la Vila Vella de Tossa de Mar. La web actual d'El Petit (elpetitrestaurant.es) està feta amb WordPress + Divi i es veu antiquada. La demo és un lavado de cara amb el nostre stack habitual: HTML/CSS/JS vanilla, un sol arxiu `index.html`.

La web original va ser dissenyada per **Bosco, Estudi Gràfic** — els crèdits NO apareixen a la demo.

---

## Stack i decisions tècniques

- **Stack:** HTML5 / CSS custom properties / JS vanilla — un sol fitxer `index.html`
- **Fonts:** Almarai (300, 400, 700, 800) — Google Fonts
- **Idioma:** Català exclusivament (sense selector d'idiomes)
- **Imatges:** carpeta `/images/` del projecte
- **Carta:** carpeta `/carta/` (pendent de rebre)
- **Desplegament previst:** Vercel (demo) → servidor Contabo + Cloudflare si tanca

---

## Paleta de colors

| Variable | Valor | Ús |
|----------|-------|----|
| `--color-naranja` | `#ea6409` | Accent principal, CTAs, destacats |
| `--color-crema` | `#f2ede4` | Fons seccions clares |
| `--color-pedra` | `#e0d8cc` | Fons seccions intermèdies |
| `--color-fosc` | `#1a1510` | Navbar, hero overlay, seccions fosques |
| `--color-text` | `#2c2419` | Text principal |

---

## Estructura de la web (seccions en ordre)

1. **Navbar** — sticky, logo centrat, links de navegació desktop, blur en scroll
2. **Hero** — carousel infinit tipus roda, 12 fotos, 100vh, overlay fosc, logo gran, subtítol, rating Google, CTA reserva
3. **Tradició** — text esquerra / imatge dreta (`bacalao.jpg`)
4. **Producte** — imatge esquerra / text dreta (`11.jpg`)
5. **Celler** — text esquerra / imatge dreta (`fotos_vinos.jpg`)
6. **La nostra gastronomia** — àlbum fotogràfic tipus llibre, 20 fotos verticals, navegació per click/swipe, fade entre fotos, comptador `X / 20`
7. **El que diuen de nosaltres** — carousel automàtic de ressenyes Google, rating 4,5 · 599
8. **Reserva & Contacte** — secció fusionada en 3 columnes: Horaris / Formulari / Mapa
9. **Footer** — logo, Instagram, TripAdvisor, Google Maps, legal

---

## Fotos Hero (ordre exacte)

1. façana_hero.jpg
2. bacalao.jpg
3. flambejant.jpg
4. interior2.jpg
5. interior1.jpg
6. canelon.jpg
7. vino1.jpg
8. steak_tartar.jpg
9. vino4.jpg
10. steak_tartar3.jpg
11. xupxup.jpg
12. suquet_de_peix.jpg

---

## Fotos Àlbum "La nostra gastronomia" (ordre)

arroz.jpg · arroz_negro.jpg · arroz_pulpo.jpg · arroz_seco2.jpg · bravas.jpg · coca.jpg · vino2.jpg · vino3.jpg · vino5.jpg · croquetas.jpg · ensalada.jpg · fritos.jpg · mejillones.jpg · ostra.jpg · paella.jpg · perrito.jpg · steak_tartar.jpg · tacos_cesar.jpg · tataki_atun.jpg · tiradito.jpg

---

## Dades del local

- **Adreça:** Carrer Portal, 18 · 17320 Tossa de Mar
- **Telèfon:** +34 622 725 043
- **Coordenades mapa:** lat 41.7168142 / lng 2.9324053
- **Instagram:** @elpetit.restaurant
- **TripAdvisor:** enllaç complet inclòs al codi
- **Google Maps:** enllaç complet inclòs al codi
- **Rating Google:** 4,5 ⭐ · 599 ressenyes

## Horaris

| Dia | Horari |
|-----|--------|
| Dilluns | 12:30–16:00 / 19:00–22:00 |
| Dimarts | 12:30–16:00 / 19:00–22:00 |
| Dimecres | **Tancat** |
| Dijous | 12:30–16:00 / 19:00–22:00 |
| Divendres | 12:30–16:00 / 19:00–22:00 |
| Dissabte | 12:30–16:00 / 19:00–22:00 |
| Diumenge | 12:30–16:00 / 19:00–22:00 |

---

## Correccions aplicades durant la sessió

- [x] Overlay hero més fosc i amb gradient vertical
- [x] Autoplay hero allargat de 4s a 6s
- [x] Logo navbar amb refresh al fer click
- [x] Botó WhatsApp sticky — SVG corregit, z-index 99999
- [x] Layout "Producte": imatge esquerra, text dreta
- [x] Àlbum gastronomia: refet com a llibre/àlbum amb fade i comptador
- [x] Horaris + Reserva + Contacte fusionats en una sola secció
- [x] Ressenyes: transició millorada amb translateY + indicador de puntets
- [x] Footer: icona TripAdvisor corregida amb SVG adequat
- [x] Ordre seccions: ressenyes abans que reserva

---

## Pricing previst (pendent de confirmar amb Carlus)

- Pack Base: 350€ + IVA
- **Pack SEO: 450€ + IVA** ← recomanat (la web actual no té schema.org, robots.txt ni res)
- Pack Presència Total: 600€ + IVA
- Pagament: 50% a la signatura, 50% a l'entrega

---

## ⚠️ PENDENTS

### Urgents (entrega: 9 de juny de 2025)

- [ ] **Revisar totes les imatges del carousel Hero** — verificar que es carreguen correctament i que es veuen bé (enquadrament, llum, ordre visual)
- [ ] **Revisar totes les imatges de l'àlbum "La nostra gastronomia"** — verificar que es veuen senceres amb `object-fit: contain`, que les verticals no queden retallades i que el conjunt té coherència visual
- [ ] **Donar-li més personalitat a la web** — les seccions de text/imatge es veuen planes, cal afegir algun element diferenciador (decoració, microdetalls, tipografia més expressiva, etc.) abans de l'entrega
- [ ] Confirmar la data "desde 1989" i handle d'Instagram amb Carlus (per a Can Carlus, però apuntat per coherència)

### Post-entrega / si tanca

- [ ] Rebre i integrar la carta (carpeta `/carta/`)
- [ ] Configurar domini propi
- [ ] Pack SEO: schema.org Restaurant + FAQPage, robots.txt, sitemap.xml, Google Search Console
- [ ] Google Business Profile d'El Petit (optimització)
- [ ] Multiidioma (responsabilitat del soci)
- [ ] Activar backend del formulari de reserva (ara és demo estàtica)

