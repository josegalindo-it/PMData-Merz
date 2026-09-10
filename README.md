# merz-emea-datapm

Micro-site de propuesta de José Galindo para el rol de Senior Delivery/Program Manager — Customer Data, Analytics & AI (EMEA), cobertura de maternidad de 6 meses (extensible) para Merz, a través de la plataforma freelance Shakers.

- **Publicado en:** GitHub Pages, rama `main`, raíz del repo (`index.html`).
- **Tipo:** `oferta-freelance`.
- **Fuente de contenido:** [`src/SCHEME.md`](src/SCHEME.md) — es el único fichero que se edita a mano. Basado en `MICROSITE_TEMPLATE.en.md` v0.3.
- **Origen:** generado como borrador desde [`src/PROPUESTA_Shakers_EMEA_DataAnalyticsAI_PM.md`](src/PROPUESTA_Shakers_EMEA_DataAnalyticsAI_PM.md) (fuente externa del sistema TOS) mediante `propuesta_to_scheme.py`, y completado a mano.
- **Derivado:** `src/SCHEME.yaml` se genera automáticamente a partir del `.md`. No editar directamente: los cambios se pierden en la siguiente regeneración.
- **Modos de contenido usados:** "Qué aporto" en modo *logros* (4 logros con métrica real). "Arquitectura conceptual" en modo *puntos* (Cadence/Handover/Vendor governance/Boundary) — en el `PROPUESTA` de origen llegó en prosa, sin viñetas; se convirtió a mano al revisar el borrador (ver "Histórico").
- **CV:** [`assets/cv-merz-emea-datapm.pdf`](assets/cv-merz-emea-datapm.pdf), enlazado desde el botón "Download CV" del hero (`botones_hero` → `destino: cv`, resuelto contra `cv_pdf`).
- **URL publicada:** declarada en `url_publicada` dentro de `src/SCHEME.md` (`https://proposals.josegalindo.net/PMData-Merz`).
- **Cliente:** el `PROPUESTA` de origen no nombra al cliente final (solo menciona "Shakers · EMEA Digital Innovation Hub", la plataforma freelance intermediaria) — `cliente_u_organizacion: "Merz"` se rellenó a mano con el dato indicado directamente por Jose al generar este microsite.

## ESTADO: borrador sin revisar (`version_documento: "0.2"`)

Este `SCHEME.md` es un borrador de validación del pipeline, no un entregable listo para enviar. Antes de publicarlo, revisa en `src/SCHEME.md`:

- El H1, la cita del hero y los 4 títulos `###` de sección (Motivation/What I bring/Project/Closing) son sugerencias de posicionamiento, no copy aprobado.
- La lista de puntos de "Arquitectura conceptual" (Cadence/Handover/Vendor governance/Boundary) es una reestructuración a partir de la prosa original del `PROPUESTA` — no cambia el contenido, pero conviene que confirmes que la síntesis en viñetas no pierde matices.
- Sube `version_documento` a `"1.0"` cuando lo apruebes.

## Cómo regenerar el sitio

1. Editar `src/SCHEME.md` (si cambia el contenido, subir `version_documento` y anotar el motivo en su historial interno).
2. Ejecutar, desde el repo `microsite-toolkit`: `python3 build.py <ruta a este proyecto>` — produce `src/SCHEME.yaml` e `index.html`.
3. Revisar `index.html` localmente antes de hacer commit.
4. `git add`, `git commit`, `git push` — GitHub Pages republica automáticamente.

## Histórico

- v0.1 (2026-09-10) — generado como borrador por `propuesta_to_scheme.py`. Esta ejecución sacó a la luz dos huecos reales en el bootstrap (formato de viñetas de logro con guion en vez de dos puntos, y bloques Problem/Solution/Architecture con puntuación distinta a la ya validada en `grouperp-d365-integrationpm`) — corregidos en el toolkit antes de completar este borrador (ver `MICROSITE_SCHEME.md`).
- v0.2 (2026-09-10) — añadidos `cv_pdf`/botón "Download CV" y `url_publicada`; `cliente_u_organizacion` rellenado con "Merz" (dato no presente en el `PROPUESTA` de origen); Arquitectura conceptual convertida a mano de prosa a lista de puntos de gobierno.
