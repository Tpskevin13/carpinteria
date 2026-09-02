# Carpintería [Nombre de la Empresa] — Proyecto Estudiantil

Proyecto integrador escolar/técnico que simula el diseño y automatización de una carpintería industrial. El equipo aborda cuatro frentes de trabajo:

| Área | Carpeta | Responsable(s) |
|---|---|---|
| 🏢 La empresa | [`empresa/`](./empresa) | — |
| ⚡ Instalación eléctrica | [`instalacion-electrica/`](./instalacion-electrica) | — |
| 🔌 Tablero eléctrico | [`tablero/`](./tablero) | — |
| 🧵 Tuberías (canalizaciones) | [`tuberias/`](./tuberias) | — |
| 🛠️ Modelado 3D de máquina | [`modelado-3d/`](./modelado-3d) | — |
| 🤖 Automatización de máquinas | [`automatizacion/`](./automatizacion) | — |
| 💡 Iluminación | [`iluminacion/`](./iluminacion) | — |

## Sobre el proyecto

[Descripción breve: qué máquinas tiene la carpintería, qué problema resuelve el proyecto, alcance del trabajo.]

## Estructura del repositorio

```
carpinteria-proyecto/
├── empresa/                     # Presentación de la carpintería, máquinas, organigrama
├── instalacion-electrica/       # Circuitos, cálculo de cargas, planos unifilares
│   ├── planos/
│   └── calculos/
├── tablero/                       # Tablero general: llaves térmicas, diferencial
│   └── planos/
├── tuberias/                       # Canalizaciones: tipo de caño, recorrido, diámetros
│   └── planos/
├── modelado-3d/                     # Modelo SolidWorks de la máquina elegida
│   ├── piezas/
│   └── renders/
├── automatizacion/                   # Lógica de control: relé, marcha, paro, emergencia
│   ├── esquemas/
│   └── logica-relee/
├── iluminacion/                        # Cálculo lumínico y disposición de luminarias
│   ├── planos/
│   └── calculos/
├── docs/                                # Memoria descriptiva, cronograma, presentación final
└── recursos/                              # Fotos, normas, fichas técnicas de referencia
    ├── fotos/
    └── referencias/
```

## Cómo documentar

Cada carpeta principal tiene su propio `README.md` con una guía de qué subir y cómo nombrarlo. Los archivos pesados o binarios (SolidWorks, PDFs de planos, fotos) van en sus subcarpetas; los `README.md` explican en texto qué contiene cada uno y por qué se tomó cada decisión.

## Equipo

- Kevin Dibella
- Octavio Di Carlantonio
- Lucio Di Carlantonio
- Agustín Duarte

## Cronograma

Ver [`docs/cronograma.md`](./docs/cronograma.md)

## Licencia

Ver [`LICENSE`](./LICENSE)
