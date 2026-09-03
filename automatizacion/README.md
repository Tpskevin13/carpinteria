# Automatización de Máquinas

# Automatización de Máquinas

Lógica de mando y control de la máquina: arranque directo de un motor trifásico con enclavamiento, mediante contactor comandado por pulsadores de marcha y paro, más protección térmica.

## Archivos

| Archivo | Contenido | Estado |
|---|---|---|
| `normal_030338.cad` (CADe SIMU) | Esquema de **mando** (circuito de control) y **potencia** (circuito de fuerza) del arranque directo | ✅ Revisado y correcto |
| `topografico_030341.cad` (CADe SIMU) | Vista topográfica: disposición física de los componentes en el tablero | 🔄 Pendiente de terminar |

> Los `.cad` son archivos de proyecto de CADe SIMU. Para que cualquiera pueda verlos sin instalar el programa, se exportan también en PDF/PNG (ver `esquemas/`).

## Circuito de mando (control)

- **`-Q`**: guardamotor/disyuntor — protección del circuito de mando.
- **`-F`**: contacto NC del relé térmico/guardamotor — corta el circuito si el motor se sobrecarga.
- **`-P`**: botón de **paro** (NC), en serie.
- **`-S`**: botón de **marcha** (NA), en paralelo con el contacto auxiliar 13-14 de `-K` (enclavamiento/retención: una vez que arranca, se mantiene solo aunque se suelte el botón).
- **`-K`**: bobina del contactor (A1-A2).

Orden de la lógica: protección → paro → marcha con enclavamiento → bobina. Correcto.

## Circuito de potencia (fuerza)

- **`-Q`** (guardamotor, 3 polos) → **`-K`** (contactos principales del contactor, 3 polos) → motor (**U1, V1, W1, PE**).

El guardamotor es un único dispositivo físico: sus contactos de potencia (3 polos) van en el circuito de fuerza, y su contacto auxiliar NC (`-F`) va en el circuito de mando.

## Pendiente / Notas

- [ ] Terminar la vista topográfica (`topografico_030341.cad`) y verificar que la numeración de bornes coincida con el esquema de mando/potencia.
- [ ] Exportar ambos archivos a PDF/PNG y subirlos junto con el `.cad` original.
- [ ] Sugerencia de prolijidad: renombrar `-P` y `-S` en el esquema como "Paro" y "Marcha" explícitamente, para que se entienda sin tener que deducirlo.

## Elementos típicos a documentar

- [ ] Contactor (marca/modelo, bobina de qué tensión, contactos auxiliares usados)
- [ ] Relé térmico / guardamotor (calibrado a qué corriente — sale del cálculo de la instalación eléctrica)
- [ ] Botón de marcha (normalmente abierto)
- [ ] Botón de paro (normalmente cerrado)
- [ ] Seta/hongo de emergencia (normalmente cerrado, enclavamiento mecánico)
- [ ] Piloto/luz indicadora de máquina encendida (opcional pero suma)


## Pendiente / Notas

- [ ] Confirmar tensión de mando (directo a 220V o con transformador a 24V — más seguro).
- [ ] Definir si el arranque es directo o si necesita arranque suave/estrella-triángulo (depende de la potencia del motor, sale de instalación eléctrica).
