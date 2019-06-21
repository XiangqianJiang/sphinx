=================
Program Structure
=================

::

	===============================================================================
	========================== 2019/06/17 21:32:13.985 ============================
	==== BRANCH: Main                               TIME: Jul 12 2018 17:20:34 ====
	============= VERSION: 5.7.2.1706            Build Type: Release  =============
	== SM Software Revision: 2018.07.12-16.50-R5.7-72241
	== Log Source: rack index 0-Rack 0, Group 0, Dut 1
	==== HOST CONTROLLER NAME: MPT3000HES1030        IP ADDRESS: 10.71.42.90 ====
	===============================================================================


	Program:         specconfig.stil
	Program Folder:  C:\Users\tester\Desktop\OwenJiang\JIRA11_SpecConfig\SpecConfig.stil
	Time:            21 32 13            Date:    June 17, 2019

	2019-06-17 21:32:14= = = = = = = = = = = = = = = = = = = = STATE: START : BEGIN= = = = = = = = = = = = = = = = = = = =
	2019-06-17 21:32:14- - - - - - - - - - - - - - - - - - - - TEST: Init Testing Flow : BEGIN- - - - - - - - - - - - - - - - - - - -
	Parameter [Serial Number]: [A04F630A].
	Parameter [SKU]: [0TS1618].
	Parameter [Station Type]: [63].
	Parameter [Work Order]: [819354].
	Parameter [Operation ID]: [11].
	Parameter [LogLevel]: [3].
	Parameter [FW_ATTR]: [CUSTFW].
	Parameter [PSID]: [AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA].
	Parameter [UART LOG]: [0].
	[2019-06-17 21:32:14] <INFO> - DIB PN: G8003-66518
	[2019-06-17 21:32:14] <INFO> - TP REVISION: 1.0.0.70451
	[2019-06-17 21:32:14] <INFO> - TP working under NO_ENCODE mode
	[2019-06-17 21:32:14] <INFO> - Log Level is Info
	try to read cim string: 0
	try to read cim string: 1
	try to read cim string: 2
	Scan Information: [TPInit,SKU,UserID,WorkOrder,DUTSN:1,0TS1618,11,819354,A04F630A]
	[2019-06-17 21:32:17] <INFO> - gScanInfo: [DUTSN: A04F630A]
	[2019-06-17 21:32:17] <INFO> - gScanInfo: [SKU: 0TS1618]
	[2019-06-17 21:32:17] <INFO> - gScanInfo: [WorkOrder: 819354]
	[2019-06-17 21:32:17] <INFO> - gScanInfo: [UserID: 11]
	[2019-06-17 21:32:17] <INFO> - init sfc call
	ES mode, force CIM return pass. (no actual CIM supported)
	CIM call(getSysInfo - SLTVER;CIMVER;RACK;PRIM;SLOT;TESTER;WorkOrder;SKU;UserID;DUTSN;RECIPE;ActualVersion;WorkingMode;) return with no info (0)!
	[2019-06-17 21:32:17] <INFO> - ES MODE, skip read config info
	[2019-06-17 21:32:17] <INFO> - init report
	[2019-06-17 21:32:17] <INFO> - zip folder name: A04F630A_P_D1_HFT_2019-06-17_213217
	[2019-06-17 21:32:17] <INFO> - init parameter db
	[2019-06-17 21:32:17] <INFO> - Select File=/home/tester/userfiles/CUSTFW/aspen_generic_L000001G_5c674d3d012e_manifest.json
	[2019-06-17 21:32:17] <INFO> - 30 files defined in manifest json
	[2019-06-17 21:32:17] <INFO> - FW manifest parsing successfully from folder=CUSTFW
	[2019-06-17 21:32:17] <INFO> - write init csv
	[2019-06-17 21:32:17] <INFO> - end of init TB

	Init Testing Flow        Test Time(Secs): 3.008       Status:        0(Pass)
	2019-06-17 21:32:17- - - - - - - - - - - - - - - - - - - - TEST: Init Testing Flow : COMPLETE- - - - - - - - - - - - - - - - - - - -
	2019-06-17 21:32:17- - - - - - - - - - - - - - - - - - - - TEST: Power On : BEGIN- - - - - - - - - - - - - - - - - - - -
	Parameter [POV_12V_rail]: [12].
	Parameter [POV_5V_3_3V_rail]: [3.3].
	Parameter [PowerON_wait]: [10].
	Parameter [Notify]: [1].
	Parameter [Rescan]: [0].
	Parameter [Max Retry]: [0].
	Parameter [Delay_between_OffOn]: [5].
	Parameter [time_to_ready_limit]: [15].
	Parameter [Link Speed]: [3].
	[2019-06-17 21:32:17] <INFO> - Powering on device... notify = true power_on_wait = 10, rescan = 0
	[2019-06-17 21:32:17] <INFO> - dps channel 1 vol:12.000000
	[2019-06-17 21:32:17] <INFO> - Skipping setting Chan_3p3V voltage and current settings for 8U DIB...

	[2019-06-17 21:32:17] <INFO> - Setting E3 pin to high for 8U DIB...


	************************************
	PCIe Link Status :
	LinkUp          = true
	LTSSM           = 0x10, LTSSM_L0
	LinkWidth       = x4
	LinkSpeed       = 8.0G
	ActiveLanes     = 00001111 (0x0f)
	ValidLanes      = 00001111 (0x0f)
	LinkUpCount     = 1
	LinkRetrainCnt  = 3
	************************************
	[2019-06-17 21:32:27] <INFO> - Time to ready:9.408000s
	[2019-06-17 21:32:27] <INFO> - Device powered on...
	[2019-06-17 21:32:27] <INFO> - lba_open=46
	[2019-06-17 21:32:27] <INFO> - Device enumerated...

	Power On                 Test Time(Secs): 9.522       Status:        0(Pass)
	2019-06-17 21:32:27- - - - - - - - - - - - - - - - - - - - TEST: Power On : COMPLETE- - - - - - - - - - - - - - - - - - - -
	2019-06-17 21:32:27= = = = = = = = = = = = = = = = = = = = STATE: START : COMPLETE= = = = = = = = = = = = = = = = = = = =
	2019-06-17 21:32:27= = = = = = = = = = = = = = = = = = = = STATE: Step2 : BEGIN= = = = = = = = = = = = = = = = = = = =
	2019-06-17 21:32:27- - - - - - - - - - - - - - - - - - - - TEST: Spec Config : BEGIN- - - - - - - - - - - - - - - - - - - -
	Parameter [Customer]: [AWS].
	Parameter [Security]: [SED].
	Parameter [Capacity]: [512GB].
	Parameter [Form Factor]: [M.2].
	Parameter [JsonFolder]: [OOBAspen+].
	[2019-06-17 21:32:27] <INFO> - path = /home/tester/userfiles/OOBAspen+ 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_NVMeCommandSetSpecific.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_NVMeCapabilityNFeatures.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_NVMeAdminCommandSet.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_NVMeCommandSet.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_Power_State_Descriptors.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_Vendor_Specific.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_Namespace Identification Descriptor.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_GET_FEATURES.json 
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json 
	[2019-06-17 21:32:27] <INFO> -  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
	[2019-06-17 21:32:27] <INFO> -  ^^^^^^ Start Admin Test ^^^^^^
	[2019-06-17 21:32:27] <INFO> -  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
	[2019-06-17 21:32:27] <INFO> - 
			  Admin Cmd [0]
	[2019-06-17 21:32:27] <INFO> - Current Return Buff Size = 4096 bytes
	[2019-06-17 21:32:27] <INFO> - Send cmd[0]
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Composite Temperature
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [3] = Available Spare Threshold 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : A 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : a 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [5] = Data Units Read 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 2 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [6] = Data Units Write 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 2 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [7] = Host Read Commands 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 2E 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [8] = Host Write Commands 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 1E 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [10] = Power cycle 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 29 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [11] = Power On Hour 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 1A 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [12] = Unsafe Shutdown 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 3 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <INFO> - Current JsonFile : /home/tester/userfiles/OOBAspen+/configspec_GET LOG PAGE.json
	[2019-06-17 21:32:27] <ERROR> - <==Fail Item [14] = Number Of Error Log 
	[2019-06-17 21:32:27] <ERROR> - [Actual Value] 	  : 6 
	[2019-06-17 21:32:27] <ERROR> - [Expect Value]    : 0 
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 1
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 2
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 3
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 4
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 5
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 6
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 7
	[2019-06-17 21:32:27] <ERROR> - [#]SKIP  : Temperature Sensor 8
	[2019-06-17 21:32:27] <INFO> - Current Item Screen Fail !!!
	[2019-06-17 21:32:27] <ERROR> - Admin Spec config Excute Fail 
	[2019-06-17 21:32:27] <INFO> - 


	[2019-06-17 21:32:27] <INFO> -  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
	[2019-06-17 21:32:27] <INFO> -  ^^^^^^ Start LogPage3E Test ^^^^^^
	[2019-06-17 21:32:27] <INFO> -  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
	[2019-06-17 21:32:27] <INFO> - jsonFile = /home/tester/userfiles/OOBAspen+/configspec_LOG PAGE 3E.json 
	[2019-06-17 21:32:27] <INFO> - reply len: 5086
	[2019-06-17 21:32:27] <INFO>------Screen Attributes----------
	[2019-06-17 21:32:27] <INFO> - Current Item Screen Pass !!!
	[2019-06-17 21:32:27] <INFO> - Start write GetLogPage3E CSV
	[2019-06-17 21:32:27] <INFO> - Write LogPage3E Csv successfully!

	Spec Config              Test Time(Secs): 0.118       Status: 63926010(Spec Config-Data Mismatch)
	2019-06-17 21:32:27- - - - - - - - - - - - - - - - - - - - TEST: Spec Config : COMPLETE- - - - - - - - - - - - - - - - - - - -
	ERROR1: FlowWalk_Run failed to add StylusBin as return argument
	2019-06-17 21:32:27= = = = = = = = = = = = = = = = = = = = STATE: Step2 : COMPLETE= = = = = = = = = = = = = = = = = = = =
	2019-06-17 21:32:27= = = = = = = = = = = = = = = = = = = = STATE: PowerOff : BEGIN= = = = = = = = = = = = = = = = = = = =
	2019-06-17 21:32:27- - - - - - - - - - - - - - - - - - - - TEST: Power Off : BEGIN- - - - - - - - - - - - - - - - - - - -
	Parameter [Graceful]: [1].
	Parameter [PowerOFF_wait]: [0].
	[2019-06-17 21:32:27] <INFO> - Powering off device... graceful = true power_off_wait = 0
	Mon Jun 17 21:32:30 2019 block device removal detected.
	[2019-06-17 21:32:30] <INFO> - Setting E3 pin to low for 8U DIB...


	Power Off                Test Time(Secs): 3.129       Status:        0(Pass)
	2019-06-17 21:32:30- - - - - - - - - - - - - - - - - - - - TEST: Power Off : COMPLETE- - - - - - - - - - - - - - - - - - - -
	2019-06-17 21:32:30= = = = = = = = = = = = = = = = = = = = STATE: PowerOff : COMPLETE= = = = = = = = = = = = = = = = = = = =
	2019-06-17 21:32:30= = = = = = = = = = = = = = = = = = = = STATE: Free : BEGIN= = = = = = = = = = = = = = = = = = = =
	[2019-06-17 21:32:30] <INFO> - request: setTPErrorCode_32889001
	ES mode, force CIM return pass. (no actual CIM supported)
	CIM call(setTPErrorCode_32889001 - (null)) return with no info (0)!
	ES mode, force CIM return pass. (no actual CIM supported)
	CIM call(saveTestLog_A04F630A_P_D1_HFT_2019-06-17_213217.txt - (null)) return with no info (0)!
		zip warning: name not matched: A04F630A_P_D1_HFT_2019-06-17_213217/*

	zip error: Nothing to do! (try: zip -r A04F630A_P_D1_HFT_2019-06-17_213217.zip . -i A04F630A_P_D1_HFT_2019-06-17_213217/*)
	'cd /home/tester/userfiles/; zip -r A04F630A_P_D1_HFT_2019-06-17_213217.zip A04F630A_P_D1_HFT_2019-06-17_213217/* 2>&1' failed with exit code 12.
	ES mode, force CIM return pass. (no actual CIM supported)
	CIM call(FTPsaveReport_A04F630A_P_D1_HFT_2019-06-17_213217.csv - (null)) return with no info (0)!
	[2019-06-17 21:32:30] <INFO> - Deleting FA logs to free space
	cd /home/tester/userfiles/; rm A04F630A_P_D1_HFT_2019-06-17_213217.zip; rm -rf A04F630A_P_D1_HFT_2019-06-17_213217 2>&1 pass.
	[2019-06-17 21:32:30] <INFO> - ...End tp_free...

	   PASS    BIN:      1   PASS  TEST-TIME: 0:00:16.442




   