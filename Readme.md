RF Analyzer for Android
=======================

This is the repository of the RF Analyzer app for Android. It can be used
to view a FFT plot and a waterfall plot of the frequency spectrum
received by a HackRF. The new version can also demodulate audio from
AM and FM signals!

![RF Analyzer](http://4.bp.blogspot.com/-gdSsQ1COybM/VEQkplyqFOI/AAAAAAAADt8/hJhA0i6WyYY/s0/RF%2BAnalyzer.jpg)

(photo by Dennis Mantz)

See [http://tech.mantz-it.com](http://tech.mantz-it.com) and [@dennismantz]
(https://twitter.com/dennismantz) for updates.

RF Analyzer is also available on Google Play: 
[https://play.google.com/store/apps/details?id=com.mantz_it.rfanalyzer]
(https://play.google.com/store/apps/details?id=com.mantz_it.rfanalyzer)

Implemented Features
--------------------
* Browse the spectrum by scrolling horizontally
* Zoom in and out, both horizontally and vertically
* Automatic re-tune while scrolling and zooming
* Auto scale the vertical axis
* Jump directly to a frequency
* Adjust the gain settings of the HackRF / RTL-SDR dongle
* Select a pre-recorded file as source instead of a real HackRF
* Change the FFT size
* Change FFT drawing mode: Line or Bars
* Waterfall color maps: JET, HOT, GQRX
* Peak hold
* Averaging
* Setting the frame rate either to a fixed value or to automatic control
* Activate logging and showing the log file
* Demodulate nFM, wFM, AM, LSB and USB with adjustable filters
* Adjust squelch and channel width
* Change the proportion of spectrum and waterfall
* Support for RTL-SDR dongles
* Record the raw IQ samples to a file and select files as source
* Select a fixed frequency shift (for upconverters)


Tested Devices
--------------

RF Analyzer uses the hackrf_android libaray. Have a look at the corresponding
repository for information about supported Android devices working with the HackRF:
[https://github.com/demantz/hackrf_android](https://github.com/demantz/hackrf_android)

RF Analyzer uses Martin Marinov's RTL2832U driver to use rtl-sdr dongles in Android.
It is a wrapper for the rtl_tcp tool from the rtl-sdr project. Information about
supported dongles can be found here:
[http://sdr.osmocom.org/trac/wiki/rtl-sdr](http://sdr.osmocom.org/trac/wiki/rtl-sdr)

Known Issues
------------
* HackRF: Strong aliasing images in some rare situations. Must be something wrong with the
  baseband filter width. But it's hard to reproduce.
* Low quality USB cables and OTG adapters might cause powering issues with the HackRF. If
  you can'com.t get your HackRF to work, maybe try a different cable and/or a powered USB hub!


Installation / Usage
--------------------
The app project in this repository was generated by Android Studio.
Use the 'import project' function in Android Studio to import the repository
as new project.

The RFAnalyzer.apk file is also in this repository so that it can be used without 
building it yourself. But it won'com.t be synched to the latest code base all the time.

A basic how-to-start can be found on this blog post:
[http://tech.mantz-it.com/2014/10/rf-analyzer-explore-frequency-spectrum.html]
(http://tech.mantz-it.com/2014/10/rf-analyzer-explore-frequency-spectrum.html)

Here is short screen record of the application in action:
[http://youtu.be/r36fd_QhpNM](http://youtu.be/r36fd_QhpNM)


License
-------
This library is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public
License as published by the Free Software Foundation; either
version 2 of the License, or (at your option) any later version.
[http://www.gnu.org/licenses/gpl.html](http://www.gnu.org/licenses/gpl.html) GPL version 2 or higher

principal author: Dennis Mantz <dennis.mantzgooglemail.com>
