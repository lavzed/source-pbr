# Preamble
August 2022

This branch of thexas4 serves to add additional features into the PBR shader. This shader is an alternative to BlueFlytrap's mesh-stacking method, which achieves only a pseudo-PBR effect. I added the additional features below to correspond with humans made from Character Creator 3 and up.

### Features (or differences from main branch):
- Two extra bumpmaps
- Facial flexes
- Fixed alpha-test lighting
- Weird rimlight/subsurface-scattering implementation
- Bumptransform for micronormals

These features have rudimentary implementation; they have been made not with optimization 
in mind, rather to enhance my Garry's Mod artistry. I would like your thoughts on how 
you would better implement these changes. Thank you.

### Changed files:
- pbr_ps30.fxc
- pbr_vs30.fxc
- pbr_ps20b.fxc
- pbr_vs20.fxc
- pbr_dx9.cpp

## Installation
If you would like to have PBR in your Garry's Mod, make sure that you are not in the
x86-64 branch. Place the dll from \mp\game\mod_hl2mp\bin\ into the bin folder inside
the "garrysmod" folder (not the folder that contains hlmv or hlfaceposer). If there
isn't a bin folder in the "garrysmod" folder, make one.
Move the vcs files from \mp\game\mod_hl2mp\shaders\fxc into the corresponding
directory in the "garrysmod" folder (garrysmod\shaders\fxc). Again, make a folder if it is not there.

Thanks to thexas4 and his team for introducing (Unreal-like) PBR in Source Engine. 

##               SOURCE 1 SDK LICENSE
Source SDK Copyright(c) Valve Corp.  

THIS DOCUMENT DESCRIBES A CONTRACT BETWEEN YOU AND VALVE 
CORPORATION ("Valve").  PLEASE READ IT BEFORE DOWNLOADING OR USING 
THE SOURCE ENGINE SDK ("SDK"). BY DOWNLOADING AND/OR USING THE 
SOURCE ENGINE SDK YOU ACCEPT THIS LICENSE. IF YOU DO NOT AGREE TO 
THE TERMS OF THIS LICENSE PLEASE DON’T DOWNLOAD OR USE THE SDK.  

  You may, free of charge, download and use the SDK to develop a modified Valve game 
running on the Source engine.  You may distribute your modified Valve game in source and 
object code form, but only for free. Terms of use for Valve games are found in the Steam 
Subscriber Agreement located here: http://store.steampowered.com/subscriber_agreement/ 

  You may copy, modify, and distribute the SDK and any modifications you make to the 
SDK in source and object code form, but only for free.  Any distribution of this SDK must 
include this LICENSE file and thirdpartylegalnotices.txt.  
 
  Any distribution of the SDK or a substantial portion of the SDK must include the above 
copyright notice and the following: 

    DISCLAIMER OF WARRANTIES.  THE SOURCE SDK AND ANY 
    OTHER MATERIAL DOWNLOADED BY LICENSEE IS PROVIDED 
    "AS IS".  VALVE AND ITS SUPPLIERS DISCLAIM ALL 
    WARRANTIES WITH RESPECT TO THE SDK, EITHER EXPRESS 
    OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, IMPLIED 
    WARRANTIES OF MERCHANTABILITY, NON-INFRINGEMENT, 
    TITLE AND FITNESS FOR A PARTICULAR PURPOSE.  

    LIMITATION OF LIABILITY.  IN NO EVENT SHALL VALVE OR 
    ITS SUPPLIERS BE LIABLE FOR ANY SPECIAL, INCIDENTAL, 
    INDIRECT, OR CONSEQUENTIAL DAMAGES WHATSOEVER 
    (INCLUDING, WITHOUT LIMITATION, DAMAGES FOR LOSS OF 
    BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF 
    BUSINESS INFORMATION, OR ANY OTHER PECUNIARY LOSS) 
    ARISING OUT OF THE USE OF OR INABILITY TO USE THE 
    ENGINE AND/OR THE SDK, EVEN IF VALVE HAS BEEN 
    ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.  
 
       
If you would like to use the SDK for a commercial purpose, please contact Valve at 
sourceengine@valvesoftware.com.
