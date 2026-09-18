# Propuesta de Alianza Estratégica para Financiación Educativa

Micrositio ejecutivo del **Instituto Centro de Sistemas Avanzados Ltda. (ICSA)** para presentar ante una entidad financiera una propuesta de convenio de financiación educativa.

## Contenido

Página única con navegación por secciones: presentación del instituto, resumen ejecutivo de la oportunidad, población estudiantil, oferta educativa por áreas, distribución de programas, costos por programa, cursos cortos, escenarios de penetración, simulador de colocación, propuesta de valor, modelo del convenio, indicadores de seguimiento, aspectos por definir y contacto.

## Fuentes de la información

- **Cifras de población, programas y costos:** archivo institucional `DATOS PROPUESTA FINANCIERA.xlsx` (hojas BASE ESTUDIANTES, RESUMEN POR PROGRAMA, COSTOS POR PROGRAMA y COSTOS CURSOS CORTOS), período 2026-1.
- **Información institucional:** sitio oficial [icsa.edu.co](https://icsa.edu.co).

Notas de consistencia verificadas contra el archivo fuente:

- El total de 2.249 estudiantes coincide entre el conteo individual y el resumen por programa.
- El cuadro de áreas del archivo suma 2.139 porque omite el programa Auxiliar en Clínica Veterinaria (110 estudiantes); el micrositio incorpora esa área para que la distribución cierre en 2.249, y lo documenta en la propia página.
- Los totales por programa de la hoja de costos cuadran con la suma de semestres más prácticas en los 17 casos.
- La hoja de costos cubre únicamente programas técnicos; bachillerato por ciclos e idiomas no tienen costo registrado.

No se publica ningún dato personal de estudiantes: la base individual se usa solo para obtener indicadores agregados.

## Advertencias del documento

Los escenarios de penetración y los resultados del simulador son ejercicios hipotéticos de referencia. No constituyen proyecciones ni compromisos de colocación, aprobación o desembolso por ninguna de las partes. Toda condición financiera queda sujeta a las políticas y al proceso de aprobación de la entidad financiera.

## Estructura

```
index.html        Sitio completo (HTML, CSS y JavaScript sin dependencias externas)
logo.png          Logo institucional
.nojekyll         Publica el sitio tal cual en GitHub Pages
```

No requiere compilación ni instalación: se abre directamente en el navegador.

## Actualizar los datos

Todas las cifras están agrupadas al final de `index.html`, dentro del método `renderVals()` de la clase `Component`, en arreglos con nombres explícitos (`areasRaw`, `progRaw`, `costosRaw`, `cursos`, `niveles`, `instituto`, `contacto`). Para un nuevo período basta con reemplazar esos valores; la maquetación no cambia.

## Publicación

Para publicarlo con GitHub Pages: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)`**.

## Confidencialidad

Documento de trabajo de carácter confidencial, preparado para presentación ante una entidad financiera.
