# Juridique AI Website - Design Roadmap

## Research Sources (December 2025)

- [SaaS Landing Page Design Best Practices 2025](https://www.designstudiouiux.com/blog/saas-landing-page-design/)
- [Top SaaS Design Trends 2025](https://www.designstudiouiux.com/blog/top-saas-design-trends/)
- [Landing Page Design Trends 2025](https://www.eloqwnt.com/blog/landing-page-design-trends-for-2025-what-drives-conversions-today)
- [UX/UI Design Principles in Legal Tech](https://www.lazarev.agency/articles/legaltech-design)
- [Top UX Strategies for Legal Technology 2025](https://adamfard.com/blog/ux-strategies-for-legal-technology)
- [AstroWind Template](https://github.com/arthelokyo/astrowind)
- [Harvey AI](https://www.harvey.ai) - Legal AI reference
- [Legora](https://legora.com/) - Legal AI workspace reference

---

## Key Design Principles Applied

### 1. Hero Section
- **Clear value proposition**: "Assistance juridique intelligente"
- **Primary CTA**: Direct link to the app
- **Trust signals**: 5 jurisdictions, EU compliance badges
- **No clutter**: Minimal navigation, focused messaging

### 2. Visual Design (2025 Trends)
- **Dark mode with accent colors**: Emerald green (#10b981) as primary
- **Glassmorphism**: Frosted glass effects for cards
- **Subtle gradients**: Background depth without distraction
- **Micro-interactions**: Hover states, smooth transitions

### 3. Legal Tech Specific
- **Trust-first design**: Compliance badges, EU hosting prominently displayed
- **Progressive disclosure**: Show features step by step
- **Professional but accessible**: Legal expertise without intimidation
- **Mobile-first**: Responsive from the start

### 4. Content Strategy
- **Real content only**: Using actual app features, real costs, real URLs
- **French language**: Target audience is francophone
- **No fluff**: Direct, professional communication
- **Transparency**: Showing actual pricing model

---

## Site Structure

```
www/
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── Features.astro
│   │   ├── Modules.astro
│   │   ├── Compliance.astro
│   │   ├── Pricing.astro
│   │   ├── CTA.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── public/
│   └── favicon.svg
└── astro.config.mjs
```

---

## Content (From Real Project)

### Tagline
"Assistance juridique intelligente pour l'Europe"

### Value Proposition
- 5 modules spécialisés (P1-P5)
- 5 juridictions européennes (FR, BE, LU, DE, CH)
- Hébergement 100% européen
- Conformité RGPD et AI Act

### Modules
1. **Analyse de Contrat** - Détecte les risques et clauses problématiques
2. **Création d'Entreprise** - Recommande la meilleure structure juridique
3. **Assistant Juridique** - Répond aux questions en conversation
4. **Correspondance** - Génère des courriers professionnels
5. **Actes de Procédure** - Rédige des documents pour les tribunaux

### Trust Signals
- Hébergé en Europe (Azure Sweden)
- Conforme RGPD
- Conforme AI Act
- Données locales (localStorage)
- Connexion Microsoft sécurisée

### Pricing (Real)
- Infrastructure: ~28€/mois (DEV + PROD)
- Par requête: 0.03€ - 0.15€
- Comparaison: 1000x moins cher qu'un avocat

### URLs
- Production: https://aoli-juridique-prod-frontend.azurewebsites.net
- Dev: https://aoli-juridique-dev-frontend.azurewebsites.net

---

## Implementation Phases

### Phase 1: Core Structure ✓
- [x] Astro project setup
- [x] Tailwind CSS integration
- [x] Design roadmap documentation

### Phase 2: Layout & Components
- [ ] Base layout with dark theme
- [ ] Header with navigation
- [ ] Hero section with CTA
- [ ] Features grid

### Phase 3: Content Sections
- [ ] Modules showcase
- [ ] Compliance/Trust section
- [ ] Pricing transparency
- [ ] Final CTA

### Phase 4: Polish
- [ ] Animations & micro-interactions
- [ ] Mobile optimization
- [ ] Performance optimization
- [ ] SEO meta tags

---

## Color Palette

```css
--primary: #10b981;      /* Emerald - same as app */
--secondary: #3b82f6;    /* Blue */
--accent: #8b5cf6;       /* Purple */
--background: #0f172a;   /* Slate 900 */
--surface: #1e293b;      /* Slate 800 */
--text: #f8fafc;         /* Slate 50 */
--muted: #94a3b8;        /* Slate 400 */
```

---

## Typography

- **Headings**: Inter or system-ui, bold
- **Body**: Inter or system-ui, regular
- **Code/URLs**: JetBrains Mono or monospace

---

## Performance Targets

- Lighthouse Performance: 95+
- Lighthouse Accessibility: 100
- Lighthouse Best Practices: 100
- Lighthouse SEO: 100
- First Contentful Paint: < 1s
- Largest Contentful Paint: < 2s
