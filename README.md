### Ary

Firmware and Rust, mostly. Lately a lot of USB HID.

**[cyclone2](https://github.com/dank0i/cyclone2)** - GameSir Cyclone 2, a JieLi BR23 pad. I pulled
the firmware, patched it for battery and LED over Bluetooth, and raised the 2.4G report rate. The Pi
half fakes an Xbox 360 receiver so the pad shows up as XInput on Windows. The Ghidra module for
these chips renders byte-load addresses wrong, that's documented in there too.

**[pc-bridge](https://github.com/dank0i/pc-bridge)** - Rust agent, puts my gaming PC in Home
Assistant over MQTT. Game detection, sleep state, remote launch, wake-on-LAN.

**[controllernav](https://github.com/dank0i/controllernav)** - Discord with a controller. I built it
because I game from bed.

Open to software engineering roles.
