12jul2013 Chris Korda

Ported Steve Harris' LADSPA plugins 0.4.15 to 32-bit and 64-bit Windows.
Visual Studio 2008 or a later version is required to build this project.
Minor source modifications were made; they're commented with "// ck".
The modified source files are available at waveshop.sourceforge.net.
The unmodified source files are available at plugin.org.uk.

To build the plugins, open swh-plugins.sln in the swh-plugins folder,
use the Configuration Manager to select a configuration and platform,
and build the solution. All plugins should build (with some warnings).

The following plugins use FFTW (Fastest Fourier Transform in the West):
imp_1199
mbeq_1197
pitch_scale_1193
pitch_scale_1194
These four plugins depend on libfftw3f-3.dll and won't load without it.
The necessary files from FFTW 3.3.3 are included in this distribution.
If you prefer to download and/or build FFTW yourself, visit www.fftw.org.

This program is free software; you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the Free
Software Foundation; either version 2 of the License, or any later version.
