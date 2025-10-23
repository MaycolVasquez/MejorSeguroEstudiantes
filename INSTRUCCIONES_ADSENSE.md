# 📢 Instrucciones para Integrar Google AdSense

## 🎯 Espacios de Anuncios Disponibles

Tu página web ya está preparada con **6 espacios estratégicos** para anuncios de Google AdSense:

### 1. **Anuncio Superior** (después del Hero)
- **ID:** `#ad-top`
- **Ubicación:** Justo después de la sección Hero
- **Formato recomendado:** Banner horizontal 728x90 o 970x90
- **Visibilidad:** Alta (primera sección visible)

### 2. **Anuncio después de Riesgos**
- **Clase:** `.ad-horizontal`
- **Ubicación:** Entre "Riesgos" y "Coberturas"
- **Formato recomendado:** Banner horizontal 728x90
- **Visibilidad:** Media-Alta

### 3. **Anuncio después de Coberturas**
- **Clase:** `.ad-horizontal`
- **Ubicación:** Entre "Coberturas" y "Comparativa"
- **Formato recomendado:** Banner horizontal 728x90
- **Visibilidad:** Media

### 4. **Anuncio después de Comparativa**
- **Clase:** `.ad-horizontal`
- **Ubicación:** Entre "Comparativa" y "Consejos"
- **Formato recomendado:** Banner horizontal 728x90
- **Visibilidad:** Media

### 5. **Anuncio Superior de Recomendaciones**
- **ID:** `#ad-bottom`
- **Ubicación:** Antes de la sección de Recomendaciones
- **Formato recomendado:** Cuadrado 336x280 o Banner 728x90
- **Visibilidad:** Alta

### 6. **Anuncio Inferior**
- **ID:** `#ad-bottom`
- **Ubicación:** Después de Recomendaciones, antes del Footer
- **Formato recomendado:** Banner horizontal 728x90
- **Visibilidad:** Media

## 📝 Cómo Agregar los Códigos de AdSense

### Paso 1: Obtén tu código de AdSense
1. Inicia sesión en tu cuenta de Google AdSense
2. Ve a "Anuncios" → "Por unidad de anuncios"
3. Crea una nueva unidad de anuncio
4. Copia el código generado

### Paso 2: Reemplaza el placeholder
Busca en `index.html` las secciones con comentarios como:
```html
<!-- Google AdSense - Anuncio Superior (728x90 o 970x90) -->
<!-- Reemplazar con código de AdSense aquí -->
<p class="ad-label">Publicidad</p>
```

Reemplázalas con tu código de AdSense:
```html
<!-- Google AdSense - Anuncio Superior -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-XXXXXXXXXX"
     data-ad-slot="XXXXXXXXXX"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
```

### Paso 3: Elimina el texto "Publicidad"
Una vez agregues el código real de AdSense, elimina la línea:
```html
<p class="ad-label">Publicidad</p>
```

## 🎨 Formatos Recomendados por Ubicación

### Espacios Horizontales (entre secciones)
- **728x90** - Leaderboard (Desktop)
- **320x50** - Banner móvil (Mobile)
- **Responsive** - Se adapta automáticamente

### Espacio Superior/Inferior
- **970x90** - Large Leaderboard (Desktop grande)
- **728x90** - Leaderboard (Desktop)
- **336x280** - Large Rectangle (Alternativa)
- **Responsive** - Recomendado

## ✅ Checklist antes de Aplicar a AdSense

Antes de solicitar la aprobación de Google AdSense, asegúrate de:

- [ ] Tu sitio está publicado en un dominio propio (no localhost)
- [ ] Tienes al menos 20-30 páginas de contenido original
- [ ] El contenido cumple con las políticas de AdSense
- [ ] Tienes páginas de:
  - [ ] Política de Privacidad
  - [ ] Términos de Uso
  - [ ] Sobre Nosotros/Contacto
- [ ] El sitio es responsive y funciona en móviles
- [ ] No hay enlaces rotos
- [ ] El contenido es original (no copiado)

## 🚀 Optimización de AdSense

### Mejores Prácticas

1. **No satures de anuncios**
   - Usa máximo 3-4 anuncios por página
   - Ya tienes 6 espacios, puedes empezar con 3-4

2. **Usa anuncios responsive**
   - Se adaptan mejor a todos los dispositivos
   - Mejor experiencia de usuario

3. **Coloca anuncios estratégicamente**
   - Los espacios actuales ya están optimizados
   - Primera mitad de la página = mejor rendimiento

4. **Experimenta con formatos**
   - Prueba diferentes tamaños
   - Analiza métricas en AdSense

5. **Contenido de calidad**
   - Más tráfico = más ingresos
   - Contenido relevante = anuncios relevantes

## 📊 Métricas a Monitorear

Una vez integrado AdSense, revisa:

- **CTR** (Click-Through Rate) - Tasa de clics
- **CPC** (Cost Per Click) - Costo por clic
- **RPM** (Revenue Per Mille) - Ingresos por 1000 impresiones
- **Cobertura** - % de solicitudes con anuncios

### Objetivos razonables:
- CTR: 1-3%
- CPC: $0.20-$2.00 (varía por nicho)
- RPM: $3-$10 (inicial)

## 🔧 Ajustes CSS (si necesario)

Los estilos ya están optimizados, pero puedes ajustar:

```css
/* En styles.css, busca .ad-placeholder */
.ad-placeholder {
    /* Ajusta altura según tu anuncio */
    min-height: 90px; /* Para 728x90 */
    /* min-height: 280px; */ /* Para 336x280 */
}
```

## 🌐 Antes de Publicar

1. **Sube tu sitio a un hosting**
   - Netlify, Vercel, GitHub Pages (gratuitos)
   - Hostinger, Bluehost, etc. (pagos)

2. **Configura un dominio**
   - Necesario para AdSense
   - Ejemplo: www.seguroestudiantesguia.com

3. **Aplica a AdSense**
   - Ve a: https://www.google.com/adsense
   - Completa la solicitud
   - Espera aprobación (7-14 días)

4. **Agrega los códigos**
   - Una vez aprobado, agrega los códigos
   - Los anuncios aparecerán en 24-48 horas

## 📱 Testing Responsive

Antes de publicar, verifica que los anuncios se vean bien en:
- 📱 Móviles (< 480px)
- 📱 Tablets (481px - 768px)
- 💻 Desktop (> 768px)

## ⚠️ Políticas Importantes de AdSense

**NO hagas:**
- ❌ Click en tus propios anuncios
- ❌ Pedir a otros que hagan click
- ❌ Colocar anuncios en pop-ups
- ❌ Modificar el código de AdSense
- ❌ Contenido inapropiado/ilegal

**SÍ haz:**
- ✅ Contenido original y de calidad
- ✅ Tráfico orgánico legítimo
- ✅ Cumple todas las políticas
- ✅ Diseño responsive
- ✅ Buena experiencia de usuario

## 🆘 Soporte

Si tienes problemas:
1. Centro de ayuda de AdSense: https://support.google.com/adsense
2. Foro de la comunidad de AdSense
3. Verifica tu correo (notificaciones de Google)

## 📈 Próximos Pasos

1. ✅ Tu página ya está lista (informativa)
2. ⏳ Sube a hosting con dominio
3. ⏳ Aplica a Google AdSense
4. ⏳ Espera aprobación
5. ⏳ Agrega códigos de anuncios
6. ⏳ Monitorea y optimiza

---

**Última actualización:** Octubre 2025

**Nota:** Esta página ya está 100% optimizada para AdSense con espacios estratégicos y contenido informativo de calidad. ¡Solo falta agregar los códigos una vez aprueban tu cuenta!

© 2025 EstudiaSeguro - Guía de Integración AdSense