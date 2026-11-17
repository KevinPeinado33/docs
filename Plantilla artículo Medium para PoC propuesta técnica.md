# Plantilla: artículo Medium para PoC / propuesta técnica

Nov 17, 2026 · @Dev Crafters

## Cómo usar esta plantilla

Copia la estructura y reemplaza todo lo que está entre \[corchetes\]. Cada sección trae una guía corta (qué poner y cuánto) y un ejemplo de referencia con una PoC ficticia: **distribuir mini apps en una Super App de React Native con Module Federation**.

- Extensión objetivo: 1,500 a 2,500 palabras (7 a 12 min de lectura).
- Las secciones 2 a 8 son el artículo; la 9 es tu checklist antes de publicar.
- Borra las guías y ejemplos al terminar.

## 1. Título, subtítulo y portada

**Título:** \[Cómo + verbo + resultado concreto + tecnología\]

**Subtítulo:** \[Una línea con el resultado o el gancho\]

**Portada:** \[Diagrama de la arquitectura o captura de la PoC funcionando\]

Guía: el título debe decir qué resolviste, no el tema general. Evita "Explorando..." o "Introducción a...".

Ejemplo:

- Título: *Cómo distribuimos mini apps en React Native sin publicar la app completa*
- Subtítulo: *Una PoC con Module Federation que redujo el ciclo de release de semanas a horas*

## 2. Intro: el problema

&#91;Párrafo 1: el dolor concreto. Qué pasaba, a quién afectaba y con qué frecuencia.\]

&#91;Párrafo 2: por qué importa. Costo en tiempo, dinero, bugs o experiencia del usuario.\]

&#91;Párrafo 3: qué vas a mostrar en el artículo. Una frase.\]

Guía: 2 o 3 párrafos cortos. El lector decide aquí si sigue leyendo.

Ejemplo:

> Cada vez que un equipo quería lanzar un cambio en su módulo, teníamos que publicar toda la app en las tiendas. Con 6 equipos trabajando en paralelo, un release tardaba hasta 3 semanas. En este artículo muestro una PoC que permite actualizar cada mini app por separado.

## 3. Contexto y alternativas evaluadas

&#91;Una frase con los criterios que usaste para decidir.\]

| Opción | Ventaja | Desventaja | ¿La elegimos? |
| --- | --- | --- | --- |
| \[Opción A\] | \[...\] | \[...\] | \[Sí / No\] |
| \[Opción B\] | \[...\] | \[...\] | \[Sí / No\] |
| \[Opción C\] | \[...\] | \[...\] | \[Sí / No\] |

&#91;Un párrafo: por qué elegiste la opción ganadora.\]

Guía: esta sección es la que te da credibilidad. Muestra que no elegiste por moda.

Ejemplo de criterios: *tamaño del bundle, independencia de deploy entre equipos y cumplimiento con las políticas de las tiendas.*

## 4. La propuesta: arquitectura

&#91;Imagen del diagrama de arquitectura\]

&#91;Párrafo que explica el diagrama: los componentes principales y cómo se comunican.\]

- **\[Componente 1\]:** \[qué hace\]
- **\[Componente 2\]:** \[qué hace\]
- **\[Componente 3\]:** \[qué hace\]

Guía: un diagrama vale más que tres párrafos. Hazlo en Excalidraw, draw.io o Mermaid y expórtalo como imagen.

Ejemplo: *Host app (shell) → descarga el manifest remoto → carga cada mini app (Cards, Seguros) como bundle independiente desde un CDN.*

## 5. Implementación paso a paso

### Paso 1: \[Nombre del paso\]

&#91;Qué haces y por qué, en 1 o 2 frases.\]

```ts
// [Snippet corto: solo las líneas que importan]
```

### Paso 2: \[Nombre del paso\]

&#91;Qué haces y por qué.\]

```ts
// [Snippet]
```

### Paso 3: \[Nombre del paso\]

&#91;Qué haces y por qué.\]

```ts
// [Snippet]
```

**Repo completo:** \[link a GitHub\]

Guía: de 3 a 5 pasos. Snippets de 10 a 25 líneas, nunca archivos completos. Después de cada snippet, explica la línea clave.

## 6. Resultados

| Métrica | Antes | Después |
| --- | --- | --- |
| \[Tiempo de release\] | \[...\] | \[...\] |
| \[Tamaño del bundle\] | \[...\] | \[...\] |
| \[Tiempo de carga\] | \[...\] | \[...\] |

&#91;Párrafo: qué funcionó y qué te sorprendió.\]

Guía: si no tienes métricas reales, no las inventes. Cuenta qué validaste (por ejemplo, "se puede actualizar una mini app sin tocar el host") y ponle una captura o GIF.

## 7. Limitaciones y próximos pasos

**Limitaciones:**

- &#91;Dónde se rompe o qué no cubre la PoC\]
- &#91;Riesgos: seguridad, políticas de tiendas, rendimiento\]

**Próximos pasos:**

- &#91;Qué harías para llevarlo a producción\]
- &#91;Qué te falta validar\]

Guía: ser honesto aquí te hace ver más senior. Una PoC sin limitaciones no es creíble.

## 8. Conclusión

&#91;2 o 3 frases: el problema, la solución y el aprendizaje principal.\]

&#91;Llamado a la acción: una pregunta para que comenten, el link al repo o una invitación a seguirte.\]

Ejemplo:

> Module Federation no es una bala de plata, pero para equipos que necesitan independencia de deploy cambia las reglas del juego. ¿Lo has probado en mobile? Te leo en los comentarios.

## 9. Checklist antes de publicar

- [ ] Sin código, nombres internos, URLs ni arquitectura real de la empresa (usa un dominio genérico)
- [ ] Revisado con tu líder o con la política de divulgación de la empresa, si aplica
- [ ] Repo público con README y sin secretos ni API keys
- [ ] Imagen de portada y al menos un diagrama
- [ ] 5 tags elegidos (ej.: React Native, Micro Frontends, Software Architecture, Mobile Development, JavaScript)
- [ ] Leído en voz alta una vez para cortar lo que sobra
- [ ] Enviado a una publicación (ITNEXT, Level Up Coding, Better Programming) o publicado en tu perfil
- [ ] Post en LinkedIn con un resumen de 3 líneas y el diagrama
