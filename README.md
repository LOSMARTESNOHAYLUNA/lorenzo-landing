# Landing Lorenzo Arquitectura — Estudios de arquitectura

Landing page estática orientada a estudios de arquitectura e interiorismo. CTA principal: reservar reunión técnica. CTA secundario: descargar guía.

## Estructura

```
lorenzo-landing/
├── index.html              # Página principal
├── vercel.json             # Configuración de Vercel (caché de assets)
├── assets/
│   └── logo-lorenzo.png    # Logo oficial
└── README.md
```

## Despliegue en Vercel

### Opción 1 — Subida directa (la más rápida)

1. Entra en https://vercel.com/new
2. Arrastra la carpeta `lorenzo-landing` completa (o el ZIP descomprimido) a la zona de subida
3. Vercel detecta automáticamente que es un sitio estático
4. Pulsa **Deploy**

En 30-60 segundos la landing estará online en una URL tipo `lorenzo-landing-xxx.vercel.app`.

### Opción 2 — Desde GitHub

1. Crea un repositorio en GitHub y sube estos archivos manteniendo la estructura
2. En Vercel, **Add New > Project > Import Git Repository**
3. Selecciona el repo y pulsa **Deploy**

Cada commit al repo despliega automáticamente una nueva versión.

## Dominio personalizado

Una vez desplegado, en el panel del proyecto en Vercel:

1. **Settings > Domains**
2. Añadir el dominio deseado (ej. `estudios.lorenzoarquitectura.com`)
3. Vercel da las instrucciones DNS para configurar en el proveedor del dominio

## Pendiente antes de publicar en producción

- [ ] Conectar el envío de los formularios a un backend/CRM (actualmente simulado en frontend, ver comentarios en el `<script>` de `index.html`)
- [ ] Sustituir la imagen de fondo del hero (actualmente Unsplash como placeholder) por una imagen definitiva
- [ ] Revisar enlaces de "políticas legales y de privacidad" (actualmente `#`)
- [ ] Confirmar direcciones de Madrid y Toledo en el footer
- [ ] Añadir scripts de analítica (Google Analytics, Plausible o similar)
