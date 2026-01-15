# 🚀 Guía de Inicio Rápido - Proyecto Astro

## Paso 1: Instalar Dependencias

```bash
cd portfolio-astro
npm install
```

## Paso 2: Iniciar el Servidor de Desarrollo

```bash
npm run dev
```

El sitio estará disponible en `http://localhost:4321`

## Paso 3: Personalizar el Proyecto

### Contenido Principal
Edita el archivo `src/pages/index.astro` para personalizar:
- Tu nombre y descripción
- Sección "Sobre Nosotros"
- Proyectos que has realizado
- Información de contacto

### Agregar Nuevos Proyectos
En `src/pages/index.astro`, busca la sección `projects-grid` y agrega más componentes `ProjectCard`:

```astro
<ProjectCard
  title="Nombre del Proyecto"
  description="Descripción breve del proyecto"
  technologies={['React', 'Node.js', 'MongoDB']}
  image="/ruta/a/imagen.jpg"
  link="https://tu-proyecto.com"
/>
```

### Personalizar Colores
Edita las variables CSS en `src/layouts/Layout.astro`:

```css
:root {
  --accent: 136, 58, 234;        /* Color principal */
  --accent-light: 224, 204, 250; /* Color claro */
  --accent-dark: 49, 10, 101;    /* Color oscuro */
}
```

## Paso 4: Agregar Más Páginas

Crea nuevos archivos en `src/pages/`:

### Ejemplo: Página de Blog
```bash
touch src/pages/blog.astro
```

```astro
---
import Layout from '../layouts/Layout.astro';
---

<Layout title="Blog">
  <main>
    <h1>Mi Blog</h1>
    <!-- Contenido del blog -->
  </main>
</Layout>
```

## Paso 5: Construir para Producción

```bash
npm run build
```

Los archivos optimizados estarán en la carpeta `dist/`

## Paso 6: Desplegar

### Opción A: Vercel
1. Crea una cuenta en [Vercel](https://vercel.com)
2. Conecta tu repositorio de GitHub
3. Vercel detectará automáticamente Astro y lo desplegará

### Opción B: Netlify
1. Crea una cuenta en [Netlify](https://netlify.com)
2. Arrastra la carpeta `dist/` a Netlify Drop
3. O conecta tu repositorio para deploy automático

### Opción C: GitHub Pages
```bash
npm run build
# Sube la carpeta dist/ a la rama gh-pages
```

## 🎨 Ideas de Mejora

1. **Agregar un Blog**
   ```bash
   npm install @astrojs/mdx
   npx astro add mdx
   ```

2. **Agregar Tailwind CSS**
   ```bash
   npx astro add tailwind
   ```

3. **Agregar React para Componentes Interactivos**
   ```bash
   npx astro add react
   ```

4. **Agregar un Formulario de Contacto**
   - Usa servicios como Formspree o Netlify Forms

5. **Agregar Animaciones**
   ```bash
   npm install @astrojs/animations
   ```

## 📚 Recursos Útiles

- [Documentación de Astro](https://docs.astro.build)
- [Tutorial Oficial](https://docs.astro.build/en/tutorial/0-introduction/)
- [Temas de Astro](https://astro.build/themes/)
- [Integraciones](https://astro.build/integrations/)

## 🐛 Solución de Problemas

### El servidor no inicia
```bash
# Elimina node_modules e reinstala
rm -rf node_modules package-lock.json
npm install
```

### Errores de TypeScript
```bash
# Verifica la configuración
npm run astro check
```

### El sitio no se ve bien en móvil
- Revisa que las media queries estén correctamente configuradas
- Usa las herramientas de desarrollo del navegador (F12)

## 🤝 Trabajar en Equipo

### Git Workflow Recomendado

1. **Clonar el repositorio**
   ```bash
   git clone <url-del-repo>
   cd portfolio-astro
   ```

2. **Crear una rama para tu feature**
   ```bash
   git checkout -b feature/nombre-feature
   ```

3. **Hacer cambios y commits**
   ```bash
   git add .
   git commit -m "Descripción del cambio"
   ```

4. **Subir cambios**
   ```bash
   git push origin feature/nombre-feature
   ```

5. **Crear Pull Request en GitHub**
   - Ve a GitHub
   - Crea un Pull Request
   - Espera revisión del compañero
   - Merge cuando esté aprobado

### Comunicación

- Usen GitHub Issues para reportar bugs y proponer features
- Usen GitHub Projects para organizar tareas
- Revisen el código mutuamente (Code Reviews)
- Mantengan el README actualizado

## 🎯 Checklist del Proyecto

- [ ] Proyecto instalado y funcionando
- [ ] Contenido personalizado
- [ ] Imágenes agregadas
- [ ] Colores personalizados
- [ ] Al menos 3 proyectos agregados
- [ ] Información de contacto actualizada
- [ ] Sitio responsivo verificado
- [ ] Build de producción exitoso
- [ ] Sitio desplegado online
- [ ] README actualizado con info del proyecto

---

¡Feliz desarrollo! 🎉
