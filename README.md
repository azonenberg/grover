# What is it?

Fully open source (3-clause BSD licensed) headless bit error rate tester (BERT).

1U rackmount form factor with 1000baseT or 10Gbase-R interface to client PC.

Currently under development and not yet usable.

# What can it do?

(Planned)

* Generate PRBS patterns (PRBS7, PRBS9, PRBS15, PRBS23, PRBS31)
* Measure BER of incoming PRBS patterns
* Replay custom 8b/10b, 64/66b, and other common serial data streams
* Capture incoming serial data for protocol decoding (high speed serial logic/protocol analyzer)
* Generate trigger pulses based on serial data streams
* Display eye patterns of serial data
* Possibly usable as a sampling oscilloscope for serial data streams

# What's the max data rate?

Depends on what FPGA is loaded (any UltraScale+ in the B676 package will work)

# Where's the software?

ngscopeclient and libscopehal (https://github.com/ngscopeclient/scopehal-apps/)

# Why the name?

Because I already had a commercial BERT in my lab with hostname "ernie".
