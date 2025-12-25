# Linux-SDR

## Table of Contents
- [Interfacing SDR with Linux](#interfacing-sdr-with-linux)
- [Decoding Tools for SDR](#decoding-tools-for-sdr)
  - [GSM/Cellular](#gsmcellular)
  - [Satellite](#satellite)
  - [AIS and Marine](#ais-and-marine)
  - [ADS-B and Aviation](#ads-b-and-aviation)
  - [Digital Voice](#digital-voice)
  - [Others](#others)
- [Linux Distros for SDR Prebuilts](#linux-distros-for-sdr-prebuilts)
- [SDR Hardware](#sdr-hardware)
- [SDR Antennas and Accessories](#sdr-antennas-and-accessories)
  - [Antenna Design Tools](#antenna-design-tools)
  - [Antenna Switches](#antenna-switches)
  - [Antenna Rotators](#antenna-rotators)
- [Tutorials and Documentation](#tutorials-and-documentation)
- [Community and Support](#community-and-support)
- [Contributing](#contributing)

---

## Interfacing SDR with Linux

A comprehensive list of SDR tools for Linux covering a variety of applications.

- **[GNU Radio](https://www.gnuradio.org/)** - A free and open-source software development toolkit that provides signal processing blocks to implement SDR systems. *(Open-Source)*
- **[SDRangel](https://github.com/f4exb/sdrangel)** - Versatile SDR software with a modular design supporting various devices and advanced signal processing. *(Latest Release: v3.12, August 2023)*
- **[SDRplay SDRUno](https://www.sdrplay.com/sdruno/)** - A powerful SDR application designed for SDRplay's range of SDR receivers, offering advanced features, an intuitive user interface, and regular updates.
- **[CubicSDR](https://cubicsdr.com/)** - A multi-platform SDR application that supports various SDR devices and offers features like spectrum display and waterfall visualization.
- **[GQRX](https://gqrx.dk/)** - An open-source SDR receiver powered by GNU Radio, providing a graphical interface and support for numerous SDR hardware options.
- **[SoapySDR](https://github.com/pothosware/SoapySDR)** - A vendor-neutral SDR software abstraction layer enabling compatibility between SDR hardware and various SDR applications.
- **[LinHPSDR](https://openhpsdr.org/)** - An SDR application based on the HPSDR Hermes board, providing support for high-performance SDR receivers.
- **[OpenWebRx+](https://luarvique.github.io/ppa/)** - A multi-user SDR receiver application that supports various SDR hardware and offers a simple web interface for remote access.
- **[Thetis](https://github.com/TAPR/OpenHPSDR-Thetis)** - A multi-platform SDR application supporting HPSDR Mercury, Penelope, and Excalibur hardware, offering advanced features and a customizable user interface.
- **[QSpectrumAnalyzer](https://github.com/xmikos/qspectrumanalyzer)** - A real-time spectrum analyzer integrated with GNU Radio for advanced signal visualization.
- **[SDRangelino](https://github.com/f4exb/sdrangelino)** - A lightweight SDR application optimized for embedded systems, offering essential signal processing features.
- **[DesktopHPSDR](https://github.com/dl1bz/deskhpsdr)** - A fork on PIHPSDR made for desktop use with some improvements 

---

## Decoding Tools for SDR

Categorized by application for easier navigation.

### GSM/Cellular
- **[gr-gsm](https://github.com/ptrkrysik/gr-gsm)** - Decode GSM/3G/4G LTE base stations using GNU Radio.
- **[gr-lte](https://github.com/kit-cel/gr-lte)** - Decode LTE base stations with GNU Radio.

### Satellite
- **[gr-iridium](https://github.com/daniestevez/gr-iridium)** - Decode Iridium satellite signals using GNU Radio.
- **[gr-satellites](https://github.com/daniestevez/gr-satellites)** - Decode various satellite signals with GNU Radio.

### AIS and Marine
- **[gr-ais](https://github.com/bistromath/gr-ais)** - Decode AIS (Automatic Identification System) signals using GNU Radio.
- **[rtl_ais](https://github.com/dgiardini/rtl-ais)** - Decode AIS signals with RTL-SDR.

### ADS-B and Aviation
- **[dump1090](https://github.com/antirez/dump1090)** - Decode ADS-B (Automatic Dependent Surveillance-Broadcast) signals.
- **[gr-air-modes](https://www.cgran.org/wiki/gr-air-modes)** - Decode ADS-B signals using GNU Radio with RTL-SDR support.

### Digital Voice
- **[dsd](https://github.com/szechyjs/dsd)** - Decode digital voice protocols such as P25 and DMR.
- **[SDRTrunk](https://github.com/DSheirer/sdrtrunk)** - Decode P25, DMR, and other digital voice protocols.

### Others
- **[multimon-ng](https://github.com/EliasOenal/multimon-ng)** - Decode a variety of digital transmission modes.
- **[QRadioLink](https://github.com/qradiolink/qradiolink)** - A VOIP GNU/Linux SDR transceiver application using Internet protocols.
- **[WSJT-X](https://physics.princeton.edu/pulsar/k1jt/wsjtx.html)** - Decode weak signals in amateur radio.
- **[fldigi](http://www.w1hkj.com/)** - Decode a variety of digital transmission modes.
- **[flrig](http://www.w1hkj.com/flrig-help/)** - Control amateur radio transceivers.
- **[xastir](https://xastir.org/index.php/Main_Page)** - Decode APRS (Automatic Packet Reporting System) signals.
- **[RaspberryNoAA2](https://github.com/jekhokie/raspberry-noaa-v2)** - Capture NOAA and Meteor-M2 satellite imagery on Raspberry Pi.
- **[gr-pocsag](https://www.cgran.org/browser/projects/gr-pocsag/trunk)** - Decode POCSAG pager signals using GNU Radio.
- **[multimode RX](https://www.cgran.org/browser/projects/multimode/trunk)** - A GNU Radio flowgraph for multimode reception.
- **[simple_fm_rvc](https://www.cgran.org/browser/projects/simple_fm_rcv/trunk)** - A simple FM receiver flowgraph.
- **[python-librtlsdr](https://github.com/dbasden/python-librtlsdr)** - Python wrapper for RTL-SDR.
- **[pyrtlsdr](https://github.com/roger-/pyrtlsdr)** - Another Python wrapper for RTL-SDR.
- **[rtlsdr-waterfall](https://github.com/keenerd/rtlsdr-waterfall)** - Python FFT GUI for RTL-SDR.
- **[Wireless Temp. Sensor RX](https://github.com/kevinmehall/rtlsdr-433m-sensor)** - GNU Radio app for wireless temperature sensors.
- **[QtRadio](http://napan.ca/ghpsdr3/index.php/RTL-SDR)** - SDR graphical user interface.
- **[SDR# (SDRSharp)](http://sdrsharp.com/)** - Popular SDR GUI primarily for Windows, with Linux guides available.
- **[tetra_demod_fft](https://www.cgran.org/browser/projects/tetra_demod_fft)** - TETRA trunking signal demodulation using GNU Radio.
- **[airprobe](http://git.gnumonks.org/cgi-bin/gitweb.cgi?p=airprobe.git)** - GSM sniffer tool.
- **[Linrad](http://www.nitehawk.com/sm5bsz/linuxdsp/hware/rtlsdr/rtlsdr.htm)** - SDR GUI with DAGC changes applied to librtlsdr master.
- **[gr-ais (fork)](https://github.com/chgans/gr-ais)** - Forked version of gr-ais for AIS reception.
- **[GNSS-SDR](http://www.gnss-sdr.org/)** - Real-time GPS signal processing.
- **[LTE-Cell-Scanner](https://github.com/Evrytania/LTE-Cell-Scanner)** - LTE scanner and tracker.
  - **[LTE-Cell-Scanner OpenCL accelerated](https://github.com/JiaoXianjun/LTE-Cell-Scanner)** - OpenCL-accelerated version for enhanced performance.
- **[Simulink-RTL-SDR](http://www.cel.kit.edu/simulink_rtl_sdr.php)** - MATLAB/Simulink wrapper for RTL-SDR.
- **[gr-scan](http://www.techmeology.co.uk/gr-scan/)** - Scanner flowgraph for GNU Radio.
- **[kalibrate-rtl](https://github.com/steve-m/kalibrate-rtl)** - Calibration tool *(Windows build available)*.
- **[pocsag-mrt](https://github.com/iZsh/pocsag-mrt)** - Multichannel real-time POCSAG decoder.
- **[adsb#](http://sdrsharp.com/index.php/a-simple-and-cheap-ads-b-receiver-using-rtl-sdr)** - ADS-B receiver guide using RTL-SDR.
- **[osmo-gmr-rtl](https://osmocom.org/projects/gmr/wiki/GettingStarted#RTLSDRdongles)** - GMR1 receiver setup with RTL-SDR dongles.
- **[dump1090](https://github.com/antirez/dump1090)** - ADS-B receiver.
- **[rtl_433](https://github.com/merbanan/rtl_433)** - Temperature sensor receiver.
- **[randio](https://github.com/michelp/randio)** - Random number generator using SDR.
- **[gr-wmbus](https://github.com/oWCTejLVlFyNztcBnOoh/gr-wmbus)** - Decode m-bus (EN 13757-4) signals.
- **[ec3k](https://github.com/avian2/ec3k)** - EnergyCount 3000 receiver.
- **[RTLSDR-Scanner](https://github.com/EarToEarOak/RTLSDR-Scanner)** - Radio scanner application.
- **[simple_ra](https://cgran.org/wiki/simple_ra)** - Radio astronomy application.
- **[rtlizer](https://github.com/csete/rtlizer)** - Spectrum analyzer for RTL-SDR.
- **[FS20_decode](https://github.com/eT0M/rtl_sdr_FS20_decoder)** - FS20 decoder for home automation signals.
- **[OpenLTE](http://sourceforge.net/p/openlte/home/Home/)** - LTE toolkit for research and development.
- **[rtltcpaccess](https://github.com/steve-m/rtltcpaccess)** - DAB compatibility layer.
- **[SDR-J](http://www.sdr-j.tk)** - "Analog" SDR & DAB receiver.
- **[gortlsdr](https://github.com/jpoirier/gortlsdr)** - Golang wrapper for RTL-SDR.
- **[gr-rds (fork)](https://github.com/bastibl/gr-rds)** - RDS + WBFM receiver using GNU Radio.
- **[acarsdec](http://sourceforge.net/projects/acarsdec/)** - ACARS decoder for aircraft communications.
- **[rtl-sdr-airband](https://github.com/microtony/RTLSDR-Airband)** - Air band receiver and ATIS decoding.

---

## Linux Distros for SDR Prebuilts

A selection of Linux distributions tailored for SDR applications, penetration testing, and digital forensics.

1. **[Ham Radio Linux](https://sourceforge.net/projects/hamradiolinux/)** - A Linux distribution for amateur radio operators based on Ubuntu.
2. **[Raspbian Ham Radio](https://sourceforge.net/projects/raspberry-pi-amateur-radio-g4klx/)** - A Linux distribution for amateur radio on Raspberry Pi OS.
3. **[Kali Linux](https://www.kali.org/)** - A distribution for penetration testing and security auditing with various SDR tools.
4. **[Pentoo](https://www.pentoo.ch/)** - A penetration testing distribution with integrated SDR tools.
5. **[Parrot OS](https://parrotlinux.org/)** - A security-focused distribution including a range of SDR applications.
6. **[BlackArch](https://blackarch.org/)** - A penetration testing distribution with extensive SDR toolsets.
7. **[BackBox](https://backbox.org/)** - A Linux distribution for penetration testing with built-in SDR utilities.
8. **[Dracos Linux](https://dracos-linux.org/)** - A penetration testing distribution featuring various SDR tools.
9. **[NST](https://www.networksecuritytoolkit.org/)** - A network security toolkit with integrated SDR applications.
10. **[CAINE](https://www.caine-live.net/)** - A digital forensics-focused distribution that includes SDR tools.
11. **[Kali NetHunter](https://www.kali.org/kali-linux-nethunter/)** - A mobile penetration testing platform with SDR capabilities.
12. **[Fedora Jam](https://getfedora.org/en/workstation/download/)** - A Fedora-based distribution with audio and SDR tools pre-installed for music and radio enthusiasts.

---

## SDR Hardware

A diverse list of SDR hardware options catering to various applications and performance needs.

1. **[RTL-SDR](https://www.rtl-sdr.com/)** - A popular, low-cost USB software-defined radio receiver.
2. **[HackRF One](https://greatscottgadgets.com/hackrf/)** - A wideband transceiver with a frequency range of 1 MHz to 6 GHz.
3. **[USRP B200](https://www.ettus.com/all-products/usrp-b200/)** - A versatile SDR with a frequency range of 70 MHz to 6 GHz.
4. **[FunCube Dongle Pro+](https://www.funcubedongle.com/)** - A high-performance SDR with a frequency range of 150 kHz to 1.9 GHz.
5. **[Airspy Mini](https://airspy.com/airspy-mini/)** - A compact SDR with a frequency range of 24 MHz to 1.8 GHz.
6. **[Ettus Research USRP N210](https://www.ettus.com/all-products/usrp-n210/)** - A high-performance SDR with a frequency range of 10 MHz to 6 GHz.
7. **[BeagleBone SDR](https://beagleboard.org/sdr)** - An SDR module designed for the BeagleBone platform.
8. **[LimeSDR](https://limemicro.com/products/limesdr/)** - A versatile SDR with a frequency range of 100 kHz to 3.8 GHz.
9. **[ADALM-PLUTO](https://www.analog.com/en/design-center/evaluation-hardware-and-software/evaluation-boards-kits/adalm-pluto.html)** - A portable SDR with a frequency range of 325 MHz to 3.8 GHz.
10. **[XTRX](https://xtrx.io/)** - A high-performance SDR with a frequency range of 30 MHz to 3.8 GHz.
11. **[Red Pitaya](https://www.redpitaya.com/)** - A programmable SDR platform with a frequency range of 10 MHz to 1 GHz.
12. **[Raspberry Pi with RTL-SDR](https://www.raspberrypi.org/)** - An SDR setup using a Raspberry Pi and RTL-SDR dongle.
13. **[SDRplay RSP1A](https://www.sdrplay.com/rsp1a/)** - A versatile SDR with a frequency range of 1 kHz to 2 GHz.
14. **[Xilinx ZCU102](https://www.xilinx.com/products/boards-and-kits/ek-u1-zcu102-g.html)** - An SDR development board with a high-performance FPGA.
15. **[Nutaq PicoSDR](https://nutaq.com/product/picosdr/)** - A compact SDR with a frequency range of 300 MHz to 3.8 GHz.
16. **[ADALM-2000](https://www.analog.com/en/design-center/evaluation-hardware-and-software/evaluation-boards-kits/adalmlogic.html)** - An SDR development board with a frequency range of 0 MHz to 50 MHz.
17. **[mPCIe SDR](https://www.microchip.com/wwwproducts/en/ATSAM9G20)** - A compact SDR module designed for use with mPCIe interfaces.
18. **[NI USRP B210](https://www.ni.com/en-us/support/model.usrp-b210.html)** - A high-performance SDR with a frequency range of 70 MHz to 6 GHz.
19. **[Tango](https://www.analog.com/en/design-center/evaluation-hardware-and-software/evaluation-boards-kits/tango.html)** - A versatile SDR with a frequency range of 500 MHz to 6 GHz.
20. **[Teleradio P104](https://www.tele-radio.com/products/p104/)** - A compact SDR with a frequency range of 0 MHz to 1.5 GHz.
21. **[NetSDR](https://www.winradio.com/NetSDR.html)** - A high-performance SDR with a frequency range of 10 kHz to 2 GHz.
22. **[LabSat 3](https://www.labsat.co.uk/products/labsat-3/)** - A compact SDR designed for GNSS signal simulation.
23. **[Quake SDR](https://www.quake.com/products/sdr/)** - A high-performance SDR with a frequency range of 10 MHz to 6 GHz.
24. **[RFSPACE SDR-14](http://www.rfspace.com/sdr-14/)** - A high-performance SDR with a frequency range of 10 kHz to 2 GHz.
25. **[IRIS](https://www.kacst.edu.sa/EN/Research/Pages/IRIS.aspx)** - A versatile SDR with a frequency range of 10 MHz to 2.6 GHz.
26. **[KX3](https://elecraft.com/kx3.html)** - A portable SDR with a frequency range of 160 meters to 10 meters.
27. **[FTDI Synchronous](https://www.ftdichip.com/Products/ICs/FT2232H.html)** - An SDR module designed for use with FTDI synchronous serial interfaces.
28. **[Siano SMSC](https://www.siano.com/products/)** - A versatile SDR with a frequency range of 50 MHz to 2.7 GHz.
29. **[LimeSDR Mini](https://limemicro.com/products/boards/limesdr-mini/)** - A compact SDR with a frequency range of 10 MHz to 3.5 GHz.
30. **[BladeRF 2.0](https://www.nuand.com/bladeRF-2/)** - An advanced SDR with an extended frequency range, improved performance, and additional I/O capabilities.

---

## SDR Antennas and Accessories

### Antenna Types and Accessories

1. **[RTL-SDR Blog 1090 MHz ADS-B Antenna](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-1090-mhz-ads-b-antenna/)** - Optimized for receiving ADS-B signals from aircraft.
2. **[RTL-SDR Blog 1090 MHz ADS-B LNA](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-1090-mhz-ads-b-lna/)** - A low-noise amplifier to boost ADS-B signal reception.
3. **[RTL-SDR Blog 1090 MHz ADS-B Filtered LNA](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-1090-mhz-ads-b-filtered-lna/)** - Enhanced LNA with filtering for better ADS-B reception.
4. **[RTL-SDR Blog 1090 MHz ADS-B Ceramic Filtered Preamp](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-1090-mhz-ads-b-ceramic-filtered-preamp/)** - Preamp with ceramic filters for improved ADS-B signal clarity.
5. **[RTL-SDR Blog 1090 MHz ADS-B Triple Filtered LNA](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-1090-mhz-ads-b-triple-filtered-lna/)** - Triple-filtered LNA for enhanced ADS-B performance.
6. **[RTL-SDR Blog 1090 MHz ADS-B Outdoor Antenna](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-1090-mhz-ads-b-outdoor-antenna/)** - Outdoor antenna designed for optimal ADS-B signal reception.
7. **[RTL-SDR Blog 1090 MHz ADS-B Antenna Tripod Mount](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-1090-mhz-ads-b-antenna-tripod-mount/)** - Mounting solution for ADS-B antennas.
8. **[LNA4ALL](https://lna4all.blogspot.com/)** - A low-cost wideband low-noise amplifier compatible with various SDRs.
9. **[Mini-Whip](https://www.nonstopsystems.com/radio/frank_radio_antenna_active_miniwhip.htm)** - A low-cost active antenna suitable for SDR applications.
10. **[Diamond Discone Antenna](https://www.diamondantenna.net/d130nj.html)** - A wideband discone antenna for versatile SDR usage.
11. **[Youloop](https://www.nonstopsystems.com/radio/frank_radio_antenna_loop.htm)** - A low-cost passive loop antenna compatible with SDRs.
12. **[RTL-SDR Blog SMA Pigtail Antenna Set](https://www.rtl-sdr.com/new-product-rtl-sdr-blog-sma-pigtail-antenna-set/)** - A set of SMA pigtail antennas for various SDR applications.

### Antenna Design Tools

1. **[4nec2](http://www.qsl.net/4nec2/)** - A free NEC-based antenna modeler and optimizer.
2. **[MMANA-GAL](http://hamsoft.ca/pages/mmana-gal.php)** - A free MMANA-GAL-based antenna modeler and optimizer.
3. **[EZNEC](https://www.eznec.com/)** - A commercial NEC-based antenna modeler and optimizer.
4. **[NanoVNA](https://nanorfe.com/)** - A low-cost vector network analyzer for measuring antenna performance.

### Antenna Switches

1. **[DX Engineering](https://www.dxengineering.com/)** - A variety of antenna switches for HF, VHF, and UHF bands.
2. **[MFJ Enterprises](https://www.mfjenterprises.com/)** - A range of antenna switches catering to different frequency bands.

### Antenna Rotators

1. **[Yaesu](https://www.yaesu.com/)** - A selection of antenna rotators suitable for HF, VHF, and UHF frequencies.
2. **[Alfa Radio](https://www.alfaradio.ca/)** - Various antenna rotators designed for different SDR applications.

---

## Tutorials and Documentation

1. **[GNU Radio Tutorials](https://wiki.gnuradio.org/index.php/Tutorials)** - Comprehensive guides for getting started with GNU Radio.
2. **[RTL-SDR Wiki](https://www.rtl-sdr.com/wiki/)** - Extensive resources and tutorials for using RTL-SDR hardware.
3. **[SDRplay SDRUno User Guide](https://www.sdrplay.com/docs/sdruno/)** - Detailed documentation for SDRplay SDRUno software.
4. **[CubicSDR Documentation](https://cubicsdr.com/docs/)** - Guides and documentation for using CubicSDR.
5. **[SDRangel Wiki](https://wiki.sdrangel.org/)** - Documentation and user guides for SDRangel.

---

## Community and Support

1. **[Reddit r/RTLSDR](https://www.reddit.com/r/RTLSDR/)** - A community for RTL-SDR users to discuss and seek help.
2. **[GNU Radio Mailing List](https://lists.gnu.org/mailman/listinfo/discuss-gnuradio)** - Official mailing list for GNU Radio discussions.
3. **[SDR Forum](https://sdr-forum.com/)** - A forum dedicated to SDR enthusiasts and professionals.
4. **[RTL-SDR Discord](https://discord.gg/rtlsdr)** - A Discord server for real-time discussions and support.
5. **[Stack Overflow SDR Tag](https://stackoverflow.com/questions/tagged/sdr)** - Q&A for SDR-related programming and technical issues.

---


