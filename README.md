# TRON Light-Cycle (Juego Android)

Un clon del clásico juego de arcade **TRON**, desarrollado de forma
nativa para Android utilizando **100% Kotlin** y **Jetpack Compose**.

El proyecto implementa un juego de "light-cycles" donde los jugadores
deben atrapar a su oponente con su estela de luz sin chocar.

Este proyecto fue creado como una demostración de: - Arquitectura
moderna de Android - Manejo de estado en Compose - Lógica de juego en
tiempo real

> **Recomendación:** graba tu pantalla mientras juegas una ronda,
> conviértelo en GIF y súbelo al repositorio. Luego reemplaza esta línea
> por la imagen real del gameplay.

``` md
![Gameplay GIF](ruta/a/tu/gameplay.gif)
```

------------------------------------------------------------------------

## ✨ Características Principales

-   Jugabilidad Clásica: Controla tu moto de luz y deja una estela. ¡No
    choques!
-   Modo un Jugador (vs. IA) con lógica básica de evasión.
-   Sistema de Puntuación --- Mejor de 10 rondas.
-   Estadísticas Persistentes via SharedPreferences.
-   Pausa y Reanudar en cualquier momento.
-   Diseño enfocado al uso horizontal (landscape).
-   Estela crece automáticamente cada 5s.
-   **Modo Bluetooth en desarrollo**.

------------------------------------------------------------------------

## 🛠️ Stack Tecnológico

-   **Lenguaje:** Kotlin
-   **UI:** Jetpack Compose
-   **Arquitectura:** MVVM
-   **Estado:** Kotlin Flows (StateFlow)
-   **Asincronía:** Coroutines
-   **Navegación:** Navigation Compose
-   **Persistencia:** SharedPreferences

------------------------------------------------------------------------

## 📂 Estructura del Proyecto

    com.example.tron
    │
    ├── data/
    │   ├── GameModels.kt
    │   ├── StatsRepository.kt
    │
    ├── navigation/
    │   ├── Screen.kt
    │
    ├── ui/
    │   ├── screens/
    │   │   ├── BluetoothConnectionScreen.kt
    │   │   ├── GameModeSelectionScreen.kt
    │   │   ├── GameScreen.kt
    │   │   ├── PlayerSetupScreen.kt
    │   │   ├── RoundResultsScreen.kt
    │   │   ├── TeamSelectionScreen.kt
    │   │   └── WinnerScreen.kt
    │   │
    │   └── theme/
    │       ├── Color.kt
    │       ├── Theme.kt
    │       └── Type.kt
    │
    ├── viewmodel/
    │   ├── GameViewModel.kt
    │
    └── MainActivity.kt

------------------------------------------------------------------------

## 🏁 Cómo Ejecutar

Requisitos: - Android Studio (última versión) - Emulador o dispositivo
Android

Clonar repo:

``` bash
git clone https://github.com/tu-usuario/tu-repositorio.git
```

Luego: 1. Abrir con Android Studio 2. Sincronizar Gradle 3. Ejecutar

------------------------------------------------------------------------

## 🔮 Futuro Trabajo / Mejoras

-   Implementar completamente el modo multijugador Bluetooth
-   Añadir música y SFX
-   Implementar Power-Ups (ya definidos en el modelo)