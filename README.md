# What is it?

Fully open source (3-clause BSD licensed) headless bit error rate tester (BERT).

1U rackmount form factor with 1000baseT or 10Gbase-R interface to client PC.

Currently under early development (requirements identification and beginnings of schematic capture)

# What's the max data rate?

Depends on what FPGA is loaded (any UltraScale+ in the B676 package will work).

* Artix UltraScale+, any speed grade: 16.375 Gbps
* Kintex UltraScale+, -1 speed: 25.785 Gbps
* Kintex UltraScale+, -2 speed: 28.21 Gbps
* Kintex UltraScale+, -3 speed: 32.75 Gbps

# What ports are provided?

Back panel:
* DC power (24/48V DC on 6 pin Molex Mini-Fit Jr)
* Ethernet uplink (SFP+ / SFP28 or 1000baseT RJ45)
* RS232 debug console (Cisco style RJ45)
* SMA trigger out
* 10 MHz reference in

Front panel:
* 2x QSFP+ / QSFP28 (8 GTYs). If using an Artix FPGA, one of the two QSFP+ is unavailable.
* 2x SFP+ / SFP28 (2 GTYs)
* 4x paired 2.92mm (4x GTYs), pigtailed off SMPM connectors on the main board

This leaves one GTY unused.

# What can it do?

(Planned)

* Generate PRBS patterns (PRBS7, PRBS9, PRBS15, PRBS23, PRBS31)
* Measure BER of incoming PRBS patterns
* Replay custom 8b/10b, 64/66b, and other common serial data streams
* Capture incoming serial data for protocol decoding (high speed serial logic/protocol analyzer)
* Generate trigger pulses based on serial data streams
* Display eye patterns of serial data
* Possibly usable as a sampling oscilloscope for serial data streams

# Where's the software?

ngscopeclient and libscopehal (https://github.com/ngscopeclient/scopehal-apps/)

# Why the name?

Because I already had a commercial BERT in my lab with hostname "ernie".
