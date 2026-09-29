# CONFORM-X

Helmet-mounted conformal antenna system for tactical communications in urban CQB environments.

## Repository contents

- `src/conform-x-simulator.html` — interactive CONFORM-X simulator/source code.
- `docs/Schematic.pdf` — supplied technical architecture schematic.
- `README.md` — project documentation derived from the supplied README document.

## Technical architecture

The supplied project description specifies six thin, flexible antenna elements around the helmet surface, with UHF for voice communication and 1.28 GHz L-band for video/data. It also describes AMC/HIS plus RF absorber layers, a diplexer, VSWR monitoring, a magnetic breakaway connector, SDR/Raspberry Pi processing, and helmet-to-helmet mesh communication.

## Running the simulator

The simulator is a standalone HTML file using Three.js and GSAP from CDN-hosted libraries.

1. Open `src/conform-x-simulator.html` in a modern web browser.
2. Ensure internet access is available so the Three.js and GSAP CDN dependencies can load.
3. Use the controls to switch between the legacy vest whip and proposed helmet conformal array views.
4. Use the UHF voice and L-band video/data controls to visualize the illustrative transmission behavior.

> Note: The simulator's particle flow is illustrative and is not an RF electromagnetic solver.

## Source documentation

The project documentation and schematic in this repository are based on the files supplied with this project.

## Supplied README content

Idea Description

CONFORM-X is a helmet-mounted conformal antenna system designed for tactical teams operating in urban close-quarter battle (CQB) environments. In such areas, traditional vest-mounted whip antennas can snag on doors, windows, and other obstacles during fast movement. Their low position can also cause signal weakening inside concrete and steel structures.

Our idea is to make the helmet part of the communication system. CONFORM-X uses six thin and flexible antenna elements placed around the helmet surface. This creates a low-profile design without a large antenna sticking out. The antenna is designed to fit on a non-structural helmet cover without modifying the ballistic shell.

The system has two communication paths. UHF is used for voice communication with existing tactical radios, while the 1.28 GHz L-band is used for video and data transmission. The L-band elements work as an array to direct signals toward the required direction. The system can also support helmet-to-helmet mesh communication when walls or other obstacles block a direct connection.

For safety and signal control, CONFORM-X uses an AMC/HIS backing layer and RF absorber to direct radiation outward and reduce radiation toward the operator's head. A diplexer separates the UHF and L-band signals, while an SDR and Raspberry Pi handle L-band video and data processing. Heavy components such as the battery and processing units can remain on the vest, keeping the helmet lightweight.

The system also includes VSWR monitoring for antenna fault detection and a magnetic breakaway connector for safer cable handling. Key challenges such as helmet curvature, limited antenna space, and interference between frequency bands are addressed through antenna tuning, filtering, careful element placement, and RF testing.

Abstract

CONFORM-X is a helmet-mounted conformal antenna system developed for tactical teams operating in urban close-quarter battle environments. During such operations, communication can become difficult because conventional vest-mounted whip antennas are rigid, protruding, and more likely to snag on doors, windows, and other obstacles. Their low position can also lead to signal attenuation and fading inside reinforced concrete and steel structures.

The proposed system integrates the antenna with the helmet instead of using a large external whip. It uses six thin, flexible antenna elements that follow the curved helmet surface. The design supports two communication paths: UHF for tactical voice communication and 1.28 GHz L-band for video and data transmission. The L-band elements work as an array to help control the direction of the transmitted signal. The system can also support helmet-to-helmet mesh relay when direct communication is blocked by walls or other obstacles.

For radiation control, CONFORM-X uses an Artificial Magnetic Conductor (AMC) / High-Impedance Surface (HIS) layer with an RF absorber. This structure is designed to direct radiation upward and outward rather than toward the operator's head. A diplexer separates the UHF and L-band signals, while an SDR and Raspberry Pi handle the L-band video and data path. The heavier electronics and battery can remain on the vest or belt to reduce the load on the helmet.

The system also includes a magnetic breakaway connector for safer cable handling and MCU-based VSWR monitoring to detect antenna faults. Key engineering challenges include antenna detuning caused by helmet curvature, limited space for the antenna elements, and possible interaction between UHF and L-band systems. These are addressed through precision tuning, matching, filtering, careful array configuration, and RF testing.

Overall, CONFORM-X aims to provide a low-profile, flexible and practical communication platform that supports voice, video and data while remaining integrated with the operator's protective equipment.
