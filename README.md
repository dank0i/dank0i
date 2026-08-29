### Ary

Firmware and Rust, mostly. Lately a lot of USB HID.

**[pc-bridge](https://github.com/dank0i/pc-bridge)** - Rust agent, puts my gaming PC in Home
Assistant over MQTT. Game detection, sleep state, remote launch, wake-on-LAN. Recently a module
host, so personal automation runs as a supervised subprocess instead of living in the tree. Not a
DLL plugin: Rust has no stable ABI, and a plugin built against an older version loaded into a
self-updating binary doesn't error, it corrupts memory.

**[cyclone2](https://github.com/dank0i/cyclone2)** - GameSir Cyclone 2, a JieLi BR23 pad. I pulled
the firmware, patched it for battery and LED over Bluetooth, and raised the 2.4G report rate. The Pi
half fakes an Xbox 360 receiver so the pad shows up as XInput on Windows. The Ghidra module for
these chips renders byte-load addresses wrong, that's documented in there too.

**[sc3](https://github.com/dank0i/sc3)** - A FIFINE SC3 desk mixer sums its line in into the USB
mic send, so whoever I'm talking to hears themselves back. The vendor's update claims to fix that
and doesn't. The routing is in encrypted firmware, so I broke it: 81 of 87 sibling images ship
unencrypted, which makes it known-plaintext. All 315,654 words come out. It also reports one of its
four faders, so the patch exposes all four and I got the per-app volume mixer I'd been meaning to
build out of potentiometers.

**[football-forecast](https://github.com/dank0i/football-forecast)** - Forecasts 25,979 European
matches and scores the result against bookmaker odds instead of against nothing. Using no betting
data it gets 92% of the way to the market. Turns out the gap left over is missing information, not
a worse model. [Writeup](https://dank0i.github.io/football-forecast).

**[ledger](https://github.com/dank0i/ledger)** - Double-entry ledger, Spring Boot and React.
Idempotent posting, and row locks taken in consistent id order so concurrent postings don't race.

**[controllernav](https://github.com/dank0i/controllernav)** - Discord with a controller. I built it
because I game from bed.

More at [dank0i.github.io](https://dank0i.github.io). Open to software and ML engineering roles.
