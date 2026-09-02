# Carpintería [TK-VA] — Proyecto 

Proyecto integrador escolar/técnico que simula el diseño y automatización de una carpintería industrial. El equipo aborda cuatro frentes de trabajo:

| Área | Carpeta | Responsable(s) |
|---|---|---|
|  Instalación eléctrica | [`instalacion-electrica/`](./instalacion-electrica) | — |
|  Modelado 3D de máquina | [`modelado-3d/`](./modelado-3d) | — |
|  Automatización de máquinas | [`automatizacion/`](./automatizacion) | — |
|  Iluminación | [`iluminacion/`](./iluminacion) | — |

## Sobre el proyecto

[Descripción breve: qué máquinas tiene la carpintería, qué problema resuelve el proyecto, alcance del trabajo.]

## Estructura del repositorio

```
carpinteria-proyecto/
├── instalacion-electrica/     # Tablero, circuitos, cálculo de cargas, planos unifilares
│   ├── planos/
│   └── calculos/
├── modelado-3d/                # Modelo SolidWorks de la máquina elegida
│   ├── piezas/
│   └── renders/
├── automatizacion/              # Lógica de control: relé, marcha, paro, emergencia
│   ├── esquemas/
│   └── logica-relee/
├── iluminacion/                  # Cálculo lumínico y disposición de luminarias
│   ├── planos/
│   └── calculos/
├── docs/                          # Memoria descriptiva, cronograma, presentación final
└── recursos/                      # Fotos, normas, fichas técnicas de referencia
    ├── fotos/
    └── referencias/
```

## Cómo documentar

Cada carpeta principal tiene su propio `README.md` con una guía de qué subir y cómo nombrarlo. Los archivos pesados o binarios (SolidWorks, PDFs de planos, fotos) van en sus subcarpetas; los `README.md` explican en texto qué contiene cada uno y por qué se tomó cada decisión.

## Equipo

- [Integrante 1] — [rol]
- [Integrante 2] — [rol]
- [Integrante 3] — [rol]

## Cronograma

Ver [`docs/cronograma.md`](./docs/cronograma.md)

## Licencia

Ver [`LICENSE`](./LICENSE)
