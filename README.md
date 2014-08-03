# opencv-dsp-acceleration

This is a clone project from
http://code.google.com/p/opencv-dsp-acceleration/

## Introduction

Use of optimized computer vision algorithms are vital to meet real-time
requirements of popular mobile platform like Beagleboard which use OMAP3530.
OpenCV is one of the extensively used computer vision library today. This
library is optimized to take advantage of Intel architecture. However, when
working on mobile platform like OMAP35x which also house heterogeneous DSP
core C64x+, it is desired that this library give better performance using
the on-chip DSP core. This project aims no narrow down this gap by porting
low-level OpenCV API over DSP core.

The execution of this project will be carried out in two phase. In phase one
, some of the low-level OpenCV API like cvDFT(), cvSobel(), cvAvgSdv() and
cvIntegral() will be ported to DSP. In phase two, an application that make
use of these accelerated libraries will be built to demonstrate the success
of the project.

## Licensing
It is freely redistributable under the new BSD License.

 * Copyright (c) 2010, ktmp <ktmp...@gmail.com>
 * Copyright (c) 2014, Viller Hsiao <villerhsiao@gmail.com>

All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors
   may be used to endorse or promote products derived from this software without
   specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
