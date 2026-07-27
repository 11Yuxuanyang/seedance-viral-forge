# Seedance Viral Forge

Habilidades de prompts de video con IA reutilizables para creadores que necesitan guiones de videos cortos en chino que puedan copiarse en Seedance 2.0 y publicarse rápidamente.

Seedance Viral Forge es un repositorio de guiones de video con IA orientado a 即梦 / Seedance 2.0. El enfoque no es "escribir prompts bonitos", sino producir guiones en chino que puedan generar, publicar y testear datos directamente.

## Qué hace este proyecto

Este repositorio ayuda a los usuarios a generar guiones estructurados de video con IA en chino para tres tareas reales de videos cortos:

- videos de venta de productos
- videos de baile para generación de leads de comercios
- videos de tráfico basados en tendencias

En lugar de tratar la escritura de prompts como una inspiración vaga, este repositorio la convierte en habilidades reutilizables con entradas claras, flujos predeterminados, formatos de salida y límites de seguridad.

## Por qué es importante

La mayoría de las colecciones de prompts de video con IA fallan en producción por las mismas razones:

- producen redacciones elegantes en lugar de guiones utilizables
- no solicitan los insumos mínimos faltantes
- mezclan la salida de chat predeterminada con la escritura automática de archivos
- ignoran cómo Seedance maneja la memoria, el detalle físico y la continuidad del movimiento

Este repositorio está diseñado para lo contrario. Prioriza los guiones directos a la generación, valores predeterminados conservadores y el comportamiento repetible del operador.

## Qué obtienes

| Parte | Qué hace |
|------|---------------|
| `skills/通用场景/SKILL.md` | Genera guiones de venta de productos para flujos de trabajo de Douyin / 即梦 |
| `skills/跳舞/SKILL.md` | Genera guiones de baile para leads de comercios basados en la atracción de escena + personaje |
| `skills/热梗/SKILL.md` | Genera prompts de tráfico basados en tendencias para clips virales cortos |
| `shared/SEEDANCE_BASELINE.md` | Reglas de producción compartidas para las tres habilidades |
| `docs/` | Páginas de aterrizaje en GitHub Pages para búsqueda y descubrimiento de IA |
| `archive/` | Borradores antiguos y material no apto para producción |

## Inicio rápido

### 1. Elige la habilidad adecuada

- Venta de productos: [`skills/通用场景/SKILL.md`](./skills/通用场景/SKILL.md)
- Tráfico de escenas comerciales: [`skills/跳舞/SKILL.md`](./skills/跳舞/SKILL.md)
- Tráfico de tendencias: [`skills/热梗/SKILL.md`](./skills/热梗/SKILL.md)

### 2. Proporciona la entrada mínima utilizable

Para `通用场景`:

- nombre del producto
- categoría
- 1-3 puntos de venta
- idealmente, cómo se ve y cómo se utiliza

Para `跳舞`:

- tipo de comercio
- la parte más filmable del local
- qué vende la oferta / paquete

Para `热梗`:

- una tendencia específica
- o simplemente `/热梗` y deja que la habilidad proponga direcciones

### 3. Sigue el flujo predeterminado

1. La habilidad extrae lo que falta.
2. Devuelve 3 tarjetas de dirección.
3. El usuario elige A, B, C, o solicita todas.
4. La habilidad entrega el guion final en chino.

## Casos de Uso

### Cómo generar guiones de video de productos para Seedance 2.0 en chino

Usa [`skills/通用场景/SKILL.md`](./skills/通用场景/SKILL.md) cuando necesites guiones cortos de venta de productos con una revelación clara, lógica de tomas simple y ubicación natural del CTA.

### Cómo crear prompts de promoción de baile comercial para 即梦

Usa [`skills/跳舞/SKILL.md`](./skills/跳舞/SKILL.md) cuando el objetivo sea la generación de leads locales: captar la atención con la energía del personaje y luego dirigir a los espectadores hacia el local o la oferta.

### Cómo convertir tendencias actuales en prompts de video corto con IA

Usa [`skills/热梗/SKILL.md`](./skills/热梗/SKILL.md) cuando quieras guiones priorizando el tráfico, basados en temas candentes, absurdidad visual y patrones virales probados.

### Cómo diseñar habilidades reutilizables para flujos de trabajo de prompts de video con IA

Usa [`shared/SEEDANCE_BASELINE.md`](./shared/SEEDANCE_BASELINE.md) junto con las tres habilidades de producción para estudiar cómo el trabajo de prompts puede estructurarse en protocolos operativos reutilizables en lugar de volcados de prompts aislados.

## Principios Fundamentales

- Primero que sea copiable en Seedance
- Salida de producción exclusivamente en chino
- Pedir el detalle mínimo faltante, no un formulario de entrada gigante
- Priorizar la salida de conversación, no la escritura de archivos
- Repetir detalles físicos porque el modelo no recuerda de forma fiable
- Preferir un solo plano o muy pocos cambios de escena

## Documentación

- Inicio de docs: `https://11yuxuanyang.github.io/seedance-viral-forge/`
- Cómo escribir prompts de venta de productos de Seedance: [`docs/seedance-product-video-prompts.html`](./docs/seedance-product-video-prompts.html)
- Cómo hacer videos de baile comercial de 即梦: [`docs/jimeng-merchant-dance-video-scripts.html`](./docs/jimeng-merchant-dance-video-scripts.html)
- Cómo hacer videos cortos de IA basados en tendencias: [`docs/ai-trend-video-prompts.html`](./docs/ai-trend-video-prompts.html)
- Cómo este repositorio estructura habilidades de video con IA reutilizables: [`docs/reusable-ai-video-skill-design.html`](./docs/reusable-ai-video-skill-design.html)

## Historial de Estrellas

[![Star History Chart](https://api.star-history.com/svg?repos=11Yuxuanyang/seedance-viral-forge&type=Date)](https://www.star-history.com/#11Yuxuanyang/seedance-viral-forge&Date)

## Estructura del Repositorio

```text
ai-video/
├── README.md
├── AGENTS.md
├── llms.txt
├── CITATION.cff
├── CLAUDE.md
├── shared/
│   └── SEEDANCE_BASELINE.md
├── docs/
│   ├── index.html
│   ├── styles.css
│   ├── llms.txt
│   ├── robots.txt
│   ├── sitemap.xml
│   └── plans/
├── skills/
│   ├── 通用场景/
│   │   └── SKILL.md
│   ├── 跳舞/
│   │   └── SKILL.md
│   └── 热梗/
│       └── SKILL.md
└── archive/
```

## Mejores Puntos de Entrada

- [`README.md`](./README.md)
- [`AGENTS.md`](./AGENTS.md)
- [`llms.txt`](./llms.txt)
- [`shared/SEEDANCE_BASELINE.md`](./shared/SEEDANCE_BASELINE.md)
- [`skills/通用场景/SKILL.md`](./skills/通用场景/SKILL.md)
- [`skills/跳舞/SKILL.md`](./skills/跳舞/SKILL.md)
- [`skills/热梗/SKILL.md`](./skills/热梗/SKILL.md)

## Palabras Clave que cubre este Repositorio

- Seedance 2.0 prompts
- 即梦提示词
- AI video script skills
- Chinese short-video prompts
- Douyin AI product video script
- merchant dance promo prompt
- viral trend AI video prompt
- reusable `SKILL.md` design

## Licencia

MIT. Ver [LICENSE](./LICENSE).
