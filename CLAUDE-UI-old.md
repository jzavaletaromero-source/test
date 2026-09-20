## UI

Dirección visual: **«Claro»** — decidida el 2026-09-15 sobre maquetas pobladas,
sustituye a «Ar» (`docs/05-sistema-de-diseno.md` §1.1). Plus Jakarta Sans
servida desde el repositorio, radios grandes (6 · 10 · 14 · 20 · 26), sombras
largas y suaves, mucho aire, y **el chrome tintado de verde claro** — el menú
lateral es la única región con color de marca. Modo claro por defecto; el oscuro
es elección de quien usa.

⚠️ **El color del lienzo es semántico, nunca decorativo.** Conforme, corrección,
crítico. Una tarjeta pintada de pastel «para que se vea con más color» cuesta la
regla que hace legible un informe de conformidad. Si un tablero se ve gris, casi
siempre es porque está vacío.

**`packages/ui` ya existe** (2026-09-15) y es de donde sale todo: `tokens.css`,
`motion.ts` y los once primitivos —`Button`, `Badge`, `Input`, `Table`,
`Select`, `Combobox`, `Dialog`, `Sheet`, `Skeleton`, `ThemeToggle`,
`DatePicker`—.

**Toda interfaz se construye con ellos.** No se escribe un `<input>`, un
`<table>` ni un `<select>` a mano: si un primitivo no da lo que hace falta, se
amplía el primitivo, no se rodea. Y prohibido introducir un color, espaciado,
radio o tamaño de fuente que no exista como token: si falta, se añade a
`tokens.css` con un comentario que diga POR QUÉ, y a los dos bloques oscuros.

`docs/05-sistema-de-diseno.md` sigue siendo el razonamiento; el paquete es la
implementación. Si los dos discrepan, manda el documento — salvo donde el
paquete anote una desviación deliberada, que las hay y están marcadas.

Hay una hoja de muestra con datos SST reales dentro (`packages/ui/demo`), que
se genera con los componentes del paquete: `node packages/ui/demo/dist/render.js`
tras `npx tsc --build`.

Esta es una app **densa en datos de compliance**, no una app de consumo:
densidad alta pero jerarquizada, feedback inmediato, cero pantallas de carga en
blanco.
