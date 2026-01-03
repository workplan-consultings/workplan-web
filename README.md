# WorkPlan - Sitio Web

## Instrucciones para subir a GitHub Pages

### Paso 1: Crear cuenta en GitHub (si no tenés)
1. Andá a https://github.com
2. Hacé clic en "Sign up"
3. Completá el registro con tu email

### Paso 2: Crear un repositorio nuevo
1. Una vez logueada, hacé clic en el botón verde "New" o "+" en la esquina superior derecha
2. Nombre del repositorio: `workplan-web` (o el nombre que prefieras)
3. Dejalo como "Public"
4. NO marques ninguna opción adicional (ni README, ni .gitignore, ni license)
5. Hacé clic en "Create repository"

### Paso 3: Subir los archivos
1. En la página del repositorio vacío, vas a ver la opción "uploading an existing file"
2. Hacé clic ahí
3. Arrastrá TODA la carpeta `workplan-web` o seleccioná todos los archivos:
   - index.html
   - La carpeta `assets` completa (con la subcarpeta `images`)
4. Abajo escribí un mensaje como "Primer commit - sitio web WorkPlan"
5. Hacé clic en "Commit changes"

### Paso 4: Activar GitHub Pages
1. En tu repositorio, andá a "Settings" (pestaña de arriba)
2. En el menú de la izquierda, buscá "Pages"
3. En "Source", seleccioná:
   - Branch: `main`
   - Folder: `/ (root)`
4. Hacé clic en "Save"
5. Esperá 2-3 minutos y refrescá la página
6. Va a aparecer un link: `https://tu-usuario.github.io/workplan-web/`

### Paso 5: Conectar tu dominio workplan.com.ar
1. En la misma sección "Pages" de GitHub, hay un campo "Custom domain"
2. Escribí: `www.workplan.com.ar`
3. Hacé clic en "Save"

4. Ahora andá a tu panel de NIC Argentina (donde tenés el dominio)
5. Buscá la sección de DNS o "Delegar dominio"
6. Agregá estos registros:

**Opción A - Si podés agregar registros A:**
```
Tipo: A
Host: @
Valor: 185.199.108.153

Tipo: A
Host: @
Valor: 185.199.109.153

Tipo: A
Host: @
Valor: 185.199.110.153

Tipo: A
Host: @
Valor: 185.199.111.153

Tipo: CNAME
Host: www
Valor: tu-usuario.github.io
```

**Opción B - Si solo podés agregar CNAME:**
```
Tipo: CNAME
Host: www
Valor: tu-usuario.github.io
```

7. Esperá entre 24-48 horas para que los DNS se propaguen
8. Una vez funcionando, volvé a GitHub Pages y marcá "Enforce HTTPS"

---

## Estructura de archivos

```
workplan-web/
├── index.html          (página principal)
├── README.md           (este archivo)
└── assets/
    └── images/
        ├── Workplan_sin_fondo.png
        ├── Lorena_Palma_Fuente_5.png
        └── Gestion_de_Talento__2_.jpg
```

## Funcionalidades incluidas

- ✅ Diseño responsive (se adapta a celulares y tablets)
- ✅ Formulario de contacto funcional (usa FormSubmit.co - gratuito)
- ✅ Formulario de carga de CV
- ✅ Política de Privacidad (Ley 25.326 Argentina)
- ✅ Términos y Condiciones
- ✅ Animaciones suaves
- ✅ Menú móvil
- ✅ SEO básico

## Para editar contenido

El archivo `index.html` contiene todo el sitio. Podés editarlo con cualquier editor de texto (Notepad++, VS Code, o incluso el Bloc de notas).

- Para cambiar textos: buscá el texto que querés cambiar y reemplazalo
- Para cambiar imágenes: subí la nueva imagen a `assets/images/` y cambiá el nombre en el código
- Para agregar testimonios: buscá la sección "testimonios" y reemplazá los placeholders

## Soporte

Los formularios envían los datos a: workplan.consultings@gmail.com

Si necesitás ayuda técnica, contactame.

---
Desarrollado para WorkPlan - Gestión de Talento
Enero 2025
