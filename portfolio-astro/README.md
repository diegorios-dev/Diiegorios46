# Portfolio Astro - Proyecto Colaborativo

Un proyecto de portfolio colaborativo construido con [Astro](https://astro.build), diseñado para ser desarrollado por dos programadores trabajando juntos.

## 🚀 Estructura del Proyecto

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── ProjectCard.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

## 🧞 Comandos

Todos los comandos se ejecutan desde la raíz del proyecto, desde la terminal:

| Comando                   | Acción                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Instala las dependencias                         |
| `npm run dev`             | Inicia el servidor de desarrollo en `localhost:4321` |
| `npm run build`           | Construye el sitio de producción en `./dist/`    |
| `npm run preview`         | Previsualiza tu build localmente antes de desplegar |
| `npm run astro ...`       | Ejecuta comandos CLI como `astro add`, `astro check` |
| `npm run astro -- --help` | Obtén ayuda usando el CLI de Astro              |

## 📚 Características

- ✅ **Diseño Moderno**: Interfaz atractiva con degradados y animaciones
- ✅ **Componentes Reutilizables**: ProjectCard para mostrar proyectos
- ✅ **Responsivo**: Se adapta a todos los tamaños de pantalla
- ✅ **SEO Optimizado**: Meta tags y estructura semántica
- ✅ **TypeScript**: Tipado estricto para mejor desarrollo
- ✅ **Rendimiento**: Sitio estático ultra rápido

## 🎨 Secciones Incluidas

1. **Hero Section**: Presentación impactante con llamados a la acción
2. **Sobre Nosotros**: Información sobre el equipo y enfoque
3. **Proyectos**: Galería de proyectos con tarjetas interactivas
4. **Tecnologías**: Stack tecnológico visual
5. **Contacto**: Información de contacto y enlaces
6. **Footer**: Pie de página con información adicional

## 🔧 Próximos Pasos para Personalizar

1. **Actualizar Contenido**: 
   - Edita `src/pages/index.astro` con tu información personal
   - Agrega tus proyectos reales en la sección de proyectos

2. **Agregar Imágenes**:
   - Coloca tus imágenes en la carpeta `public/`
   - Actualiza las rutas en los componentes

3. **Personalizar Estilos**:
   - Modifica los colores en las variables CSS
   - Ajusta los estilos en cada componente

4. **Agregar Más Páginas**:
   - Crea nuevos archivos `.astro` en `src/pages/`
   - Ejemplo: `src/pages/blog.astro`, `src/pages/about.astro`

5. **Integrar React/Vue** (Opcional):
   ```bash
   npx astro add react
   # o
   npx astro add vue
   ```

6. **Agregar Tailwind CSS** (Opcional):
   ```bash
   npx astro add tailwind
   ```

## 📖 Recursos de Aprendizaje

- [Documentación de Astro](https://docs.astro.build)
- [Tutorial de Astro](https://docs.astro.build/en/tutorial/0-introduction/)
- [Discord de Astro](https://astro.build/chat)

## 🤝 Contribución

Este es un proyecto colaborativo. Para trabajar juntos:

1. Crea una rama para tu característica: `git checkout -b feature/nueva-caracteristica`
2. Haz commits de tus cambios: `git commit -m 'Agrega nueva característica'`
3. Push a la rama: `git push origin feature/nueva-caracteristica`
4. Abre un Pull Request para revisión

## 📝 División de Tareas Sugerida

### Desarrollador 1:
- [ ] Diseño y estilos generales
- [ ] Componentes UI (Header, Footer, Cards)
- [ ] Animaciones y transiciones
- [ ] Responsive design

### Desarrollador 2:
- [ ] Configuración del proyecto
- [ ] Sistema de contenido (blog posts, proyectos)
- [ ] SEO y meta tags
- [ ] Optimización y deploy

## 🚀 Deploy

Este proyecto está configurado para desplegarse fácilmente en:

- **Vercel**: Conecta tu repositorio GitHub
- **Netlify**: Deploy automático desde GitHub
- **GitHub Pages**: Ya configurado en `astro.config.mjs`
- **Cloudflare Pages**: Zero configuration

## 📄 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.

---

¡Feliz codificación! 🎉
