# Infraestructura Web — PROPIO

> Cómo alojamos la web de cada barbería. Documento técnico para implementación.

---

## Esquema general

```
Cliente (navegador)
        │
        ▼
  ┌─────────────────────┐
  │   VERCEL (GRATIS)   │  ← Web del barbero (HTML estático)
  │   tubarberia.es     │
  │   HTTPS automático  │
  └─────────┬───────────┘
            │
            ▼
  ┌─────────────────────┐
  │   TU VPS (10€/mes)  │  ← API + BD (compartido para todos)
  │   api.propio.app    │
  │   FastAPI + Postgres│
  └─────────────────────┘
```

## Paso a paso para cada barbero nuevo

### 1. Comprar el dominio
- Proveedor: DonDominio, Namecheap, o el que prefieras
- Coste: ~12€/año
- ¿Quién paga? El cliente (tú lo gestionas)

### 2. Configurar dominio en Vercel
- Desde el panel de Vercel: Add Domain → `tubarberia.es`
- Vercel te da los DNS a configurar (CNAME)
- HTTPS se activa solo automáticamente

### 3. Crear la web del barbero
- Clonar `salon-de-caballeros.html` como template
- Cambiar: nombre, fotos, servicios, precios, enlace de reserva
- Subir a Vercel (mismo proyecto o proyecto separado)
- Tiempo estimado: 30-45 minutos

### 4. Configurar el booking
- El booking (demo.html del barbero) apunta a tu API en el VPS
- Cada barbero tiene su propia URL de booking
- La web del barbero redirige a esa URL de booking

## Ejemplo práctico: Luis

```
Web:    https://salondecaballeros.es → Vercel
Booking: https://codigodecaballeros.site → VPS (API)
Admin:   https://codigodecaballeros.site/admin.html → VPS (frontend estático servido por nginx)
```

## Notas

- Vercel no tiene límite de sitios en el plan gratuito
- Cada dominio nuevo en Vercel es 100% gratis
- El backend en tu VPS soporta todos los clientes sin cambios
- Si el barbero quiere darse de baja, el dominio se puede redirigir o cancelar
