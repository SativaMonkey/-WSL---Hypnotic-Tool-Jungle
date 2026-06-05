# TUNE.html | Hypnotic Tool Jungle
**v1.0.0 | ONEOFAPES**

[![Deploy with Vercel](https://vercel.com/button)](https://wsl-hypnotic-tool-jungle.vercel.app/)
[![Web Audio API](https://img.shields.io/badge/Audio-Web_Audio_API-black?style=flat-square)]()
[![HTML5 Canvas](https://img.shields.io/badge/Graphics-Canvas_3D-black?style=flat-square)]()

<div align="center">
  <a href="https://wsl-hypnotic-tool-jungle.vercel.app/">
    <img src="readme_/ui-preview.gif" alt="Hypnotic Tool Jungle - Console UI" width="800"/>
  </a>
  <br><br>
  <a href="https://wsl-hypnotic-tool-jungle.vercel.app/">
    <img src="readme_/visualizer-preview.gif" alt="Hypnotic Tool Jungle - 3D Visualizer" width="800"/>
  </a>
  <br><br>
  <p><i>Click the interface to launch the live generative environment.</i></p>
</div>

## System Overview
Результат нічного спринту. Чистий vibecode. Повністю автономне генеративне аудіо-візуальне середовище, запаковане в один файл `TUNE.html`. Жодних зовнішніх залежностей, фреймворків чи медіа-ассетів. Вся генерація звуку та 3D-графіки відбувається локально на стороні клієнта. Повна оффлайн-функціональність.

* **Target Vibe:** Deep House / Dystopian Ambient.
* **Architecture:** Zero-dependency (Vanilla JS + Web Audio API + HTML5 Canvas).

## Generative Engine & Math
Логіка синтезу та візуалізації побудована на жорстких математичних послідовностях. Динамічний сід унеможливлює повторення сесій.

* **Algorithmic Core:** Мелодійні лінії, вибір пресетів тембру та переходи акордів генеруються на основі обробки символів числа Пі (`piStr`) та ряду Фібоначчі (`fib`).
* **Harmonic Grid:** Обертання дорійських акордних послідовностей (до 5 голосів). Транспоновані для вивільнення суб-басового діапазону.
* **Procedural Layers:** Генеративна перкусія (liquid drips, organic liquid foley, phonk cowbells, congas, vocal chants) та ефект деградації стрічки (Wow/Flutter LFO).

## Visual Pipeline (3D Canvas)
Матричні 3D-проєкції з розрахунком тривимірних координат вершин для 6 режимів (3D DNA Helix, Cylinder Mesh, Particle Wave Ring, Axonometric Step Grid, Terrain Wave). 
Процедурна анімація зоряного неба та пилу жорстко прив'язана до амплітуди низьких та середніх частот.

## Interactive Control System
Система оптимізована під touch-інтерфейси (passive-listeners, блокування скролу сторінки, нульова затримка відгуку).

* **XY Pad:**
  * **X-Axis:** Майстер-фільтр (Lowpass ліворуч / Highpass праворуч). Центр — мертва зона (Bypass).
  * **Y-Axis:** Частота LFO-модуляції саб-басу (1Hz - 20Hz).
* **Soundboard Interrupts:** Миттєве накладання ваншотів поверх міксу через виділену шину реверберації (`1` Orca Call, `2` Sonar Ping, `3` Singing Bowl, `4` Abyssal Swell).
* **DJ Tape-Stop `[SPACE]`:** Глобальний плавний глайд BPM до 10 із приглушенням гучності (ducking). Відпускання відновлює оригінальний темп.

## Deployment & Execution
**Local Run** Відкрити `TUNE.html` у будь-якому сучасному браузері.

**Vercel Deployment** Статичний деплой. Build commands не потрібні. Root Directory: `./`
