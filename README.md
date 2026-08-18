# Gráficas del Agregador Defoe

Host público de las gráficas interactivas que se embeben en los artículos de
[defoe.mx](https://www.defoe.mx). Mismo propósito que `radar-defoe-media`: URLs
permanentes para material que vive dentro de una nota.

## Cómo está organizado

Una carpeta por entrega, con la fecha del artículo:

```
20260817/    «El piso lo puso la economía» — corte del 11-ago-2026
```

**Las carpetas no se sobrescriben.** Los HTML del Agregador se regeneran cada
jueves, pero un artículo publicado debe seguir mostrando los datos con los que se
escribió. Por eso cada entrega congela su copia.

## Cómo se embebe

```html
<iframe src="https://defoe-ui.github.io/defoe-graficas/20260817/eeuu_comparado_general.html"
        width="100%" height="450" frameborder="0" scrolling="no"></iframe>
```

Los HTML son autocontenidos (~1.4 MB): no piden nada a servidores externos.

## Origen

Se generan con el Paso 3 del Agregador (`graficas/R/50_run_graficas.R`) a partir
de las estimaciones del modelo bayesiano multinivel. No se editan a mano.
