# Zedboard_FMCOMMS2

""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
------------------------------ Interfacing zedboard with FMCOMMS2 (AD9361 transceiver) using NO OS------------------------
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

1) Download and make the files from the link https://wiki.analog.com/resources/fpga/docs/build
2) Extract the zip file and move to directory ..../hdl/projects/fmcomms2/zed/ and open the fmcomms2_zed.xpr file with "Vivado 2018.3" or higher. (For using versions lower than 2018.3, first check how to downgrade 2018.3 files).
2) Click on open block diagram from "IP Integrator" menu.

""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
------------------------------------------------------------------- SDK ---------------------------------------------------------------
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

3) Bitstream is already generated in project. Click on "File", "Export" , "Export Hardware" and tick the "include bitstream".
4) Click on "Launch SDK" from "File" menu.
5) When SDK is opened, click on "File", "New Application project", name a project like "AD_ZB", click "Next" and finish.
6) Now expand the project folder and  find the folder "src". 
7) Select all files in folder ..../AD9361_using_SDK/SDK_files/ and drag to src folder. 
8) Click on drag down button from system debugger (Green icon) and run configurations. 
9) Left side, there is system debugger option. double click on it, Debug type "Standalone debug", tick the "reset entire FPGA", and tick the "ps7_cortexa" option. Then apply and run.
