# Ketzalli Labs — README (Org)

**Slogan:** _Inclusión que se transforma con tecnología._  
**Color primario:** `#0039A6`

## ¿Quiénes somos?
Ketzalli Labs es una organización dentro del ecosistema del Tec de Monterrey dedicada a crear soluciones tecnológicas para la inclusión lingüística en México, con enfoque principal en el **Lenguaje de Señas Mexicana (LSM)**. Combinamos investigación aplicada, diseño centrado en las personas y herramientas de vanguardia para acercar educación, accesibilidad y comunicación a todas y todos.

## Misión
**Impulsar la inclusión en México** desarrollando productos digitales que faciliten el aprendizaje, la práctica y la adopción de la LSM, conectando comunidades oyentes y sordas **mediante tecnología significativa y responsable**.

## Visión
Ser la **referencia nacional** en plataformas de aprendizaje y traducción de LSM, integrando academia, industria y sociedad civil para lograr **un México sin barreras de comunicación**, exportando buenas prácticas a Latinoamérica.

## Principios y valores
- **Humanismo tecnológico:** la persona primero; la tecnología como puente.  
- **Diseño inclusivo:** accesible, usable, medible y co-creado con la comunidad sorda.  
- **Rigor académico:** métricas de aprendizaje, validación con evidencia y ética de datos.  
- **Orgullo mexicano:** identidad y patrimonio lingüístico como motor de innovación.  
- **Colaboración abierta:** estándares, APIs y conocimiento compartido cuando sea posible.

---

## Producto Inicial (MVP): App para reforzar LSM
**Objetivo:** facilitar el estudio autónomo de LSM y ofrecer analítica educativa para docentes y administradores.

**Funcionalidades clave del MVP**
- Registro / inicio de sesión y acceso como invitado.  
- Diccionario de señas por categorías con **videos** por cada seña.  
- **Búsqueda** de palabras o frases.  
- **Actividades y quizzes** interactivos.  
- **Progreso**: guardado y visualización del avance.  
- **Vista de administrador** (panel web o en la app) para ver progreso de usuarios.

**Posibles funcionalidades “extra” (backlog)**
- Favoritos y listas personalizadas.  
- Modo práctica con cámara (básico) para validar duración/movimiento.  
- Retos diarios/semanales; logros/insignias; flashcards.  
- Estadísticas avanzadas y compartir progreso.  
- Audio opcional, **modo examen**, retroalimentación lúdica y mini-juego de memoria.

**Dashboard del administrador (backlog)**
- Gestión de contenidos (señas, videos y categorías).  
- Gestión de quizzes.  
- Reportes de progreso exportables (PDF/Excel).  
- Estadísticas de uso (accesos, videos más vistos, quizzes).

---

## Enfoque técnico (sugerido)
- **Frontend móvil:** Flutter (iOS/Android) o React Native.  
- **Web admin:** React + Vite.  
- **Backend:** Node.js (NestJS) o Python (FastAPI).  
- **Base de datos:** Postgres.  
- **Almacenamiento de video:** S3-compatible con CDN.  
- **Analítica:** eventos encolados (Kafka/Redpanda) + Superset/Metabase.  
- **ML (futuro):** evaluación de señas con visión por computadora (on-device + cloud).  
- **Accesibilidad:** WCAG 2.2, captions, alto contraste, navegación por gestos.  
- **Seguridad y privacidad:** OAuth2/OIDC, RBAC, cifrado en tránsito y reposo, gobernanza de datos.

---

## Resultados esperados
- Incremento medible de dominio por categoría (tasa de aciertos en quizzes).  
- Adherencia/retención semanal de estudio.  
- Reducción de tiempo para encontrar y aprender una seña específica.  
- Satisfacción de usuarios (NPS) y adopción por docentes/comunidades.

---

## Roadmap (alto nivel)
1. **MVP (0–3 meses):** diccionario con video, cuentas, búsqueda, quizzes y progreso; tablero básico.  
2. **Aprendizaje asistido (3–6 meses):** retos, logros, flashcards y exportes admin.  
3. **Práctica guiada (6–9 meses):** modo cámara básico y modo examen.  
4. **Inteligencia aplicada (9–12 meses):** analítica avanzada, recomendaciones y piloto de evaluación automática de señas.

---

## Estructura de repos/organización (sugerida)
```
ketzalli-labs/
  README.md
  apps/
    mobile/          # Flutter/React Native
    admin-web/       # React
  services/
    api/             # NestJS/FastAPI
    worker/          # colas, jobs, notificaciones
  packages/
    ui/              # componentes compartidos
    sdk/             # cliente TS/Flutter para API
  infra/
    terraform/       # IaC
    k8s/             # despliegues
  docs/
    product/         # MRD/PRD, user stories
    design/          # UX, flujos, accesibilidad
    research/        # validación con comunidad LSM
```
---

## Contribución
1. Haz fork y crea una rama: `feat/tu-feature`.  
2. Sigue el _styleguide_ (lint, tests, accesibilidad).  
3. Pull Request con descripción, criterios de aceptación y capturas.  
4. Revisión por pares y checklist de accesibilidad/seguridad.  

> Consulta `docs/product/` y `docs/design/` antes de proponer cambios que afecten UX o currículo LSM.

## Código de Conducta
Esperamos un trato respetuoso, lenguaje inclusivo y colaboración empática con la comunidad sorda. Cero tolerancia a discriminación o acoso. (Ver `CODE_OF_CONDUCT.md`).

## Licencia
Definir según estrategia (ej. **AGPL** para servicios + **CC BY-NC** para contenidos didácticos). Evitar licenciar videos sin autorización explícita.

## Contacto
- **Ketzalli Labs** — Tec de Monterrey  
- Correo: contacto@ketzallilabs.mx (placeholder)  
- Sitio: https://ketzallilabs.mx (placeholder)
