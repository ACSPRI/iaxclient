 
IAXClient library
=================

For more information read the original README file.
This software package is a stripped down version, which only
includes the original library, and the GSM / Speex codecs.
Intended for usage on the GNU/Linux operating system, audio
drivers for Pulseaudio have been added, along with a transition
to the CMake build system. Some features from the original package
are no longer usable. The library is compiled with a static linking
option. Pulseaudio drivers are enabled by default. The Portaudio 
and OpenAL drivers are no longer used or supported. ALSA is still
optional.

Building the library
====================

Install al prerequisites before attempting to compile.
Pulseaudio development headers are additionally required.
Building outside of the main source tree is encouraged.
<pre>
sudo apt-get install build-essential cmake libpulse-dev
mkdir build/
cd build/
cmake ../lib
make
</pre>

Link with your project using -liaxclient_lib.

Building the client
===================
The client included here is the original "simpleclient"
that appeared in the original iaxclient package. It can
be used as a command line, auto answering IAX client.

<pre>
cd ..
cd simpleclient
make
</pre>

License information
===================

Original licenses for each component apply. Additionally, the
Pulseaudio drivers are released under the GPLv2 license.
