# Automatización de Máquinas

Lógica de mando y control de la máquina, basada en relé (contactor) comandado por pulsadores de marcha, paro y parada de emergencia — el esquema clásico de arranque directo de un motor.

## Contenido a subir

- **`esquemas/`**
  - **Circuito de fuerza**: motor → contactor → protecciones (térmica/guardamotor) → alimentación.
  - **Circuito de mando** (comúnmente a 220V o con transformador a 24V, según lo que definan): botón de marcha (NA) en paralelo con el contacto auxiliar del contactor (enclavamiento/retención), en serie con el botón de paro (NC) y el hongo de emergencia (NC).
  - Diagrama completo: fuerza + mando en la misma lámina, como se entrega en un proyecto real.
- **`logica-relee/`**
  - Explicación en texto de la lógica: qué hace cada elemento (contactor, relé térmico, pulsadores) y por qué está conectado así.
  - Si suman algo más avanzado (temporizador, relé de enclavamiento para marcha adelante/atrás, sensor, etc.) documentarlo acá también.

## Elementos típicos a documentar

- [ ] Contactor (marca/modelo, bobina de qué tensión, contactos auxiliares usados)
- [ ] Relé térmico / guardamotor (calibrado a qué corriente — sale del cálculo de la instalación eléctrica)
- [ ] Botón de marcha (normalmente abierto)
- [ ] Botón de paro (normalmente cerrado)
- [ ] Seta/hongo de emergencia (normalmente cerrado, enclavamiento mecánico)
- [ ] Piloto/luz indicadora de máquina encendida (opcional pero suma)

## Formato sugerido

Los esquemas se pueden dibujar en cualquier software de diagramas (incluso a mano y escanear) y subir como PDF/imagen. Si usan un simulador (como el simulador de circuitos de CADe SIMU, o incluso Fritzing/draw.io para el diagrama), aclarar cuál en este README.

## Pendiente / Notas

- [ ] Confirmar tensión de mando (directo a 220V o con transformador a 24V — más seguro).
- [ ] Definir si el arranque es directo o si necesita arranque suave/estrella-triángulo (depende de la potencia del motor, sale de instalación eléctrica).
