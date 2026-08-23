# Panel de gastos

Panel interactivo de un solo archivo que muestra en qué se gasta un presupuesto operativo, mes a mes: gasto total del período, variación frente al mes anterior, la categoría con mayor crecimiento, desglose por categoría y el detalle completo de cada gasto en una tabla filtrable y ordenable.

Incluye un aviso de **confiabilidad de los datos**, que señala explícitamente filas con importes faltantes, gastos que el propio equipo marcó como pendientes de verificar, y posibles cargos duplicados — para que quien lo use nunca tenga más confianza en las cifras de la que los datos realmente justifican.

Construido bajo la dirección de [Claude Code](https://claude.com/claude-code), de Anthropic.

## Nota sobre los datos que se muestran

El panel viene precargado con datos reales de gasto operativo de la organización (enero–junio de 2026): proveedores, categorías e importes. Puede reemplazarlos en cualquier momento con el botón "Cargar CSV actualizado" — ver la sección siguiente.

## Cómo se actualizan los datos

Todo el procesamiento ocurre en el navegador de quien lo usa; el archivo no se conecta a ningún servidor, base de datos ni API. Para ver otro conjunto de datos, use el botón **"Cargar CSV actualizado"** dentro del panel y seleccione un archivo CSV con las columnas `Date, Vendor, Category, Amount, Notes`. Los datos cargados no se envían ni se guardan en ningún lado — existen solo mientras la pestaña del navegador está abierta.

## Stack técnico

HTML, CSS y JavaScript sin dependencias externas ni framework — un único archivo (`panel_gastos.html`), sin backend. Los gráficos son SVG generado dinámicamente en el propio navegador.

## Licencia

*(Agregar según corresponda antes de publicar.)*
