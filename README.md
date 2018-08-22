## UWG Matlab version
Urban Weather Generator (UWG)

Repository for keeping versions of UWG Matlab code based on Bruno Bueno's PhD work with Leslie K. Norford at MIT.

As of 2018, only the Excel interface (i.e., xlsm file) can be used in the UWG Matlab version. The newest UWG is now written in Python and embedded in the Dragonfly plugin for Grasshopper with various input file formats. See more details at: <https://github.com/chriswmackey/Dragonfly>.


### Implementation
* Initiate the UWG.m function
* Select the input .epw and .xlsm files ('...\data\') as well as the save location for the output .epw file.
* If the output .epw file is enabled in the input Excel interface, it will become available in the selected location after the simulation. If not [default], it will not show up even though you may have selected a save location.
* If the output .xlsx file is enabled in the input Excel interface [default], it will become available as '...\output\UWGoutput.xlsx' after the simulation. If not, it will not show up.

### Known Issues
All inquiries generally fall into two categories:
* Matlab Runtime - when running the executable version of the file, the correct Matlab Runtime version is also required, which has changed with the UWG updates. The latest compiled version was compiled in with Matlab R2015b in Windows 64bit environment and requires Matlab Runtime 9.0. The installation file will prompt to identify and download the correct version if not already installed. For other operating systems, the Matlab code should be re-packaged to generate the correct executable version as needed.

* Layer Thickness - The UWG uses explicit time-step and thus having a wall or roof layer such as membrane that is too thin, or a layer will high thermal conductivity (e.g. metal decking) will result in fatal error. These layers should be incorporated into a single layer that is representative of the overall optical property, thermal conductivity and thermal capacitance. 


### Contact
Leslie K. Norford, PhD<br/>
George Macomber (1948) Professor in Construction Management<br/>
Massachusetts Institute of Technology<br/>
<lnorford@mit.edu>


### History
* Sep, 2018 - A UWG model tested in Abu Dhabi, based on Jiachen Mao's SM thesis (2018). Only the Excel interface can be used in the Matlab version.
* June, 2016 - UWG updated based on Joseph Yang's SM thesis (2016). Changes include addition of three input file format (XML, Matlab, Excel), and update of the internal algorithm. 
* Oct, 2015 - Github Repository created by Joseph Yang with latest version of UWG, based on Aiko Nakano's SM thesis (2015).
* Sep, 2012 - Urban Weather Generator (UWG) created, based on Bruno Bueno's PhD thesis (2012).
