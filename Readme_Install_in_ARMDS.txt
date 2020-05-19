Steps to install CMSIS Driver Validation pack into ARMDS
====================================================================
1. Get CMSIS Driver Validation pack for CM55 (https://github.com/sivadattu/CMSIS_Driver_Validation)
2. Install this pack in the ARMDS.
	- Open CMSIS Pack Manager view in ARM DS; click on folder icon(Import Existing Packs...) and select ARM.CMSIS-Driver_Validation.1.4.0.1.pack from Local_Release. 
	Note: Sometimes, Not sure why, DS is not able to extract the content of this pack; in that case, you need to manually extract the pack using 7z.
3. Create a new project.
	- File->New->Project...
	- Select "C project" under "C/C++" option; and click next
	- type the project name, Select "CMSIS C/C++ Project" under Project type; and "Arm Compiler 6" under Toolchains and click next
	- For device selection; click on ARM and select "ARMCM55" under ARM Cortex M55 and click finish.
4. In project Explorer window; double click on <projectname>.rteconfig file.
	In Components window:
	- Expand CMSIS Driver Validation
		- Select Drivers that needs to be tested.