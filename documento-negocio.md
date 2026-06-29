# Documento de Negocio — PROPIO

> Documento fuente para Notebook LM. Cada sección `##` es una diapositiva.
> Incluye pricing, contratos, infraestructura web, hosting, y modelo de negocio completo.

---

## Diapositiva 1 — Portada

**PROPIO**
Infraestructura digital propia para tu barbería

Modelo de negocio · Pricing · Infraestructura · Crecimiento

---

## Diapositiva 2 — El problema de mercado

**Las barberías dependen de intermediarios que:**

- Cobran cuota mensual fija (Booksy ~42€/mes)
- Cobran comisiones (hasta 30%) por clientes nuevos captados vía Boost
- Retienen los datos de los clientes en su plataforma
- Muestran a la competencia al lado del perfil del barbero
- El barbero no tiene control sobre su propia base de clientes

**El coste real para un barbero con Booksy:**

Cuota fija mensual + comisiones por cliente nuevo = hasta 150-200€/mes reales

_Nota visual: Gráfico comparativo de coste Booksy vs PROPIO. Una barra alta (Booksy con comisiones) vs una barra baja (PROPIO, solo cuota fija)._

---

## Diapositiva 3 — Nuestra solución: PROPIO

**PROPIO es el sistema de gestión de citas propio de la barbería.**

| Función | Beneficio |
|---------|-----------|
| Web propia con dominio | El barbero tiene su presencia digital independiente |
| Reservas online 24/7 | Los clientes reservan sin llamar, sin intermediarios |
| CRM con historial de clientes | Cada visita queda registrada, datos siempre disponibles |
| Panel de gestión profesional | Agenda, ingresos, clientes, estadísticas |
| Recordatorios automáticos | Reducción de ausencias |
| Detección de clientes inactivos | Recuperación de clientes que no vuelven |
| **0% comisiones** | El 100% del valor del servicio se queda en el negocio |

_Nota visual: Iconos de cada funcionalidad en grid. Todos en verde o grafito. Limpio, profesional._

---

## Diapositiva 4 — Planes de precios

| | Basic | Growth | Premium |
|---|---|---|---|
| **Precio** | 29€/mes | 49€/mes | 79€/mes |
| **Web propia** | Plantilla básica | Personalizada + dominio propio | Personalizada premium |
| **Reservas online** | ✅ | ✅ | ✅ |
| **CRM clientes** | ✅ | ✅ completo | ✅ completo |
| **Agenda** | ✅ | ✅ | ✅ |
| **Recordatorios** | ✅ | ✅ | ✅ |
| **Dominio propio** | ❌ | ✅ Incluido | ✅ Incluido |
| **Panel avanzado** | ❌ | ✅ | ✅ |
| **Métricas** | ❌ | Básicas | Avanzadas |
| **WhatsApp IA** | ❌ | ❌ | ✅ (próximamente) |
| **Multi-sede / equipo** | ❌ | ❌ | ✅ |
| **Soporte** | Email | Email prioritario | Prioritario + WhatsApp |

**Setup / Migración:** 149€ (una vez) — GRATIS para Plan Fundadores.

_Nota visual: 3 columnas lado a lado. Columna Growth destacada con borde verde y badge "Recomendado"._

---

## Diapositiva 5 — Plan Fundadores

**3 plazas exclusivas para los primeros clientes.**

| Beneficio | Detalle |
|-----------|---------|
| **Setup** | GRATIS (149€ ahorrados) |
| **Migración desde Booksy** | GRATIS (nosotros la hacemos) |
| **Precio** | Congelado de por vida |
| **Permanencia** | Sin permanencia. Cancela cuando quieras |
| **Soporte** | Directo con el fundador |

**Estado actual:**
- Plaza 1: Ocupada (Luis - Salón de Caballeros)
- Plaza 2: Disponible
- Plaza 3: Disponible

_Nota visual: Fondo oscuro (grafito), texto blanco. Badge "3 plazas" con punto verde. Urgencia pero sin presión._

---

## Diapositiva 6 — Contratos: modelo de compromiso

**Dos opciones para el cliente:**

| | Sin permanencia | Con compromiso |
|---|---|---|
| **Cuota mensual** | 49€/mes | 49€/mes |
| **Setup / Migración** | 149€ (una vez) | 0€ (gratis) |
| **Compromiso mínimo** | No hay | 6 meses |
| **Si cancela antes** | — | Paga el setup (149€) |
| **¿Para quién?** | Cliente que quiere probar | Cliente que ya confía |

**Plan Fundadores:** Sin permanencia + setup gratis. Siempre.

**Lógica del modelo:**
- El setup cubre el coste de migración y configuración
- El compromiso de 6 meses incentiva a quedarse sin penalizar
- Nadie se va al mes "por probar" sin haber pagado algo

_Nota visual: Tabla de 2 columnas. Opción B ligeramente destacada (es la que conviene al barbero y a ti)._

---

## Diapositiva 7 — Infraestructura web: cómo alojamos cada barbería

| Componente | Dónde se aloja | Coste |
|------------|----------------|-------|
| **Web del barbero** (landing, booking) | **Vercel** (gratis) | 0€ |
| **API / Backend** | **VPS Hostinger** (tu actual) | ~10€/mes (ya lo pagas) |
| **Base de datos** | **PostgreSQL** en el mismo VPS | Incluido |
| **Dominio del barbero** | DonDominio / Namecheap | ~12€/año (lo paga él) |
| **Automatizaciones (n8n)** | Mismo VPS | Incluido |

**Ventajas de Vercel para las webs de los barberos:**
- HTTPS/SSL automático y gratis
- CDN global (carga más rápido)
- Dominio personalizado gratis
- Sin mantenimiento
- Sin límite de sitios (gratis)

**Cada barbero tiene:**
- Su dominio (ej: `tubarberia.es`) apuntando a Vercel → su web
- Reservas y panel conectados a tu API en el VPS
- Sin coste adicional para ti por cada cliente nuevo

_Nota visual: Diagrama de arquitectura simple: Cliente → Vercel (web) → Tu VPS (API + BD). 3 cajas conectadas con flechas._

---

## Diapositiva 8 — Modelo de costes y márgenes

| Concepto | Coste | Clientes necesarios para cubrirlo |
|----------|-------|----------------------------------|
| **VPS Hostinger** | ~10€/mes | 1 cliente (49€) |
| **Dominios** | 12€/año c/u (paga el cliente) | 0€ |
| **Vercel** | 0€ | — |
| **n8n** | 0€ (self-hosted) | — |
| **WhatsApp API** | ~0-5€/mes (según uso) | Próximamente |
| **Total costes fijos** | ~10-15€/mes | — |

**Margen por cliente:**

| Plan | Precio | Coste por cliente | Margen |
|------|--------|-------------------|--------|
| Basic | 29€/mes | ~0,30€ | **~99%** |
| Growth | 49€/mes | ~0,30€ | **~99%** |
| Premium | 79€/mes | ~0,30€ | **~99%** |

**Proyección de ingresos:**

| Clientes | MRR | Costes | Beneficio mensual |
|----------|-----|--------|-------------------|
| 5 | ~245€ | ~15€ | **~230€** |
| 10 | ~490€ | ~15€ | **~475€** |
| 20 | ~980€ | ~20€ | **~960€** |
| 30 | ~1.470€ | ~25€ | **~1.445€** |

_Nota visual: Tabla de proyección con 4 columnas. La fila de 10 clientes destacada por ser el primer objetivo realista._

---

## Diapositiva 9 — La web como reemplazo de la ficha de Booksy

**Cuando un barbero deja Booksy, pierde su ficha de perfil pública.**

PROPIO le ofrece una web profesional que reemplaza esa ficha:

| Elemento de Booksy | Reemplazo en PROPIO |
|--------------------|---------------------|
| Perfil con fotos del local | Web completa (fotos, servicios, horario) |
| Catálogo de servicios | Servicios con precios visibles |
| Botón "Reservar cita" | Botón directo al sistema de reservas |
| Enlace para compartir | Dominio propio (tubarberia.es) |
| Reseñas | Enlace a Google Reviews |

**Cómo se entrega:**

Clonar el template de `salon-de-caballeros.html`, cambiar:
- Nombre del barbero y barbería
- Fotos (local, barbero, trabajos)
- Servicios y precios
- Enlace de reserva

**Tiempo estimado:** 30-45 minutos por cliente.

**Incluido en:** Plan Growth (49€/mes) y Premium (79€/mes).

_Nota visual: Antes (ficha de Booksy genérica) → Después (web propia profesional con dominio). Comparación visual lado a lado._

---

## Diapositiva 10 — Roadmap: próximos 60 días

| Semana | Hito | Responsable |
|--------|------|-------------|
| **Semana 1** | Primer cliente en vivo (Luis) | Diego |
| **Semana 2** | Landing publicada en Vercel + caso real | Diego + Agentes |
| **Semana 3** | Instagram activo + 1er reel | Diego + Growth Marketing |
| **Semana 4** | n8n desplegado en VPS + WhatsApp automation | Diego + Agentes |
| **Semana 5** | Segundo cliente onboarded | Diego + Ventas |
| **Semana 6** | Plan Fundadores completo (3 plazas) | Diego + Ventas |
| **Semana 7** | Precios ajustados para nuevos clientes (sin Fundadores) | Diego + Estratega |
| **Semana 8** | Stripe + facturación automática | Diego + Agentes |

_Nota visual: Timeline horizontal con 8 mojones. Los primeros 4 en verde (ya en marcha), los siguientes en grafito._

---

## Diapositiva 11 — Proyección a 6 meses

| Mes | Clientes | MRR | Estado del negocio |
|-----|----------|-----|-------------------|
| **Mes 1** | 1-2 | ~49-98€ | Validación |
| **Mes 2** | 3-5 | ~147-245€ | Plan Fundadores completo |
| **Mes 3** | 5-8 | ~245-392€ | Estabilidad |
| **Mes 4** | 8-12 | ~392-588€ | Crecimiento |
| **Mes 5** | 12-18 | ~588-882€ | Expansión |
| **Mes 6** | 18-25 | ~882-1.225€ | Consolidación |

**Hitos clave en el camino:**
- 3 clientes → valida el modelo de negocio
- 10 clientes → ingresos suficientes para cubrir costes + tiempo
- 20 clientes → negocio escalado, solo supervisión

_Nota visual: Gráfico de escalera ascendente. Mes 1-3 pendiente suave, mes 4-6 más pronunciada (efecto recomendación)._

---

## Diapositiva 12 — Cierre: el modelo en una frase

**PROPIO gana cuando el barbero gana.**

Sin comisiones. Sin permanencia. Sin letra pequeña.
Infraestructura digital propia para cada barbería.

3 plazas Fundadores disponibles.
La próxima barbería en entrar mantiene su precio para siempre.

**propio.app**

_Nota visual: Logo grande centrado. Tagline. Mismo estilo que portada, limpio y profesional._
