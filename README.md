# TikTok Analytics Dashboard

Dashboard analítico inspirado en el ecosistema de TikTok, diseñado para mostrar métricas clave de una cuenta de creador de contenido con visualizaciones modernas y una UI pensada para producto real.

Proyecto orientado a portafolio frontend: demuestra capacidades en diseño de dashboards, visualización de datos y microinteracciones.

---

## 🧩 Características principales

- **KPIs clave en tiempo real (mock data)**
  - Followers, Following
  - Likes totales
  - Vídeos publicados
  - Engagement medio
  - Growth de la cuenta
- **Visualizaciones con Chart.js**
  - Gráfico de línea para evolución del engagement.
  - Gráfico doughnut para distribución por tipo de contenido (trends / educativo / lifestyle).
- **Soporte multi–cuenta**
  - Cuenta principal, cuenta de marca/colaboración y cuenta secundaria.
- **Selector de rango temporal**
  - 7, 30 y 90 días, con datasets diferenciados.
- **Top videos recientes**
  - Lista con vistas y CTR estimado por vídeo.
- **Modo claro/oscuro**
  - Toggle de tema con persistencia en `localStorage`.
- **Diseño responsive**
  - Layout tipo dashboard, optimizado para móvil, tablet y desktop.
- **UI/UX**
  - Tarjetas con micro–hover, tipografía limpia y jerarquía visual clara.
  - Badges, chips y pequeños indicadores de crecimiento.

---

## 🛠️ Stack y arquitectura

**Tecnologías:**

- HTML5 semántico.
- CSS3 (sin frameworks).
- JavaScript (ES6+).
- [Chart.js](https://www.chartjs.org/) vía CDN.

**Arquitectura:**

- Single Page Application estática.
- Datos mock definidos en objetos JS segmentados por:
  - Cuenta (`main`, `brand`, `backup`).
  - Rango (`7`, `30`, `90` días).
- Renderizado dinámico de:
  - KPIs.
  - Top videos.
  - Gráficos de Chart.js.
- Gestión de estado simple en memoria:
  - `state.account`, `state.range`, `state.theme`.

---

## 📁 Estructura del proyecto

```txt
tiktok-dashboard/
├── index.html       # HTML principal (incluye CSS y JS o enlace a script/style)
├── style.css        # Estilos (si lo tienes separado)
├── script.js        # Lógica JS (si lo tienes separado)
├── img/
│   └── favicon.png  # Favicon del dashboard
├── LICENSE          # Licencia MIT
└── README.md        # Documentación del proyecto
