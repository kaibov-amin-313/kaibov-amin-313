<picture>
  <source media="(prefers-color-scheme: dark)" srcset="header-dark.svg">
  <img alt="Amin Kaibov — full-stack engineer, Almaty" src="header-light.svg" width="800">
</picture>

### Selected work

**BASHIR&CO** — luxury sourcing brand. Six-page cinematic SPA.
The problem worth solving was motion continuity: GSAP timelines that survive route
changes without leaking, so moving through the site reads as one camera move rather
than six separate pages.
`TypeScript` `Next.js` `GSAP` `Tailwind`

**AUA** — hyperlocal air quality for Almaty.
Official monitoring stations leave wide blind zones between them. The platform
interpolates coverage across the gaps, flags readings that disagree with the nearest
official post, and answers the one question a parent actually asks: can my kid go
outside right now.
`React` `TypeScript` `Leaflet` `Vite`

<details>
<summary>How the blind-zone estimate works</summary>

Readings from Kazhydromet, IQAir, air.org.kz and one local station are combined by
inverse-distance weighting, so every point on the map gets a value with a confidence
that falls off with distance from the nearest real sensor. Anywhere past the distance
threshold is drawn as a blind zone rather than quietly filled in. A z-score check
against the official post surfaces the disagreements instead of averaging them away.

It is an indicator, not a medical device, and the interface says so.
</details>

**Ahlul al-Bayt** — multilingual educational platform.
Prayer times, duas, ziyarat, audio lectures, Q&A. The hard part is typographic:
Russian, Arabic and Persian sharing one layout, each set correctly, RTL included.
`Next.js` `PostgreSQL` `Prisma`

### How I work

Architecture before implementation. The expensive mistakes are made before the first
line of code.

Motion has to earn its place. If an animation doesn't help you understand what just
happened, it comes out.

One considered screen beats five rough ones. I would rather ship less and have it hold up.

Code should still make sense in six months, to someone who isn't me.

### Colophon

Portrait rendered as ASCII, 46 columns, from a single photograph.
Set in the system monospace stack throughout.
Built by hand. Revised 2026.07.

---

[github.com/kaibov-amin-313](https://github.com/kaibov-amin-313)
