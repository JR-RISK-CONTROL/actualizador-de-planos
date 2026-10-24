# Datos de los planos de evacuación (privado)

Repositorio **privado**: los planos muestran la ubicación de cajas, oficinas y salidas de las sedes. No lo hagas público.

## Estructura

```
<sede>.json          layout original (Excel de "04 Planos y senalizacion") con el plano de evacuación 2026; incluye los íconos
sedes/<sede>/plano.json   versión vigente del plano; la crea y la actualiza el editor al guardar
```

Sedes: `novena`, `palatino`, `sanrafael`, `salitre`, `unicentro`, `ensueno`, `soacha`, `mercurio`, `cosmocentro`, `crowncali`, `bocagrande`, `sanpedro`.

## Historial

Cada **Guardar versión** del editor es un commit sobre `sedes/<sede>/plano.json` con el mensaje `<Sede> · v<N>: <motivo>`. El historial de la sede es el historial de commits de ese archivo, y desde el editor (botón **Historial**) se puede restaurar cualquier versión.

No edites los archivos `<sede>.json`: son la referencia original. Si se borra `plano.json`, el editor vuelve a abrir el layout original.

## Acceso

- Quien edita necesita acceso de escritura al repositorio y un token *fine-grained* con permiso **Contents: Read and write** solo sobre este repositorio.
- Quien solo consulta recibe el PDF; no necesita acceso.
