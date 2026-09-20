# TEST DE LENGUAJE VISUAL — BRASTT

## 1. ROL

Actúa como un UI/UX Designer Senior especializado en:

- SaaS B2B
- software empresarial
- sistemas de gestión
- aplicaciones profesionales complejas
- dashboards operativos
- sistemas de Seguridad y Salud en el Trabajo (SST)

Tu responsabilidad en esta tarea es exclusivamente definir y construir
un TEST VISUAL del lenguaje de interfaz de BRASTT.

---

# 2. CONTEXTO DEL PRODUCTO

BRASTT es un SaaS para Clínicas y Profesionales de Seguridad y Salud
en el Trabajo (SST) en Brasil.

El sistema manejará información relacionada con:

- empresas clientes
- establecimientos
- ambientes
- auditorías
- inspecciones
- NRs
- conformidad
- riesgos
- hallazgos
- documentos
- capacitaciones
- medicina ocupacional
- ASO
- PGR
- PCMSO
- plazos
- vencimientos
- obligaciones
- eventos
- histórico
- evidencias
- actividades pendientes

Es un software profesional de uso diario.

NO es una landing page.
NO es un sitio institucional.
NO es una aplicación de entretenimiento.

La interfaz debe priorizar:

- claridad
- productividad
- lectura rápida
- jerarquía
- densidad de información adecuada
- estados visuales
- seguimiento
- indicadores
- profesionalismo

---

# 3. OBJETIVO DE ESTA TAREA

IMPORTANTE:

Esta tarea es EXCLUSIVAMENTE un TEST VISUAL.

El objetivo es crear:

- PROPUESTA A
- PROPUESTA B
- PROPUESTA C

para comparar diferentes lenguajes visuales antes de decidir cuál
será implementado posteriormente en BRASTT.

Quiero poder visualizar las tres alternativas y decidir cuál dirección
de diseño continuar.

NO quiero implementar todavía el diseño definitivo en toda la aplicación.

---

# 4. REGLAS ABSOLUTAS

Estas reglas tienen PRIORIDAD sobre cualquier otra instrucción de este
documento.

## NO modificar la aplicación existente

No debes:

- modificar funcionalidades existentes
- modificar lógica de negocio
- modificar APIs
- modificar la base de datos
- modificar rutas existentes
- reemplazar componentes existentes
- eliminar componentes existentes
- hacer refactoring general
- cambiar el comportamiento actual de la aplicación
- reemplazar la UI productiva actual

## Regla principal

ANTES DE MODIFICAR CUALQUIER ARCHIVO:

1. inspecciona el proyecto
2. entiende su arquitectura
3. identifica dónde puede realizarse el test de forma aislada
4. determina qué archivos pueden crearse sin afectar la aplicación

Si existe riesgo de modificar accidentalmente la aplicación real,
detente y utiliza una estrategia más aislada.

---

# 5. FASE 1 — INSPECCIÓN DEL PROYECTO

Antes de escribir código debes inspeccionar el proyecto.

Identifica:

### Arquitectura

- framework
- estructura de carpetas
- sistema de routing
- arquitectura de componentes

### UI

- librería de componentes
- sistema de estilos
- Tailwind u otro CSS framework
- variables CSS
- tokens
- temas
- componentes reutilizables

### Configuración de IA / desarrollo

Busca:

- CLAUDE.md
- archivos de instrucciones
- documentación de UI
- design system
- theme configuration
- componentes base

### Resultado de la inspección

Antes de implementar el test, determina:

1. dónde crear el entorno aislado
2. qué componentes pueden reutilizarse
3. qué archivos NO deben modificarse
4. dónde documentar las nuevas reglas visuales

NO realices cambios durante esta fase.

---

# 6. FASE 2 — DEFINICIÓN DEL LENGUAJE VISUAL

El concepto central de BRASTT debe ser:

> LIMPIO + PROFESIONAL + VISUALMENTE INFORMATIVO

IMPORTANTE:

"Limpio" NO significa:

- todo blanco
- todo gris
- ausencia de color
- ausencia de indicadores
- tarjetas completamente planas
- interfaces sin jerarquía
- únicamente tablas y texto

La interfaz debe utilizar elementos visuales para ayudar a comprender
rápidamente la información.

Debe ser posible identificar visualmente:

- conformidad
- pendientes
- riesgos
- criticidad
- progreso
- plazos
- vencimientos
- cobertura
- documentos
- actividades
- histórico
- estados
- prioridades

---

# 7. REGLA CENTRAL DE DISEÑO VISUAL

Esta es una de las reglas más importantes del proyecto.

NO esperes a que el usuario solicite explícitamente un indicador visual.

Antes de diseñar cualquier componente o pantalla:

1. analiza qué información representa
2. identifica si alguno de esos datos tiene una dimensión visual
3. determina si puede comunicarse mejor mediante un patrón visual
4. utiliza ese patrón cuando aporte valor

Ejemplo:

Si existe:

"ASO vence en 5 días"

debes considerar:

- indicador de vencimiento
- barra temporal
- badge
- estado semántico
- color apropiado

Si existe:

"87% de conformidad"

debes considerar:

- progress bar
- indicador circular
- porcentaje visual
- tendencia

Si existe un histórico:

debes considerar:

- timeline
- actividad cronológica
- evolución

---

# 8. INDICADORES VISUALES

Utiliza indicadores cuando tengan significado funcional.

## PROGRESO

Considerar:

- progress bars
- barras de cobertura
- porcentajes
- etapas
- progreso de tareas
- progreso de auditorías
- progreso de capacitaciones

## PLAZOS

Considerar:

- tiempo restante
- barras de tiempo
- countdown
- vencimiento próximo
- vencido
- días restantes

## ESTADOS

Considerar:

- badges
- pills
- chips
- indicadores circulares
- iconos semánticos
- estados con color

## RIESGO / CRITICIDAD

Considerar:

- severidad
- prioridad
- criticidad
- alertas
- niveles de riesgo

## HISTÓRICO

Considerar:

- timelines
- eventos cronológicos
- actividad reciente
- evolución

## COBERTURA

Considerar:

- porcentajes
- progress bars
- indicadores circulares
- métricas comparativas

## DOCUMENTOS

Considerar estados como:

- válido
- próximo a vencer
- vencido
- pendente
- aprovado
- rejeitado

## AUDITORÍAS

Considerar:

- progreso
- itens conformes
- itens não conformes
- cobertura de NRs
- pendências

## CAPACITACIONES

Considerar:

- trabalhadores concluídos
- trabalhadores pendentes
- progresso
- vencimentos

## MEDICINA OCUPACIONAL

Considerar:

- exames realizados
- exames pendentes
- próximos vencimentos
- ASOs
- acompanhamento

---

# 9. REGLA CONTRA LA DECORACIÓN

NO utilizar indicadores visuales únicamente para decorar.

Todo elemento visual debe tener una función.

Antes de utilizar un indicador pregúntate:

> ¿Este elemento ayuda al usuario a comprender, comparar, priorizar o detectar información?

Si la respuesta es NO: NO lo utilices.

La interfaz debe ser visualmente rica en información, NO visualmente cargada de decoración.

---

# 10. USO DEL COLOR

BRASTT NO debe ser completamente monocromático.

El color debe utilizarse principalmente para comunicar significado.

## VERDE

Utilizar para:

- conforme
- concluído
- aprovado
- dentro del plazo
- estado saludable/normal

## ÁMBAR / AMARILLO

Utilizar para:

- atenção
- pendência
- próximo vencimento
- prioridade média
- situação que requiere atención

## ROJO

Utilizar para:

- crítico
- vencido
- não conforme
- risco elevado
- problema importante

## AZUL

Utilizar para:

- informação
- atividade
- sincronização
- información contextual

## GRIS

Utilizar para:

- información secundaria
- elementos neutros
- elementos deshabilitados

### Restricción

No utilizar colores excesivamente saturados.

No utilizar color únicamente porque "se ve bonito".

El color debe tener significado.

---

# 11. DENSIDAD DE INFORMACIÓN

BRASTT es un SaaS de uso diario.

Por lo tanto:

DEBE:

- mostrar suficiente información
- ser escaneable
- tener buena jerarquía
- aprovechar correctamente el espacio
- permitir detectar problemas rápidamente
- permitir comparar información

NO DEBE:

- convertir cada dato en una tarjeta gigante
- desperdiciar espacio
- tener demasiado espacio vacío sin propósito
- sentirse congestionado
- parecer una landing page

Buscar un equilibrio entre:

DENSIDAD + LEGIBILIDAD + JERARQUÍA

---

# 12. USO DE CARDS

NO convertir todo en cards.

Utilizar cards únicamente cuando ayuden a:

- agrupar información relacionada
- separar contextos
- destacar métricas
- organizar una sección

Combinar diferentes patrones:

- métricas
- tablas
- listas
- progress bars
- timelines
- alertas
- indicadores
- filtros
- secciones
- contenido contextual

Una pantalla profesional NO debe parecer una cuadrícula de
tarjetas independientes.

---

# 13. CREAR LAS TRES PROPUESTAS

Las tres propuestas deben representar:

- la misma información
- la misma finalidad
- las mismas funcionalidades conceptuales

La diferencia debe estar principalmente en:

- composición
- jerarquía
- densidad
- cards
- indicadores
- color
- distribución
- tratamiento visual

NO crear tres aplicaciones diferentes.

---

# 14. PROPUESTA A — ENTERPRISE CLEAN

Nombre:

ENTERPRISE CLEAN

Características:

- extremadamente limpia
- profesional
- sobria
- excelente jerarquía
- colores utilizados principalmente como indicadores
- foco en productividad
- apariencia de software empresarial premium

Debe transmitir:

"software empresarial serio, eficiente y confiable".

---

# 15. PROPUESTA B — MODERN CLINICAL

Nombre:

MODERN CLINICAL

Características:

- sensación de tecnología aplicada a salud/SST
- mayor presencia de indicadores visuales
- colores suaves
- estados claramente diferenciados
- riesgos visibles
- vencimientos visibles
- progreso visible
- sensación de sistema especializado

Debe transmitir:

"software especializado en SST moderno y profesional".

---

# 16. PROPUESTA C — PREMIUM DATA-DRIVEN

Nombre:

PREMIUM DATA-DRIVEN

Características:

- mayor énfasis en métricas
- dashboards visuales
- progress bars
- cobertura
- timelines
- tendencias
- indicadores
- jerarquía sofisticada
- apariencia de SaaS premium

Debe transmitir:

"plataforma moderna orientada a datos y toma rápida de decisiones".

---

# 17. ELEMENTOS QUE NO QUIERO

Las tres propuestas deben seguir siendo profesionales.

NO utilizar:

- gaming
- cyberpunk
- neon
- exceso de glassmorphism
- efectos exagerados
- gradientes excesivos
- animaciones innecesarias
- apariencia de landing page
- estética futurista exagerada
- elementos decorativos sin función
- diseños experimentales que reduzcan la usabilidad

---

# 18. AISLAMIENTO DEL TEST

Las tres propuestas deben existir en un entorno aislado.

Puedes crear, según la arquitectura existente:

- /ui-test
- /ui-preview
- /design-test

o utilizar otra estrategia técnicamente más apropiada.

La decisión debe basarse en la arquitectura actual.

IMPORTANTE:

El entorno de test NO debe reemplazar la aplicación existente.

NO reemplazar:

- componentes reales
- rutas reales
- páginas reales
- estilos productivos
- lógica productiva

---

# 19. DATOS MOCK

Puedes utilizar datos mock para demostrar visualmente el diseño.

Los datos mock deben:

- ser claramente identificables como datos de prueba
- representar escenarios realistas de SST
- permitir demostrar indicadores
- permitir demostrar estados
- permitir demostrar progreso
- permitir demostrar vencimientos

NO deben:

- modificar la base de datos
- modificar APIs
- convertirse en datos reales
- crear funcionalidades de negocio inexistentes

---

# 20. DESIGN SYSTEM PERMANENTE

Después de inspeccionar el proyecto identifica dónde deben quedar registradas las reglas de UI.

Prioridad:

1. CLAUDE.md / instrucciones existentes
2. documentación existente del Design System
3. archivo de configuración apropiado
4. crear documentación específica si no existe una ubicación adecuada

IMPORTANTE:

No crear documentación duplicada si ya existe un archivo apropiado.

No modificar archivos de configuración innecesariamente.

---

# 21. REGLAS PERMANENTES PARA FUTURAS INTERFACES

Debe quedar documentado que las futuras interfaces de BRASTT deben:

1. ser limpias pero no monocromáticas
2. utilizar color semánticamente
3. utilizar indicadores visuales cuando aporten información
4. utilizar progress bars para progreso/cobertura cuando corresponda
5. utilizar badges/chips para estados
6. utilizar indicadores de criticidad
7. utilizar timelines para históricos cuando corresponda
8. utilizar indicadores de vencimiento para plazos
9. mantener jerarquía visual clara
10. mantener buena densidad de información
11. evitar exceso de cards
12. evitar decoración sin significado
13. mantener apariencia SaaS B2B premium
14. priorizar legibilidad
15. priorizar productividad
16. mantener consistencia visual entre pantallas

---

# 22. REGLA DE DECISIÓN VISUAL

Antes de crear cualquier nueva pantalla en BRASTT:

ANALIZAR:

- ¿Existe progreso?
- ¿Existe porcentaje?
- ¿Existe cobertura?
- ¿Existe estado?
- ¿Existe prioridad?
- ¿Existe severidad?
- ¿Existe riesgo?
- ¿Existe vencimiento?
- ¿Existe tendencia?
- ¿Existe histórico?
- ¿Existe comparación?

Si existe alguna de estas dimensiones:

CONSIDERAR automáticamente un patrón visual apropiado.

No esperar a que el usuario diga:

"usa una barra de progreso"

o:

"usa un indicador de vencimiento".

Esta capacidad debe formar parte del criterio normal de diseño de BRASTT.

---

# 23. CRITERIOS DE ACEPTACIÓN

El trabajo será considerado correcto únicamente si:

### A. Seguridad del producto

- La aplicación existente continúa funcionando.
- No se modificó la lógica existente.
- No se modificó la base de datos.
- No se modificaron APIs.
- No se reemplazaron componentes productivos.
- No se modificaron rutas productivas innecesariamente.

### B. Test visual

Existen:

- Propuesta A
- Propuesta B
- Propuesta C

y puedo cambiar entre ellas fácilmente.

### C. Diferenciación

Las tres propuestas deben ser visualmente distinguibles.

NO quiero tres versiones prácticamente iguales.

### D. Indicadores

La interfaz debe demostrar de forma clara el uso de:

- progreso
- cobertura
- estados
- criticidad
- vencimientos
- alertas
- métricas
- histórico

cuando esos conceptos existan en los datos utilizados.

### E. Profesionalismo

Debe parecer:

SaaS B2B profesional especializado en SST.

NO debe parecer:

- landing page
- template genérico
- dashboard genérico
- aplicación experimental

---

# 24. RESULTADO FINAL ESPERADO

Al finalizar debes entregar:

## 1. Tres propuestas funcionando

- A — Enterprise Clean
- B — Modern Clinical
- C — Premium Data-Driven

## 2. Selector

Una forma clara de cambiar entre las tres propuestas.

## 3. Resumen

Explicar brevemente:

- diferencia de A
- diferencia de B
- diferencia de C

## 4. Patrones visuales utilizados

Indicar cuáles fueron utilizados:

- progress bars
- badges
- status
- timelines
- alertas
- métricas
- vencimientos
- cobertura
- etc.

## 5. Design System

Indicar:

- qué archivo fue actualizado
- qué reglas permanentes fueron agregadas

## 6. Seguridad

Confirmar explícitamente:

> La aplicación productiva existente NO fue modificada.

---

# 25. ORDEN OBLIGATORIO DE EJECUCIÓN

Ejecuta esta tarea en este orden:

FASE 1
→ Inspeccionar proyecto.

FASE 2
→ Identificar arquitectura y sistema de UI.

FASE 3
→ Identificar dónde crear el test aislado.

FASE 4
→ Crear la Propuesta A.

FASE 5
→ Crear la Propuesta B.

FASE 6
→ Crear la Propuesta C.

FASE 7
→ Verificar que las tres propuestas sean realmente diferentes.

FASE 8
→ Verificar que ninguna propuesta haya modificado accidentalmente
la aplicación productiva.

FASE 9
→ Actualizar únicamente la documentación/configuración apropiada
para establecer las reglas permanentes de UI.

FASE 10
→ Entregar resumen final.

---

# 26. REGLA FINAL

NO implementes todavía ninguna propuesta como diseño definitivo.

PRIMERO:

crear → visualizar → comparar → decidir.

DESPUÉS de que el usuario seleccione una propuesta se podrá realizar
una segunda tarea para implementar ese lenguaje visual en la aplicación
real.

EL OBJETIVO DE ESTA TAREA ES:

> CREAR 3 ALTERNATIVAS VISUALES AISLADAS PARA EVALUAR Y ELEGIR UNA
> DIRECCIÓN DE DISEÑO PARA BRASTT.
