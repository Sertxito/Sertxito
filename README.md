# Sergio Hierro | [Sertxito](https://www.sertxito.es)

**Tecnología con propósito. Personas en el centro.**

Consultor Full Stack en Avanade (Madrid) y Staff Lead de [Tech Riders](https://www.techriders.es/). Más de 10 años entre código, arquitectura y nube, sobre todo con .NET y Azure. Diseño soluciones que operan en producción, mentorizo mientras entrego y hablo de decisiones técnicas que funcionan: menos perseguir lo último, más entender el problema.

---
## 💼 Avanade

**Consultant · Full-Stack Developer | People Lead Ambassador | Early Career Lead | Trainer Counselor**

Diseño arquitectura de soluciones complejas, mentorizo perfiles jóvenes, imparto sesiones de aprendizaje técnico y ayudo a equipos a tomar decisiones que escalen.

---

## 👥 TechRiders — Casa Principal

**Staff Lead** en [TechRiders](https://www.techriders.es/).

**Entre otras cosas, lo que hago:**

- 🎓 Diseño e imparto **Programa Arquitectura Moderna** — aprenden a pensar y diseñar sistemas reales (C4, decisiones arquitectónicas, pasar a código, comunicar por qué)
- 🏫 Mentorizo jóvenes en FP, universidades y Masters.
- 🎤 Sesiones técnicas y Power Skill en eventos.
- 📺 YouTube [@TechRidersMedia](https://www.youtube.com/@TechRidersMedia)
- 🎙️ Podcast TechRiders
- 💻 GitHub [TechRiders-Community](https://github.com/TechRiders-Community)

---

## ⭐ Proyecto estrella: MCP Efficiency Engine (MCPEE)

**[mcp-efficiency-engine](https://github.com/Sertxito/mcp-efficiency-engine)** — arnés de ingeniería *local-first* que convierte cualquier repositorio en un espacio de trabajo gobernado para GitHub Copilot. Con un solo comando Copilot recibe un equipo de especialistas, instrucciones del proyecto, conocimiento local de tu código y documentos, aprobaciones para las acciones de riesgo, validación automática tras cada cambio y un rastro de auditoría completo.

```sh
npm install --global mcp-efficiency-engine
mcpee init --project <ruta>
```

**Cómo funciona el arnés**

| Capa | Qué hace |
|---|---|
| Contexto | Indexa código y documentos en local, construye grafos y envía a Copilot solo extractos citados. |
| Especialistas | Instala agentes, skills, workflows e instrucciones elegidos según tu proyecto. |
| Especificaciones | Extrae propuestas de comportamiento de tu código, o parte de tus requisitos; las aprobadas viven en `specs/approved/`. |
| Permisos | Las herramientas de solo lectura corren libres; transferir contexto y cualquier cambio de estado requieren aprobación (broker MCP + hook `preToolUse`). |
| Verificación | Tras un cambio sincroniza el conocimiento, ejecuta tu validación y solo entonces refresca la documentación. |
| Evidencia | Trazas, aprobaciones y resultados guardados en local, con vistas JSON, OTLP y HTML. |

**Greenfield y brownfield, sin elegir modo.** `mcpee init` inspecciona el proyecto y decide solo:

- **Brownfield** (ya hay código): agentes y guías para tu stack detectado, propuestas de especificación extraídas de tu código y tests, y workflows de validación construidos con tus checks existentes.
- **Greenfield** (carpeta vacía): equipo generalista (orquestador, producto, arquitectura, QA, seguridad, IA y documentación); las especificaciones nacen de los requisitos que escribas, y al reejecutar `init` con código detecta el stack y genera la validación.

Todo queda en tu proyecto y nunca sobrescribe archivos tuyos. Es el motor sobre el que nacieron los boosts, aunque cada boost funciona por su cuenta.

---
## 🚀 Boosts: agentes, skills e instrucciones listos para instalar

Cada **boost** es una pieza **100 % independiente**: lleva sus propios agentes, skills, prompts e instrucciones para GitHub Copilot / VS Code y se **autoinstala** en cualquier proyecto con un único comando, sin MCP ni dependencias externas.

```bash
npx boost-backend      # o cualquier otro boost de la tabla
```

- Cada boost aplica su **prefijo** a lo que instala (`backend-`, `cloud-`, `rag-`...), así que pueden convivir sin colisiones.
- **Nunca sobrescribe**: si un archivo ya existe, lo ignora y avisa (`[WARN] ... IGNORED`).
- Flags: `--check`, `--dry-run`, `--force`, `--uninstall`.
- Copilot detecta agentes, skills y prompts automáticamente tras recargar VS Code.

| Boost | Qué resuelve | Instalar |
|---|---|---|
| [boost_backend](https://github.com/Sertxito/boost_backend) | Patrones de backend moderno: APIs, storage, caching | `npx boost-backend` |
| [boost_frontend](https://github.com/Sertxito/boost_frontend) | Frontend con criterio: accesibilidad, rendimiento, estado | `npx boost-frontend` |
| [boost_design-UX-with-Intent](https://github.com/Sertxito/boost_design-UX-with-Intent) | Diseño UX con intención: componentes, tokens, accesibilidad | `npx boost-uxdesign` |
| [boost_cloud](https://github.com/Sertxito/boost_cloud) | Decisiones de cloud y CI/CD | `npx boost-cloud` |
| [boost_DBA](https://github.com/Sertxito/boost_DBA) | Bases de datos y DBA: modelado, rendimiento, operación | `npx boost-dba` |
| [boost_RAG-Azure](https://github.com/Sertxito/boost_RAG-Azure) | RAG production-ready en Azure: vector search, chunking, AI Search | `npx boost-rag-azure` |
| [boost_azure-iot-edge](https://github.com/Sertxito/boost_azure-iot-edge) | IoT edge-to-cloud en Azure | `npx boost-iot-edge` |
| boost_architect-forensics-expert *(privado)* | Auditoría de arquitecturas: deuda, antipatrones, riesgos | — |

### Demos y otros proyectos

- **[netcoreconf2026](https://github.com/Sertxito/netcoreconf2026)** — Demo de *Tu API ya no la van a consumir personas*: la misma API consumida por REST, por Copilot en VS Code y por herramientas MCP, con Aspire mostrando las peticiones reales (.NET 10).

- **[spec-kit-extension-rag-azure-builder](https://github.com/Sertxito/spec-kit-extension-rag-azure-builder)** — Spec Kit reutilizable para arrancar proyectos RAG.

---
## 🎤 Experiencia Real en Charlas

Hablo de lo que he visto fallar y funcionar. Arquitecturas que escalaron, decisiones que metí la pata, cómo mentorizar sin frenar.

[sessionize.com/sertxito](https://sessionize.com/sertxito/) — catálogo completo de sesiones.

---

## 📚 Donde Estoy

- 🌐 **Web:** [sertxito.es](https://www.sertxito.es)
- **LinkedIn:** [linkedin.com/in/shierroc](https://www.linkedin.com/in/shierroc/)
- **GitHub:** [@Sertxito](https://github.com/Sertxito)
- **X:** [@Sertxito](https://x.com/Sertxito)
- **Instagram:** [@sertxito](https://www.instagram.com/sertxito/)
- **TikTok:** [@sertxito](https://www.tiktok.com/@sertxito)
- **YouTube:** [@sertxito](https://www.youtube.com/@sertxito) · [@TechRidersMedia](https://www.youtube.com/@TechRidersMedia)

---
De estas bases han salido cosas a producción. Seguro que se puede hacer mejor. También seguro que se puede hacer peor.

**#NosPaganPorPensar**
