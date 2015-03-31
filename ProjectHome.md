# Overview #
**nfex** is a tool for extracting files from the network in real-time or post-capture from an offline tcpdump pcap savefile. It is based off of the code-base from the apparently defunct project [tcpxtract](http://tcpxtract.sourceforge.net).

nfex offers:

  * Asynchronous user/event-driven interface
  * Real-time or offline file extraction
  * Custom written search algorithm is lightning fast and very scalable
  * Search algorithm scales across packet boundaries for total coverage and forensic quality
  * Support for 27 file formats
  * A simple, repeatable way to add new file formats by editing the configuration file (post compilation)
  * GeoIP targeting support using the free [MaxMind](http://www.maxmind.com) [C API](http://www.maxmind.com/app/c)
  * Analysis tool for post extraction processing

# Compilation and Installation #

Build and install these fine libraries:
  * [libpcap](http://www.tcpdump.com)
  * [libnet](http://code.google.com/p/libnet)

Optionally build and install this guy:
  * [MaxMind GeoIP library](http://www.maxmind.com/app/c)

```
./configure && make
sudo make install
```
