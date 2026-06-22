# Entregable · Sesión 3 — Copilotos IA

- **Nombre / usuario: Diego Ruiz Vintimilla / diegojavinti@gmail.com**
- **Fecha de entrega: 22/06/2026**
- **Repo auditado en la Parte A** (solo tipo/contexto, NO el código): Repositorio proyecto de WEB -SCRAPING creado para verificar la identidad en las listas de control, nacionales e internacionales.

---

## 1. Hallazgos de la auditoría (Parte A)

> 3-5 cosas que el agente **no pudo inferir** del código y que tendrías que decirle explícitamente.
> Redáctalas para que otra persona las entienda sin contexto adicional. **Sin código propietario ni secretos.**

1. El agente no pudo detectar como están el nombre de las variables o funciones (camelCase).
2. En cuanto a las restricciones de no actualizar las carpetas reservadas del proyecto tampoco pudo ser detectadas.
3. Tampoco pudo detectar unas configuraciones internas para que se ajuste un estilo de un framework utilizado, para los objetos de los componentes (PrimeFaces - Poseidon).

---

## 2. SKILL.md de la skill creada (Parte B)

> Pega aquí el contenido completo de tu `.claude/skills/<nombre-skill>/SKILL.md`
> (o enlaza al archivo en tu repositorio sandbox).

```markdown
---
name: Diseño Frontend con PrimeFlex
description: Habilidad para crear interfaces y componentes utilizado en las paginas .xhtml
---

## Visión general
Esta habilidad sera utilizada en la creación de todos los componentes de UI de las paginas .xhtml manteniendo un estándar de vista en todas las paginas de la aplicación.

**Sistema de Cuadrícula (Grid):**
   - Usa `grid` para el contenedor principal.
   - Usa `col-12 md:col-6 lg:col-4` para definir el comportamiento responsive de las columnas.
   
**Tamaño y Colores:**
   - Usa las clases de color de fondo y texto integradas de PrimeFlex (ej. `bg-primary`, `text-color-secondary`, `surface-card`).
   - Para bordes: `border-round`, `border-1`, `surface-border`.

**Reglas Generales:**
   - Evita la etiqueta `<style>` para cosas básicas. Prioriza el uso de clases utilitarias de PrimeFlex.
   - Mantén un diseño "Mobile-First" utilizando siempre prefijos breakpoint de PrimeFlex cuando sea necesario (`sm:`, `md:`, `lg:`, `xl:`).
```

---

## 3. Diario de decisiones

*Skill creada:* Diseño Frontend con PrimeFlex,Habilidad para crear interfaces y componentes utilizado en las paginas .xhtml

*Decisiones de diseño tomadas:*
- Decisión 1: Que utilice PrimeFaces que es una librería de estilos, en vez de que invente estilos.
- Decisión 2: Usar una cuadricula para el contenedor principal, con el fin de mantener una uniformidad visual en el conjunto de componentes y estos a su vez que puedan adaptarse a la pantalla(responsive).

*Qué me resultó fácil:*
- Lo que me resulto fácil es el nombre y la descripción de la skill

*Qué me resultó ambiguo o difícil de decidir:*
- No se cuando va a llamar la skill, de lo que lei que hay como palabras claves que el modelo asocia en su ejecución

*Tiempo real invertido:*
- El tiempo que me tomo en leer y pensar para escribir la skill fue una hora y 30 minutos

*Qué probarías si tuvieras más tiempo:*
- Me gustaría probar en automatizar otras características que posee un componente de tabla, como por ejemplo los ordenamiento y filtros que se colocan en las columnas.

*¿Usaste IA para crear la skill?* (qué partes generaste con IA y qué partes decidiste tú)
- Use IA en revisar los estilos que tiene PrimeFlex
- Lo que defini en si mismos las reglas en como se debe aplicar

### Resultado de la prueba (Paso 8)

- ¿Se activó cuando lo esperabas?
    Realice la creación de una nueva función que implica la creación de una nueva vista .xhtml y si se activo la habilidad
- ¿El resultado fue el que querías?
    La vista si adopto el estilo que especifiqué en el skill
- Si no, ¿qué crees que falló? (no la "arregles" — documenta el primer intento)
   No aplica respuesta.
