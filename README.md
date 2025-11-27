# VoidOS 🌌

**Een Lichtgewicht, Modulair Besturingssysteem Gebouwd op de Moderne Principes van Eenvoud.**

[![Labeler](https://github.com/Bmgtje25/VoidOS/actions/workflows/label.yml/badge.svg)](https://github.com/Bmgtje25/VoidOS/actions/workflows/label.yml)
[![GitHub contributors](https://img.shields.io/github/contributors/Bmgtje25/VoidOS?style=flat-square)](https://github.com/Bmgtje25/VoidOS/graphs/contributors)
[![GitHub issues](https://img.shields.io/github/issues/Bmgtje25/VoidOS?style=flat-square)](https://github.com/Bmgtje25/VoidOS/issues)
[![Copyright](https://img.shields.io/badge/Copyright-All%20Rights%20Reserved-red?style=flat-square)](./)

---

## ✨ Over VoidOS

VoidOS is een experimenteel besturingssysteem, ontworpen om de overhead te minimaliseren en maximale aanpasbaarheid te bieden. Het project dient als een leerplatform om de diepgaande werking van de kernel, geheugenbeheer, en driver-ontwikkeling te begrijpen.

Het is primair bedoeld voor ontwikkelaars en enthousiastelingen die geïnteresseerd zijn in **low-level programmeren** en de creatie van besturingssystemen vanaf de basis.

---

## 🚀 Hoofdkenmerken

* **Modulaire Microkernel Architectuur:** Maakt een hoge mate van stabiliteit en foutisolatie mogelijk.
* **Aangepaste Bootloader:** Speciaal ontworpen voor snel en efficiënt opstarten.
* **Basis Driver Ondersteuning:** Vroege ondersteuning voor essentiële hardware (b.v., toetsenbord, serieel).
* **Geavanceerd Geheugenbeheer:** Implementatie van Paging/Virtual Memory.
* **Multitasking (Toekomstig):** Planning voor pre-emptieve multitasking voor het uitvoeren van meerdere processen.

---

## 🛠️ Bouwen en Uitvoeren

Om VoidOS lokaal te bouwen, heb je een **cross-compiler toolchain** en hulpprogramma's zoals **`make`** en **`qemu`** (voor emulatie) nodig.

### Vereisten

* `gcc` (cross-compiler voor je doelarchitectuur, b.v., `i686-elf-gcc`)
* `make`
* `qemu` (voor het testen)

### Stappen

1.  **Clone de Repository:**
    ```bash
    git clone [https://github.com/Bmgtje25/VoidOS.git](https://github.com/Bmgtje25/VoidOS.git)
    cd VoidOS
    ```

2.  **Initialiseer Submodules (Indien van toepassing):**
    ```bash
    git submodule update --init --recursive 
    ```

3.  **Compileer het OS:**
    ```bash
    make all
    ```
    *Dit commando compileert de kernel en de nodige modules.*

4.  **Start de Emulatie (met QEMU):**
    ```bash
    make run
    ```
    *Dit start het gebouwde OS in de QEMU emulator.*

> **Opmerking:** Zorg ervoor dat de paden naar je cross-compiler correct zijn ingesteld in de `Makefile` als je problemen ondervindt met het bouwen.

---

## 🗺️ Status en Roadmap

| Fase | Status | Doel |
| :--- | :--- | :--- |
| **Huidig: Fase 1** | **In Ontwikkeling** | Kernel-initialisatie, Basis Geheugenbeheer, Schermuitvoer (VGA). |
| Fase 2 | Gepland | Multitasking, Systeemoproepen (Syscalls), Basis Shell-interface. |
| Fase 3 | Gepland | Filesystem-ondersteuning, Driver-uitbreiding (netwerk, opslag). |

### Belangrijkste Focus Momenteel

1.  Voltooiing van het Geheugenbeheer (Heap & Paging).
2.  Implementatie van de Interrupt Service Routines (ISR's) en Interrupt Request (IRQ) handling.

---

## 🤝 Bijdragen

Omdat dit project **Alle Rechten Voorbehouden** is, zijn externe bijdragen momenteel beperkt. Als je geïnteresseerd bent om aan dit project bij te dragen, neem dan direct contact op met de auteur via de contactgegevens hieronder om de mogelijkheden te bespreken.

---

## ⚖️ Auteursrecht en Gebruik

**Alle rechten op deze broncode zijn voorbehouden.**

Dit project is **geen** open source en de code mag niet worden gekopieerd, bewerkt, of verspreid zonder de uitdrukkelijke, schriftelijke toestemming van de auteur (Bmgtje25). Dit besturingssysteem is uitsluitend voor demonstratie en persoonlijk onderzoek.

---

## 📞 Contact

**Boris** - [@Bmgtje25](https://github.com/Bmgtje25)

Project Link: [https://github.com/Bmgtje25/VoidOS](https://github.com/Bmgtje25/VoidOS)
