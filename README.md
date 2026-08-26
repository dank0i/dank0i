# Ary

I make hardware do things it was not shipped to do, then wire the result into my house.

### [cyclone2](https://github.com/dank0i/cyclone2)

Reverse engineering a GameSir Cyclone 2, a game controller built on a JieLi BR23 SoC. Documents the
image layout, the instruction encodings, the timer subsystem, and four firmware patches that add
capabilities the stock firmware does not expose. It also documents four rendering defects in a
public Ghidra processor module, one of which silently corrupts global addresses, so anyone using it
reads wrong addresses without knowing.

The other half is a Raspberry Pi that presents the pad to Windows as an Xbox 360 Wireless Receiver,
giving native XInput with working rumble and battery, with nothing installed on the PC. Getting
output reports to flow at all required patching the kernel's `f_fs` module.

### [pc-bridge](https://github.com/dank0i/pc-bridge)

A Rust agent that exposes a gaming PC to Home Assistant over MQTT: event-driven game detection,
power and sleep state, remote launch, wake-on-LAN. Signed release binaries, and CI that runs
cargo-deny, gitleaks, trivy and semgrep on every push.

### [controllernav](https://github.com/dank0i/controllernav)

Navigate the Discord client with a game controller. Discord lets you bind push-to-talk to a gamepad
but gives you no way to move around the client with one. This adds a focus ring you drive with the
d-pad, and a virtual cursor for anything the ring cannot reach.

---

Currently looking for software engineering roles.
