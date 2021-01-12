# PolarisBiosEditor 1.7xml: fork with dumping additional data as XML in console.

Just open vbios file and look in console/stdout for extended xml output.
Editing functionality is identical to the upstream, no new features.


Please build the executable yourself if you don't trust

Prebuilt version works on linux with mono, just type `./run.sh`, also see that file fore dependncies
<details>
  <summary>Example XML output (large, ~1k lines)</summary>
<pre>
&lt;ATOM_ROM_HEADER of="0x224-0x250  len=0x2C=44"&gt;
  &lt;sHeader&gt;
    &lt;usStructureSize&gt;36 = 0x24 = 0b100100&lt;/usStructureSize&gt;
    &lt;ucTableFormatRevision&gt;1&lt;/ucTableFormatRevision&gt;
    &lt;ucTableContentRevision&gt;1&lt;/ucTableContentRevision&gt;
  &lt;/sHeader&gt;
  &lt;uaFirmWareSignature&gt;
    &lt;char&gt;65 = 0x41 = 0b1000001&lt;/char&gt;
    &lt;char&gt;84 = 0x54 = 0b1010100&lt;/char&gt;
    &lt;char&gt;79 = 0x4F = 0b1001111&lt;/char&gt;
    &lt;char&gt;77 = 0x4D = 0b1001101&lt;/char&gt;
  &lt;/uaFirmWareSignature&gt;
  &lt;usBiosRuntimeSegmentAddress&gt;49152 = 0xC000 = 0b1100000000000000&lt;/usBiosRuntimeSegmentAddress&gt;
  &lt;usProtectedModeInfoOffset&gt;969 = 0x3C9 = 0b1111001001&lt;/usProtectedModeInfoOffset&gt;
  &lt;usConfigFilenameOffset&gt;456 = 0x1C8 = 0b111001000&lt;/usConfigFilenameOffset&gt;
  &lt;usCRC_BlockOffset&gt;621 = 0x26D = 0b1001101101&lt;/usCRC_BlockOffset&gt;
  &lt;usBIOS_BootupMessageOffset&gt;284 = 0x11C = 0b100011100&lt;/usBIOS_BootupMessageOffset&gt;
  &lt;usInt10Offset&gt;1006 = 0x3EE = 0b1111101110&lt;/usInt10Offset&gt;
  &lt;usPciBusDevInitCode&gt;0&lt;/usPciBusDevInitCode&gt;
  &lt;usIoBaseAddress&gt;0&lt;/usIoBaseAddress&gt;
  &lt;usSubsystemVendorID&gt;4098 = 0x1002 = 0b1000000000010&lt;/usSubsystemVendorID&gt;
  &lt;usSubsystemID&gt;2871 = 0xB37 = 0b101100110111&lt;/usSubsystemID&gt;
  &lt;usPCI_InfoOffset&gt;584 = 0x248 = 0b1001001000&lt;/usPCI_InfoOffset&gt;
  &lt;usMasterCommandTableOffset&gt;38742 = 0x9756 = 0b1001011101010110&lt;/usMasterCommandTableOffset&gt;
  &lt;usMasterDataTableOffset&gt;38908 = 0x97FC = 0b1001011111111100&lt;/usMasterDataTableOffset&gt;
  &lt;ucExtendedFunctionCode&gt;160 = 0xA0 = 0b10100000&lt;/ucExtendedFunctionCode&gt;
  &lt;ucReserved&gt;0&lt;/ucReserved&gt;
  &lt;ulPSPDirTableOffset&gt;1380533072 = 0x52494350 = 0b1010010010010010100001101010000&lt;/ulPSPDirTableOffset&gt;
  &lt;usDeviceID&gt;4098 = 0x1002 = 0b1000000000010&lt;/usDeviceID&gt;
  &lt;usVendorID&gt;26591 = 0x67DF = 0b110011111011111&lt;/usVendorID&gt;
&lt;/ATOM_ROM_HEADER&gt;
&lt;ATOM_DATA_TABLES of="0x97FC-0x9846  len=0x4A=74"&gt;
  &lt;sHeader&gt;
    &lt;usStructureSize&gt;74 = 0x4A = 0b1001010&lt;/usStructureSize&gt;
    &lt;ucTableFormatRevision&gt;1&lt;/ucTableFormatRevision&gt;
    &lt;ucTableContentRevision&gt;1&lt;/ucTableContentRevision&gt;
  &lt;/sHeader&gt;
  &lt;UtilityPipeLine&gt;0&lt;/UtilityPipeLine&gt;
  &lt;MultimediaCapabilityInfo&gt;0&lt;/MultimediaCapabilityInfo&gt;
  &lt;MultimediaConfigInfo&gt;0&lt;/MultimediaConfigInfo&gt;
  &lt;StandardVESA_Timing&gt;38982 = 0x9846 = 0b1001100001000110&lt;/StandardVESA_Timing&gt;
  &lt;FirmwareInfo&gt;39210 = 0x992A = 0b1001100100101010&lt;/FirmwareInfo&gt;
  &lt;PaletteData&gt;39318 = 0x9996 = 0b1001100110010110&lt;/PaletteData&gt;
  &lt;LCD_Info&gt;39370 = 0x99CA = 0b1001100111001010&lt;/LCD_Info&gt;
  &lt;DIGTransmitterInfo&gt;0&lt;/DIGTransmitterInfo&gt;
  &lt;SMU_Info&gt;43600 = 0xAA50 = 0b1010101001010000&lt;/SMU_Info&gt;
  &lt;SupportedDevicesInfo&gt;0&lt;/SupportedDevicesInfo&gt;
  &lt;GPIO_I2C_Info&gt;39448 = 0x9A18 = 0b1001101000011000&lt;/GPIO_I2C_Info&gt;
  &lt;VRAM_UsageByFirmware&gt;39668 = 0x9AF4 = 0b1001101011110100&lt;/VRAM_UsageByFirmware&gt;
  &lt;GPIO_Pin_LUT&gt;39680 = 0x9B00 = 0b1001101100000000&lt;/GPIO_Pin_LUT&gt;
  &lt;VESA_ToInternalModeLUT&gt;39712 = 0x9B20 = 0b1001101100100000&lt;/VESA_ToInternalModeLUT&gt;
  &lt;GFX_Info&gt;39880 = 0x9BC8 = 0b1001101111001000&lt;/GFX_Info&gt;
  &lt;PowerPlayInfo&gt;39904 = 0x9BE0 = 0b1001101111100000&lt;/PowerPlayInfo&gt;
  &lt;GPUVirtualizationInfo&gt;0&lt;/GPUVirtualizationInfo&gt;
  &lt;SaveRestoreInfo&gt;43576 = 0xAA38 = 0b1010101000111000&lt;/SaveRestoreInfo&gt;
  &lt;PPLL_SS_Info&gt;0&lt;/PPLL_SS_Info&gt;
  &lt;OemInfo&gt;0&lt;/OemInfo&gt;
  &lt;XTMDS_Info&gt;0&lt;/XTMDS_Info&gt;
  &lt;MclkSS_Info&gt;0&lt;/MclkSS_Info&gt;
  &lt;Object_Header&gt;40744 = 0x9F28 = 0b1001111100101000&lt;/Object_Header&gt;
  &lt;IndirectIOAccess&gt;41818 = 0xA35A = 0b1010001101011010&lt;/IndirectIOAccess&gt;
  &lt;MC_InitParameter&gt;41094 = 0xA086 = 0b1010000010000110&lt;/MC_InitParameter&gt;
  &lt;ASIC_VDDC_Info&gt;0&lt;/ASIC_VDDC_Info&gt;
  &lt;ASIC_InternalSS_Info&gt;43436 = 0xA9AC = 0b1010100110101100&lt;/ASIC_InternalSS_Info&gt;
  &lt;TV_VideoMode&gt;43476 = 0xA9D4 = 0b1010100111010100&lt;/TV_VideoMode&gt;
  &lt;VRAM_Info&gt;41944 = 0xA3D8 = 0b1010001111011000&lt;/VRAM_Info&gt;
  &lt;MemoryTrainingInfo&gt;0&lt;/MemoryTrainingInfo&gt;
  &lt;IntegratedSystemInfo&gt;0&lt;/IntegratedSystemInfo&gt;
  &lt;ASIC_ProfilingInfo&gt;43066 = 0xA83A = 0b1010100000111010&lt;/ASIC_ProfilingInfo&gt;
  &lt;VoltageObjectInfo&gt;43334 = 0xA946 = 0b1010100101000110&lt;/VoltageObjectInfo&gt;
  &lt;PowerSourceInfo&gt;0&lt;/PowerSourceInfo&gt;
  &lt;ServiceInfo&gt;43656 = 0xAA88 = 0b1010101010001000&lt;/ServiceInfo&gt;
&lt;/ATOM_DATA_TABLES&gt;
&lt;ATOM_POWERPLAY_TABLE of="0x9BE0-0x9C2D  len=0x4D=77"&gt;
  &lt;sHeader&gt;
    &lt;usStructureSize&gt;833 = 0x341 = 0b1101000001&lt;/usStructureSize&gt;
    &lt;ucTableFormatRevision&gt;7 = 0x7 = 0b111&lt;/ucTableFormatRevision&gt;
    &lt;ucTableContentRevision&gt;1&lt;/ucTableContentRevision&gt;
  &lt;/sHeader&gt;
  &lt;ucTableRevision&gt;0&lt;/ucTableRevision&gt;
  &lt;usTableSize&gt;77 = 0x4D = 0b1001101&lt;/usTableSize&gt;
  &lt;ulGoldenPPID&gt;1546 = 0x60A = 0b11000001010&lt;/ulGoldenPPID&gt;
  &lt;ulGoldenRevision&gt;9275 = 0x243B = 0b10010000111011&lt;/ulGoldenRevision&gt;
  &lt;usFormatID&gt;25 = 0x19 = 0b11001&lt;/usFormatID&gt;
  &lt;usVoltageTime&gt;0&lt;/usVoltageTime&gt;
  &lt;ulPlatformCaps&gt;16941056 = 0x1028000 = 0b1000000101000000000000000&lt;/ulPlatformCaps&gt;
  &lt;ulMaxODEngineClock&gt;200000 = 0x30D40 = 0b110000110101000000&lt;/ulMaxODEngineClock&gt;
  &lt;ulMaxODMemoryClock&gt;225000 = 0x36EE8 = 0b110110111011101000&lt;/ulMaxODMemoryClock&gt;
  &lt;usPowerControlLimit&gt;50 = 0x32 = 0b110010&lt;/usPowerControlLimit&gt;
  &lt;usUlvVoltageOffset&gt;50 = 0x32 = 0b110010&lt;/usUlvVoltageOffset&gt;
  &lt;usStateArrayOffset&gt;77 = 0x4D = 0b1001101&lt;/usStateArrayOffset&gt;
  &lt;usFanTableOffset&gt;673 = 0x2A1 = 0b1010100001&lt;/usFanTableOffset&gt;
  &lt;usThermalControllerOffset&gt;664 = 0x298 = 0b1010011000&lt;/usThermalControllerOffset&gt;
  &lt;usReserv&gt;0&lt;/usReserv&gt;
  &lt;usMclkDependencyTableOffset&gt;437 = 0x1B5 = 0b110110101&lt;/usMclkDependencyTableOffset&gt;
  &lt;usSclkDependencyTableOffset&gt;315 = 0x13B = 0b100111011&lt;/usSclkDependencyTableOffset&gt;
  &lt;usVddcLookupTableOffset&gt;119 = 0x77 = 0b1110111&lt;/usVddcLookupTableOffset&gt;
  &lt;usVddgfxLookupTableOffset&gt;249 = 0xF9 = 0b11111001&lt;/usVddgfxLookupTableOffset&gt;
  &lt;usMMDependencyTableOffset&gt;478 = 0x1DE = 0b111011110&lt;/usMMDependencyTableOffset&gt;
  &lt;usVCEStateTableOffset&gt;774 = 0x306 = 0b1100000110&lt;/usVCEStateTableOffset&gt;
  &lt;usPPMTableOffset&gt;0&lt;/usPPMTableOffset&gt;
  &lt;usPowerTuneTableOffset&gt;721 = 0x2D1 = 0b1011010001&lt;/usPowerTuneTableOffset&gt;
  &lt;usHardLimitTableOffset&gt;0&lt;/usHardLimitTableOffset&gt;
  &lt;usPCIETableOffset&gt;800 = 0x320 = 0b1100100000&lt;/usPCIETableOffset&gt;
  &lt;usGPIOTableOffset&gt;826 = 0x33A = 0b1100111010&lt;/usGPIOTableOffset&gt;
&lt;/ATOM_POWERPLAY_TABLE&gt;
&lt;ATOM_Polaris_PowerTune_Table of="0x9EB1-0x9EE6  len=0x35=53"&gt;
  &lt;ucRevId&gt;4 = 0x4 = 0b100&lt;/ucRevId&gt;
  &lt;usTDP&gt;145 = 0x91 = 0b10010001&lt;/usTDP&gt;
  &lt;usConfigurableTDP&gt;0&lt;/usConfigurableTDP&gt;
  &lt;usTDC&gt;132 = 0x84 = 0b10000100&lt;/usTDC&gt;
  &lt;usBatteryPowerLimit&gt;145 = 0x91 = 0b10010001&lt;/usBatteryPowerLimit&gt;
  &lt;usSmallPowerLimit&gt;145 = 0x91 = 0b10010001&lt;/usSmallPowerLimit&gt;
  &lt;usLowCACLeakage&gt;0&lt;/usLowCACLeakage&gt;
  &lt;usHighCACLeakage&gt;0&lt;/usHighCACLeakage&gt;
  &lt;usMaximumPowerDeliveryLimit&gt;145 = 0x91 = 0b10010001&lt;/usMaximumPowerDeliveryLimit&gt;
  &lt;usTjMax&gt;90 = 0x5A = 0b1011010&lt;/usTjMax&gt;
  &lt;usPowerTuneDataSetID&gt;0&lt;/usPowerTuneDataSetID&gt;
  &lt;usEDCLimit&gt;0&lt;/usEDCLimit&gt;
  &lt;usSoftwareShutdownTemp&gt;94 = 0x5E = 0b1011110&lt;/usSoftwareShutdownTemp&gt;
  &lt;usClockStretchAmount&gt;2 = 0x2 = 0b10&lt;/usClockStretchAmount&gt;
  &lt;usTemperatureLimitHotspot&gt;105 = 0x69 = 0b1101001&lt;/usTemperatureLimitHotspot&gt;
  &lt;usTemperatureLimitLiquid1&gt;80 = 0x50 = 0b1010000&lt;/usTemperatureLimitLiquid1&gt;
  &lt;usTemperatureLimitLiquid2&gt;80 = 0x50 = 0b1010000&lt;/usTemperatureLimitLiquid2&gt;
  &lt;usTemperatureLimitVrVddc&gt;115 = 0x73 = 0b1110011&lt;/usTemperatureLimitVrVddc&gt;
  &lt;usTemperatureLimitVrMvdd&gt;115 = 0x73 = 0b1110011&lt;/usTemperatureLimitVrMvdd&gt;
  &lt;usTemperatureLimitPlx&gt;95 = 0x5F = 0b1011111&lt;/usTemperatureLimitPlx&gt;
  &lt;ucLiquid1_I2C_address&gt;0&lt;/ucLiquid1_I2C_address&gt;
  &lt;ucLiquid2_I2C_address&gt;0&lt;/ucLiquid2_I2C_address&gt;
  &lt;ucLiquid_I2C_Line&gt;144 = 0x90 = 0b10010000&lt;/ucLiquid_I2C_Line&gt;
  &lt;ucVr_I2C_address&gt;16 = 0x10 = 0b10000&lt;/ucVr_I2C_address&gt;
  &lt;ucVr_I2C_Line&gt;150 = 0x96 = 0b10010110&lt;/ucVr_I2C_Line&gt;
  &lt;ucPlx_I2C_address&gt;0&lt;/ucPlx_I2C_address&gt;
  &lt;ucPlx_I2C_Line&gt;144 = 0x90 = 0b10010000&lt;/ucPlx_I2C_Line&gt;
  &lt;usBoostPowerLimit&gt;0&lt;/usBoostPowerLimit&gt;
  &lt;ucCKS_LDO_REFSEL&gt;6 = 0x6 = 0b110&lt;/ucCKS_LDO_REFSEL&gt;
  &lt;ucHotSpotOnly&gt;0&lt;/ucHotSpotOnly&gt;
  &lt;ucReserve&gt;0&lt;/ucReserve&gt;
  &lt;usReserve&gt;0&lt;/usReserve&gt;
&lt;/ATOM_Polaris_PowerTune_Table&gt;
&lt;ATOM_FAN_TABLE of="0x9E81-0x9EAE  len=0x2D=45"&gt;
  &lt;ucRevId&gt;9 = 0x9 = 0b1001&lt;/ucRevId&gt;
  &lt;ucTHyst&gt;3 = 0x3 = 0b11&lt;/ucTHyst&gt;
  &lt;usTMin&gt;4000 = 0xFA0 = 0b111110100000&lt;/usTMin&gt;
  &lt;usTMed&gt;6500 = 0x1964 = 0b1100101100100&lt;/usTMed&gt;
  &lt;usTHigh&gt;8500 = 0x2134 = 0b10000100110100&lt;/usTHigh&gt;
  &lt;usPWMMin&gt;2000 = 0x7D0 = 0b11111010000&lt;/usPWMMin&gt;
  &lt;usPWMMed&gt;4000 = 0xFA0 = 0b111110100000&lt;/usPWMMed&gt;
  &lt;usPWMHigh&gt;6000 = 0x1770 = 0b1011101110000&lt;/usPWMHigh&gt;
  &lt;usTMax&gt;10900 = 0x2A94 = 0b10101010010100&lt;/usTMax&gt;
  &lt;ucFanControlMode&gt;1&lt;/ucFanControlMode&gt;
  &lt;usFanPWMMax&gt;100 = 0x64 = 0b1100100&lt;/usFanPWMMax&gt;
  &lt;usFanOutputSensitivity&gt;4836 = 0x12E4 = 0b1001011100100&lt;/usFanOutputSensitivity&gt;
  &lt;usFanRPMMax&gt;2200 = 0x898 = 0b100010011000&lt;/usFanRPMMax&gt;
  &lt;ulMinFanSCLKAcousticLimit&gt;91000 = 0x16378 = 0b10110001101111000&lt;/ulMinFanSCLKAcousticLimit&gt;
  &lt;ucTargetTemperature&gt;80 = 0x50 = 0b1010000&lt;/ucTargetTemperature&gt;
  &lt;ucMinimumPWMLimit&gt;20 = 0x14 = 0b10100&lt;/ucMinimumPWMLimit&gt;
  &lt;usFanGainEdge&gt;100 = 0x64 = 0b1100100&lt;/usFanGainEdge&gt;
  &lt;usFanGainHotspot&gt;100 = 0x64 = 0b1100100&lt;/usFanGainHotspot&gt;
  &lt;usFanGainLiquid&gt;100 = 0x64 = 0b1100100&lt;/usFanGainLiquid&gt;
  &lt;usFanGainVrVddc&gt;100 = 0x64 = 0b1100100&lt;/usFanGainVrVddc&gt;
  &lt;usFanGainVrMvdd&gt;100 = 0x64 = 0b1100100&lt;/usFanGainVrMvdd&gt;
  &lt;usFanGainPlx&gt;100 = 0x64 = 0b1100100&lt;/usFanGainPlx&gt;
  &lt;usFanGainHbm&gt;100 = 0x64 = 0b1100100&lt;/usFanGainHbm&gt;
  &lt;usReserved&gt;10752 = 0x2A00 = 0b10101000000000&lt;/usReserved&gt;
&lt;/ATOM_FAN_TABLE&gt;
&lt;ATOM_MCLK_TABLE of="0x9D95-0x9D97  len=0x2=2"&gt;
  &lt;ucRevId&gt;0&lt;/ucRevId&gt;
  &lt;ucNumEntries&gt;3 = 0x3 = 0b11&lt;/ucNumEntries&gt;
&lt;/ATOM_MCLK_TABLE&gt;
&lt;ATOM_MCLK_ENTRY of="0x9D97-0x9DA4  len=0xD=13"&gt;
  &lt;ucVddcInd&gt;0&lt;/ucVddcInd&gt;
  &lt;usVddci&gt;800 = 0x320 = 0b1100100000&lt;/usVddci&gt;
  &lt;usVddgfxOffset&gt;0&lt;/usVddgfxOffset&gt;
  &lt;usMvdd&gt;1000 = 0x3E8 = 0b1111101000&lt;/usMvdd&gt;
  &lt;ulMclk&gt;30000 = 0x7530 = 0b111010100110000&lt;/ulMclk&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_MCLK_ENTRY&gt;
&lt;ATOM_MCLK_ENTRY of="0x9DA4-0x9DB1  len=0xD=13"&gt;
  &lt;ucVddcInd&gt;9 = 0x9 = 0b1001&lt;/ucVddcInd&gt;
  &lt;usVddci&gt;850 = 0x352 = 0b1101010010&lt;/usVddci&gt;
  &lt;usVddgfxOffset&gt;0&lt;/usVddgfxOffset&gt;
  &lt;usMvdd&gt;1000 = 0x3E8 = 0b1111101000&lt;/usMvdd&gt;
  &lt;ulMclk&gt;100000 = 0x186A0 = 0b11000011010100000&lt;/ulMclk&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_MCLK_ENTRY&gt;
&lt;ATOM_MCLK_ENTRY of="0x9DB1-0x9DBE  len=0xD=13"&gt;
  &lt;ucVddcInd&gt;12 = 0xC = 0b1100&lt;/ucVddcInd&gt;
  &lt;usVddci&gt;950 = 0x3B6 = 0b1110110110&lt;/usVddci&gt;
  &lt;usVddgfxOffset&gt;0&lt;/usVddgfxOffset&gt;
  &lt;usMvdd&gt;1000 = 0x3E8 = 0b1111101000&lt;/usMvdd&gt;
  &lt;ulMclk&gt;200000 = 0x30D40 = 0b110000110101000000&lt;/ulMclk&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_MCLK_ENTRY&gt;
&lt;ATOM_SCLK_TABLE of="0x9D1B-0x9D1D  len=0x2=2"&gt;
  &lt;ucRevId&gt;1&lt;/ucRevId&gt;
  &lt;ucNumEntries&gt;8 = 0x8 = 0b1000&lt;/ucNumEntries&gt;
&lt;/ATOM_SCLK_TABLE&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D1D-0x9D2C  len=0xF=15"&gt;
  &lt;ucVddInd&gt;0&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;0&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;30000 = 0x7530 = 0b111010100110000&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;128 = 0x80 = 0b10000000&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D2C-0x9D3B  len=0xF=15"&gt;
  &lt;ucVddInd&gt;1&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;65510 = 0xFFE6 = 0b1111111111100110&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;60000 = 0xEA60 = 0b1110101001100000&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;0&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D3B-0x9D4A  len=0xF=15"&gt;
  &lt;ucVddInd&gt;2 = 0x2 = 0b10&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;65510 = 0xFFE6 = 0b1111111111100110&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;90000 = 0x15F90 = 0b10101111110010000&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;0&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D4A-0x9D59  len=0xF=15"&gt;
  &lt;ucVddInd&gt;3 = 0x3 = 0b11&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;65510 = 0xFFE6 = 0b1111111111100110&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;114500 = 0x1BF44 = 0b11011111101000100&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;0&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D59-0x9D68  len=0xF=15"&gt;
  &lt;ucVddInd&gt;4 = 0x4 = 0b100&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;65510 = 0xFFE6 = 0b1111111111100110&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;121500 = 0x1DA9C = 0b11101101010011100&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;0&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D68-0x9D77  len=0xF=15"&gt;
  &lt;ucVddInd&gt;5 = 0x5 = 0b101&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;65510 = 0xFFE6 = 0b1111111111100110&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;125700 = 0x1EB04 = 0b11110101100000100&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;0&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D77-0x9D86  len=0xF=15"&gt;
  &lt;ucVddInd&gt;6 = 0x6 = 0b110&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;65510 = 0xFFE6 = 0b1111111111100110&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;130000 = 0x1FBD0 = 0b11111101111010000&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;0&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_SCLK_ENTRY of="0x9D86-0x9D95  len=0xF=15"&gt;
  &lt;ucVddInd&gt;7 = 0x7 = 0b111&lt;/ucVddInd&gt;
  &lt;usVddcOffset&gt;0&lt;/usVddcOffset&gt;
  &lt;ulSclk&gt;134000 = 0x20B70 = 0b100000101101110000&lt;/ulSclk&gt;
  &lt;usEdcCurrent&gt;0&lt;/usEdcCurrent&gt;
  &lt;ucReliabilityTemperature&gt;0&lt;/ucReliabilityTemperature&gt;
  &lt;ucCKSVOffsetandDisable&gt;0&lt;/ucCKSVOffsetandDisable&gt;
  &lt;ulSclkOffset&gt;0&lt;/ulSclkOffset&gt;
&lt;/ATOM_SCLK_ENTRY&gt;
&lt;ATOM_VOLTAGE_TABLE of="0x9C57-0x9C59  len=0x2=2"&gt;
  &lt;ucRevId&gt;0&lt;/ucRevId&gt;
  &lt;ucNumEntries&gt;16 = 0x10 = 0b10000&lt;/ucNumEntries&gt;
&lt;/ATOM_VOLTAGE_TABLE&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C59-0x9C61  len=0x8=8"&gt;
  &lt;usVdd&gt;750 = 0x2EE = 0b1011101110&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C61-0x9C69  len=0x8=8"&gt;
  &lt;usVdd&gt;65282 = 0xFF02 = 0b1111111100000010&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C69-0x9C71  len=0x8=8"&gt;
  &lt;usVdd&gt;65283 = 0xFF03 = 0b1111111100000011&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C71-0x9C79  len=0x8=8"&gt;
  &lt;usVdd&gt;65284 = 0xFF04 = 0b1111111100000100&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C79-0x9C81  len=0x8=8"&gt;
  &lt;usVdd&gt;65285 = 0xFF05 = 0b1111111100000101&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C81-0x9C89  len=0x8=8"&gt;
  &lt;usVdd&gt;65286 = 0xFF06 = 0b1111111100000110&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C89-0x9C91  len=0x8=8"&gt;
  &lt;usVdd&gt;65287 = 0xFF07 = 0b1111111100000111&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C91-0x9C99  len=0x8=8"&gt;
  &lt;usVdd&gt;65288 = 0xFF08 = 0b1111111100001000&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9C99-0x9CA1  len=0x8=8"&gt;
  &lt;usVdd&gt;800 = 0x320 = 0b1100100000&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9CA1-0x9CA9  len=0x8=8"&gt;
  &lt;usVdd&gt;850 = 0x352 = 0b1101010010&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9CA9-0x9CB1  len=0x8=8"&gt;
  &lt;usVdd&gt;900 = 0x384 = 0b1110000100&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9CB1-0x9CB9  len=0x8=8"&gt;
  &lt;usVdd&gt;950 = 0x3B6 = 0b1110110110&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9CB9-0x9CC1  len=0x8=8"&gt;
  &lt;usVdd&gt;1000 = 0x3E8 = 0b1111101000&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9CC1-0x9CC9  len=0x8=8"&gt;
  &lt;usVdd&gt;1050 = 0x41A = 0b10000011010&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9CC9-0x9CD1  len=0x8=8"&gt;
  &lt;usVdd&gt;1100 = 0x44C = 0b10001001100&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VOLTAGE_ENTRY of="0x9CD1-0x9CD9  len=0x8=8"&gt;
  &lt;usVdd&gt;1150 = 0x47E = 0b10001111110&lt;/usVdd&gt;
  &lt;usCACLow&gt;0&lt;/usCACLow&gt;
  &lt;usCACMid&gt;0&lt;/usCACMid&gt;
  &lt;usCACHigh&gt;0&lt;/usCACHigh&gt;
&lt;/ATOM_VOLTAGE_ENTRY&gt;
&lt;ATOM_VRAM_INFO of="0xA3D8-0xA3EC  len=0x14=20"&gt;
  &lt;sHeader&gt;
    &lt;usStructureSize&gt;1121 = 0x461 = 0b10001100001&lt;/usStructureSize&gt;
    &lt;ucTableFormatRevision&gt;2 = 0x2 = 0b10&lt;/ucTableFormatRevision&gt;
    &lt;ucTableContentRevision&gt;2 = 0x2 = 0b10&lt;/ucTableContentRevision&gt;
  &lt;/sHeader&gt;
  &lt;usMemAdjustTblOffset&gt;75 = 0x4B = 0b1001011&lt;/usMemAdjustTblOffset&gt;
  &lt;usMemClkPatchTblOffset&gt;90 = 0x5A = 0b1011010&lt;/usMemClkPatchTblOffset&gt;
  &lt;usMcAdjustPerTileTblOffset&gt;764 = 0x2FC = 0b1011111100&lt;/usMcAdjustPerTileTblOffset&gt;
  &lt;usMcPhyInitTableOffset&gt;946 = 0x3B2 = 0b1110110010&lt;/usMcPhyInitTableOffset&gt;
  &lt;usDramDataRemapTblOffset&gt;810 = 0x32A = 0b1100101010&lt;/usDramDataRemapTblOffset&gt;
  &lt;usReserved1&gt;0&lt;/usReserved1&gt;
  &lt;ucNumOfVRAMModule&gt;1&lt;/ucNumOfVRAMModule&gt;
  &lt;ucMemoryClkPatchTblVer&gt;1&lt;/ucMemoryClkPatchTblVer&gt;
  &lt;ucVramModuleVer&gt;8 = 0x8 = 0b1000&lt;/ucVramModuleVer&gt;
  &lt;ucMcPhyTileNum&gt;4 = 0x4 = 0b100&lt;/ucMcPhyTileNum&gt;
&lt;/ATOM_VRAM_INFO&gt;
&lt;ATOM_VRAM_ENTRY of="0xA3EC-0xA42C  len=0x40=64"&gt;
  &lt;ulChannelMapCfg&gt;1985220658 = 0x76541032 = 0b1110110010101000001000000110010&lt;/ulChannelMapCfg&gt;
  &lt;usModuleSize&gt;55 = 0x37 = 0b110111&lt;/usModuleSize&gt;
  &lt;usMcRamCfg&gt;24738 = 0x60A2 = 0b110000010100010&lt;/usMcRamCfg&gt;
  &lt;usEnableChannels&gt;255 = 0xFF = 0b11111111&lt;/usEnableChannels&gt;
  &lt;ucExtMemoryID&gt;0&lt;/ucExtMemoryID&gt;
  &lt;ucMemoryType&gt;80 = 0x50 = 0b1010000&lt;/ucMemoryType&gt;
  &lt;ucChannelNum&gt;3 = 0x3 = 0b11&lt;/ucChannelNum&gt;
  &lt;ucChannelWidth&gt;5 = 0x5 = 0b101&lt;/ucChannelWidth&gt;
  &lt;ucDensity&gt;99 = 0x63 = 0b1100011&lt;/ucDensity&gt;
  &lt;ucBankCol&gt;10 = 0xA = 0b1010&lt;/ucBankCol&gt;
  &lt;ucMisc&gt;4 = 0x4 = 0b100&lt;/ucMisc&gt;
  &lt;ucVREFI&gt;0&lt;/ucVREFI&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
  &lt;usMemorySize&gt;8192 = 0x2000 = 0b10000000000000&lt;/usMemorySize&gt;
  &lt;ucMcTunningSetId&gt;0&lt;/ucMcTunningSetId&gt;
  &lt;ucRowNum&gt;11 = 0xB = 0b1011&lt;/ucRowNum&gt;
  &lt;usEMRS2Value&gt;16384 = 0x4000 = 0b100000000000000&lt;/usEMRS2Value&gt;
  &lt;usEMRS3Value&gt;24832 = 0x6100 = 0b110000100000000&lt;/usEMRS3Value&gt;
  &lt;ucMemoryVenderID&gt;33 = 0x21 = 0b100001&lt;/ucMemoryVenderID&gt;
  &lt;ucRefreshRateFactor&gt;2 = 0x2 = 0b10&lt;/ucRefreshRateFactor&gt;
  &lt;ucFIFODepth&gt;2 = 0x2 = 0b10&lt;/ucFIFODepth&gt;
  &lt;ucCDR_Bandwidth&gt;0&lt;/ucCDR_Bandwidth&gt;
  &lt;ulChannelMapCfg1&gt;0&lt;/ulChannelMapCfg1&gt;
  &lt;ulBankMapCfg&gt;484675 = 0x76543 = 0b1110110010101000011&lt;/ulBankMapCfg&gt;
  &lt;ulReserved&gt;0&lt;/ulReserved&gt;
  &lt;FullName&gt;K4G80325FB&lt;/FullName&gt;
&lt;/ATOM_VRAM_ENTRY&gt;
End of mem

&lt;ATOM_VRAM_TIMING_ENTRY of="0xA460-0xA494  len=0x34=52"&gt;
  &lt;ulClkRange&gt;25000 = 0x61A8 = 0b110000110101000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C00628C110B10570A080EC3B00100204100220114209A8800A000000000040308091B0D0F0E&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA494-0xA4C8  len=0x34=52"&gt;
  &lt;ulClkRange&gt;40000 = 0x9C40 = 0b1001110001000000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C006394121120570A091144B102002042002A021420AA8800A00000000006040C0E2B10120F&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA4C8-0xA4FC  len=0x34=52"&gt;
  &lt;ulClkRange&gt;60000 = 0xEA60 = 0b1110101001100000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C00A520241A40570B0B97051204002264003A051420CA8800A0000000000906121541151810&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA4FC-0xA530  len=0x34=52"&gt;
  &lt;ulClkRange&gt;90000 = 0x15F90 = 0b10101111110010000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C00E7B4362780570B0F9F072306002485005A091420DA8800A0000000000E081A20621D2012&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA530-0xA564  len=0x34=52"&gt;
  &lt;ulClkRange&gt;100000 = 0x186A0 = 0b11000011010100000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C000839372B90570B102148D30600448600620A14206A8900A0000000000F091D236D1F2213&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA564-0xA598  len=0x34=52"&gt;
  &lt;ulClkRange&gt;112500 = 0x1B774 = 0b11011011101110100&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C0029414831A0570C1125C9B3070046A6006A0C14206A8900A000000000110A21287B222614&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA598-0xA5CC  len=0x34=52"&gt;
  &lt;ulClkRange&gt;125000 = 0x1E848 = 0b11110100001001000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C004A494937B0570C12294A94080046A700720E14207A8900A000000000130B252D89252A14&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA5CC-0xA600  len=0x34=52"&gt;
  &lt;ulClkRange&gt;137500 = 0x2191C = 0b100001100100011100&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;333000000000000022CC1C008C515A3DC0570D132DCB74090048C7007A0014207A8900A002000000150D293197282E15&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA600-0xA634  len=0x34=52"&gt;
  &lt;ulClkRange&gt;150000 = 0x249F0 = 0b100100100111110000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;555000000000000022CC1C00AD595B41C0570E14B00B450A0068C70003011420FA8900A003000000170E2B34A42A3116&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA634-0xA668  len=0x34=52"&gt;
  &lt;ulClkRange&gt;162500 = 0x27AC4 = 0b100111101011000100&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;555000000000000022CC1C00CE616C47D0570F15B48C250B006AE7000B031420FA8900A003000000190F2F39B22D3517&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA668-0xA69C  len=0x34=52"&gt;
  &lt;ulClkRange&gt;175000 = 0x2AB98 = 0b101010101110011000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;777000000000000022CC1C00106A6D4DD0571016B90D060C006AE70014051420FA8900A0030000001B11333DC0303A17&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA69C-0xA6D0  len=0x34=52"&gt;
  &lt;ulClkRange&gt;200000 = 0x30D40 = 0b110000110101000000&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;777000000000000022CC1C0031F67E57F05711183FCFB60D006C070124081420FA8900A0030000001E123A46DB354019&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_VRAM_TIMING_ENTRY of="0xA6D0-0xA704  len=0x34=52"&gt;
  &lt;ulClkRange&gt;0&lt;/ulClkRange&gt;
  &lt;LatencyString&gt;060008000E0044FFFF00FFFFFF001F000000FFFFFF011F000000FFFFFF021F000000FFFFFF031F00000000000000E1B4&lt;/LatencyString&gt;
&lt;/ATOM_VRAM_TIMING_ENTRY&gt;
&lt;ATOM_OBJECT_HEADER_V3 of="0x9F28-0x9F3A  len=0x12=18"&gt;
  &lt;sHeader&gt;
    &lt;usStructureSize&gt;350 = 0x15E = 0b101011110&lt;/usStructureSize&gt;
    &lt;ucTableFormatRevision&gt;1&lt;/ucTableFormatRevision&gt;
    &lt;ucTableContentRevision&gt;3 = 0x3 = 0b11&lt;/ucTableContentRevision&gt;
  &lt;/sHeader&gt;
  &lt;usDeviceSupport&gt;3720 = 0xE88 = 0b111010001000&lt;/usDeviceSupport&gt;
  &lt;usConnectorObjectTableOffset&gt;72 = 0x48 = 0b1001000&lt;/usConnectorObjectTableOffset&gt;
  &lt;usRouterObjectTableOffset&gt;0&lt;/usRouterObjectTableOffset&gt;
  &lt;usEncoderObjectTableOffset&gt;251 = 0xFB = 0b11111011&lt;/usEncoderObjectTableOffset&gt;
  &lt;usProtectionObjectTableOffset&gt;0&lt;/usProtectionObjectTableOffset&gt;
  &lt;usDisplayPathTableOffset&gt;18 = 0x12 = 0b10010&lt;/usDisplayPathTableOffset&gt;
  &lt;usMiscObjectTableOffset&gt;0&lt;/usMiscObjectTableOffset&gt;
&lt;/ATOM_OBJECT_HEADER_V3&gt;
&lt;ATOM_DISPLAY_OBJECT_PATH_TABLE of="0x9F3A-0x9F3E  len=0x4=4"&gt;
  &lt;ucNumOfDispPath&gt;5 = 0x5 = 0b101&lt;/ucNumOfDispPath&gt;
  &lt;ucVersion&gt;1&lt;/ucVersion&gt;
  &lt;ucPadding2&gt;0&lt;/ucPadding2&gt;
&lt;/ATOM_DISPLAY_OBJECT_PATH_TABLE&gt;
&lt;ATOM_DISPLAY_OBJECT_PATH of="0x9F3E-0x9F48  len=0xA=10"&gt;
  &lt;usDeviceTag&gt;8 = 0x8 = 0b1000&lt;/usDeviceTag&gt;
  &lt;usSize&gt;10 = 0xA = 0b1010&lt;/usSize&gt;
  &lt;usConnObjectId&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DISPLAYPORT = 0x13&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usConnObjectId&gt;
  &lt;usGPUObjectId&gt;
    &lt;KindInNamespace&gt;0&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_GPU&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGPUObjectId&gt;
  &lt;usGraphicObjIdsFirst&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY2 = 0x21&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGraphicObjIdsFirst&gt;
&lt;/ATOM_DISPLAY_OBJECT_PATH&gt;
&lt;ATOM_DISPLAY_OBJECT_PATH of="0x9F48-0x9F52  len=0xA=10"&gt;
  &lt;usDeviceTag&gt;128 = 0x80 = 0b10000000&lt;/usDeviceTag&gt;
  &lt;usSize&gt;10 = 0xA = 0b1010&lt;/usSize&gt;
  &lt;usConnObjectId&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DISPLAYPORT = 0x13&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;2 = 0x2 = 0b10&lt;/Index&gt;
  &lt;/usConnObjectId&gt;
  &lt;usGPUObjectId&gt;
    &lt;KindInNamespace&gt;0&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_GPU&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGPUObjectId&gt;
  &lt;usGraphicObjIdsFirst&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY2 = 0x21&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;2 = 0x2 = 0b10&lt;/Index&gt;
  &lt;/usGraphicObjIdsFirst&gt;
&lt;/ATOM_DISPLAY_OBJECT_PATH&gt;
&lt;ATOM_DISPLAY_OBJECT_PATH of="0x9F52-0x9F5C  len=0xA=10"&gt;
  &lt;usDeviceTag&gt;512 = 0x200 = 0b1000000000&lt;/usDeviceTag&gt;
  &lt;usSize&gt;10 = 0xA = 0b1010&lt;/usSize&gt;
  &lt;usConnObjectId&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DISPLAYPORT = 0x13&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;3 = 0x3 = 0b11&lt;/Index&gt;
  &lt;/usConnObjectId&gt;
  &lt;usGPUObjectId&gt;
    &lt;KindInNamespace&gt;0&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_GPU&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGPUObjectId&gt;
  &lt;usGraphicObjIdsFirst&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY1 = 0x20&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGraphicObjIdsFirst&gt;
&lt;/ATOM_DISPLAY_OBJECT_PATH&gt;
&lt;ATOM_DISPLAY_OBJECT_PATH of="0x9F5C-0x9F66  len=0xA=10"&gt;
  &lt;usDeviceTag&gt;1024 = 0x400 = 0b10000000000&lt;/usDeviceTag&gt;
  &lt;usSize&gt;10 = 0xA = 0b1010&lt;/usSize&gt;
  &lt;usConnObjectId&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_HDMI_TYPE_A = 0xC&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usConnObjectId&gt;
  &lt;usGPUObjectId&gt;
    &lt;KindInNamespace&gt;0&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_GPU&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGPUObjectId&gt;
  &lt;usGraphicObjIdsFirst&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY1 = 0x20&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;2 = 0x2 = 0b10&lt;/Index&gt;
  &lt;/usGraphicObjIdsFirst&gt;
&lt;/ATOM_DISPLAY_OBJECT_PATH&gt;
&lt;ATOM_DISPLAY_OBJECT_PATH of="0x9F66-0x9F70  len=0xA=10"&gt;
  &lt;usDeviceTag&gt;2048 = 0x800 = 0b100000000000&lt;/usDeviceTag&gt;
  &lt;usSize&gt;10 = 0xA = 0b1010&lt;/usSize&gt;
  &lt;usConnObjectId&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DUAL_LINK_DVI_D = 0x4&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usConnObjectId&gt;
  &lt;usGPUObjectId&gt;
    &lt;KindInNamespace&gt;0&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_GPU&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGPUObjectId&gt;
  &lt;usGraphicObjIdsFirst&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY = 0x1E&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usGraphicObjIdsFirst&gt;
&lt;/ATOM_DISPLAY_OBJECT_PATH&gt;
Encoders:
&lt;ATOM_OBJECT_TABLE of="0xA023-0xA027  len=0x4=4"&gt;
  &lt;ucNumberOfObjects&gt;5 = 0x5 = 0b101&lt;/ucNumberOfObjects&gt;
  &lt;ucPadding0&gt;0&lt;/ucPadding0&gt;
  &lt;ucPadding1&gt;0&lt;/ucPadding1&gt;
  &lt;ucPadding2&gt;0&lt;/ucPadding2&gt;
&lt;/ATOM_OBJECT_TABLE&gt;
&lt;ATOM_OBJECT of="0xA027-0xA02F  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY2 = 0x21&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;295 = 0x127 = 0b100100111&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;301 = 0x12D = 0b100101101&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0xA055-0xA057  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_ENCODER_CAP_RECORD_TYPE = 0x14&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa057:0F00
&lt;ATOM_OBJECT of="0xA02F-0xA037  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY2 = 0x21&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;2 = 0x2 = 0b10&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;306 = 0x132 = 0b100110010&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;312 = 0x138 = 0b100111000&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0xA060-0xA062  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_ENCODER_CAP_RECORD_TYPE = 0x14&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa062:0F00
&lt;ATOM_OBJECT of="0xA037-0xA03F  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY1 = 0x20&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;317 = 0x13D = 0b100111101&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;323 = 0x143 = 0b101000011&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0xA06B-0xA06D  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_ENCODER_CAP_RECORD_TYPE = 0x14&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa06d:0F00
&lt;ATOM_OBJECT of="0xA03F-0xA047  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY1 = 0x20&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;2 = 0x2 = 0b10&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;328 = 0x148 = 0b101001000&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;334 = 0x14E = 0b101001110&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0xA076-0xA078  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_ENCODER_CAP_RECORD_TYPE = 0x14&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa078:0F00
&lt;ATOM_OBJECT of="0xA047-0xA04F  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;ENCODER_OBJECT_ID_INTERNAL_UNIPHY = 0x1E&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_ENCODER&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;339 = 0x153 = 0b101010011&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;345 = 0x159 = 0b101011001&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0xA081-0xA083  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_ENCODER_CAP_RECORD_TYPE = 0x14&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa083:0F00
Connectors:
&lt;ATOM_OBJECT_TABLE of="0x9F70-0x9F74  len=0x4=4"&gt;
  &lt;ucNumberOfObjects&gt;5 = 0x5 = 0b101&lt;/ucNumberOfObjects&gt;
  &lt;ucPadding0&gt;0&lt;/ucPadding0&gt;
  &lt;ucPadding1&gt;0&lt;/ucPadding1&gt;
  &lt;ucPadding2&gt;0&lt;/ucPadding2&gt;
&lt;/ATOM_OBJECT_TABLE&gt;
&lt;ATOM_OBJECT of="0x9F74-0x9F7C  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DISPLAYPORT = 0x13&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;116 = 0x74 = 0b1110100&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;122 = 0x7A = 0b1111010&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FA2-0x9FA4  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;12 = 0xC = 0b1100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_CONNECTOR_DEVICE_TAG_RECORD_TYPE = 0x4&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fa4:01001002000008000000
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FAE-0x9FB0  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_I2C_RECORD_TYPE = 0x1&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fb0:9000
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FB2-0x9FB4  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_HPD_INT_RECORD_TYPE = 0x2&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fb4:0600
&lt;ATOM_OBJECT of="0x9F7C-0x9F84  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DISPLAYPORT = 0x13&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;2 = 0x2 = 0b10&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;143 = 0x8F = 0b10001111&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;149 = 0x95 = 0b10010101&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FBD-0x9FBF  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;12 = 0xC = 0b1100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_CONNECTOR_DEVICE_TAG_RECORD_TYPE = 0x4&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fbf:01002002000080000000
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FC9-0x9FCB  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_I2C_RECORD_TYPE = 0x1&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fcb:9200
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FCD-0x9FCF  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_HPD_INT_RECORD_TYPE = 0x2&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fcf:0400
&lt;ATOM_OBJECT of="0x9F84-0x9F8C  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DISPLAYPORT = 0x13&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;3 = 0x3 = 0b11&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;170 = 0xAA = 0b10101010&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;176 = 0xB0 = 0b10110000&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FD8-0x9FDA  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;12 = 0xC = 0b1100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_CONNECTOR_DEVICE_TAG_RECORD_TYPE = 0x4&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fda:01003002000000020000
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FE4-0x9FE6  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_I2C_RECORD_TYPE = 0x1&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fe6:9100
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FE8-0x9FEA  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_HPD_INT_RECORD_TYPE = 0x2&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9fea:0100
&lt;ATOM_OBJECT of="0x9F8C-0x9F94  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_HDMI_TYPE_A = 0xC&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;197 = 0xC5 = 0b11000101&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;203 = 0xCB = 0b11001011&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FF3-0x9FF5  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;12 = 0xC = 0b1100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_CONNECTOR_DEVICE_TAG_RECORD_TYPE = 0x4&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0x9ff5:01004002000000040000
&lt;ATOM_COMMON_RECORD_HEADER of="0x9FFF-0xA001  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_I2C_RECORD_TYPE = 0x1&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa001:9300
&lt;ATOM_COMMON_RECORD_HEADER of="0xA003-0xA005  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_HPD_INT_RECORD_TYPE = 0x2&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa005:0500
&lt;ATOM_OBJECT of="0x9F94-0x9F9C  len=0x8=8"&gt;
  &lt;usObjectID&gt;
    &lt;KindInNamespace&gt;CONNECTOR_OBJECT_ID_DUAL_LINK_DVI_D = 0x4&lt;/KindInNamespace&gt;
    &lt;Namespace&gt;GRAPH_OBJECT_TYPE_CONNECTOR&lt;/Namespace&gt;
    &lt;Index&gt;1&lt;/Index&gt;
  &lt;/usObjectID&gt;
  &lt;usSrcDstTableOffset&gt;224 = 0xE0 = 0b11100000&lt;/usSrcDstTableOffset&gt;
  &lt;usRecordOffset&gt;230 = 0xE6 = 0b11100110&lt;/usRecordOffset&gt;
  &lt;usReserved&gt;0&lt;/usReserved&gt;
&lt;/ATOM_OBJECT&gt;
&lt;ATOM_COMMON_RECORD_HEADER of="0xA00E-0xA010  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;12 = 0xC = 0b1100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_CONNECTOR_DEVICE_TAG_RECORD_TYPE = 0x4&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa010:01005002000000080000
&lt;ATOM_COMMON_RECORD_HEADER of="0xA01A-0xA01C  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_I2C_RECORD_TYPE = 0x1&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa01c:9500
&lt;ATOM_COMMON_RECORD_HEADER of="0xA01E-0xA020  len=0x2=2"&gt;
  &lt;ucRecordSize&gt;4 = 0x4 = 0b100&lt;/ucRecordSize&gt;
  &lt;RecordType&gt;ATOM_HPD_INT_RECORD_TYPE = 0x2&lt;/RecordType&gt;
&lt;/ATOM_COMMON_RECORD_HEADER&gt;
Extra at 0xa020:0300
Routers:
Table not present:ATOM_OBJECT_TABLE
&lt;ATOM_VOLTAGE_OBJECT_INFO_V3_1 of="0xA946-0xA94A  len=0x4=4"&gt;
  &lt;sHeader&gt;
    &lt;usStructureSize&gt;102 = 0x66 = 0b1100110&lt;/usStructureSize&gt;
    &lt;ucTableFormatRevision&gt;3 = 0x3 = 0b11&lt;/ucTableFormatRevision&gt;
    &lt;ucTableContentRevision&gt;1&lt;/ucTableContentRevision&gt;
  &lt;/sHeader&gt;
&lt;/ATOM_VOLTAGE_OBJECT_INFO_V3_1&gt;
&lt;atom_voltage_object_header_v4 of="0xA94A-0xA956  len=0xC=12"&gt;
  &lt;ucVoltageType&gt;VOLTAGE_TYPE_VDDC_0x1&lt;/ucVoltageType&gt;
  &lt;ucVoltageMode&gt;VOLTAGE_OBJ_VR_I2C_INIT_SEQ_0x3&lt;/ucVoltageMode&gt;
  &lt;usSize&gt;50 = 0x32 = 0b110010&lt;/usSize&gt;
  &lt;AsI2c&gt;
    &lt;regulator_id&gt;8 = 0x8 = 0b1000&lt;/regulator_id&gt;
    &lt;i2c_id&gt;
      &lt;gpio_id&gt;150 = 0x96 = 0b10010110&lt;/gpio_id&gt;
      &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
      &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
      &lt;bfI2C_LineMux&gt;6 = 0x6 = 0b110&lt;/bfI2C_LineMux&gt;
      &lt;Description&gt;150 = 0x96 = 0b10010110&lt;/Description&gt;
    &lt;/i2c_id&gt;
    &lt;i2c_slave_addr&gt;
      &lt;shifted_i2c_slave_addr&gt;16 = 0x10 = 0b10000&lt;/shifted_i2c_slave_addr&gt;
    &lt;/i2c_slave_addr&gt;
    &lt;i2c_control_offset&gt;0&lt;/i2c_control_offset&gt;
    &lt;i2c_flag&gt;0&lt;/i2c_flag&gt;
    &lt;i2c_speed&gt;0&lt;/i2c_speed&gt;
    &lt;reserved_0xA&gt;0&lt;/reserved_0xA&gt;
    &lt;reserved_0xB&gt;0&lt;/reserved_0xB&gt;
  &lt;/AsI2c&gt;
&lt;/atom_voltage_object_header_v4&gt;
&lt;atom_i2c_data_entry of="0xA956-0xA95A  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;41 = 0x29 = 0b101001&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;36 = 0x24 = 0b100100&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA95A-0xA95E  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;43 = 0x2B = 0b101011&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;44 = 0x2C = 0b101100&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA95E-0xA962  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;51 = 0x33 = 0b110011&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;114 = 0x72 = 0b1110010&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA962-0xA966  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;36 = 0x24 = 0b100100&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;28 = 0x1C = 0b11100&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA966-0xA96A  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;20 = 0x14 = 0b10100&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;34 = 0x22 = 0b100010&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA96A-0xA96E  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;57 = 0x39 = 0b111001&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;190 = 0xBE = 0b10111110&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA96E-0xA972  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;97 = 0x61 = 0b1100001&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;3 = 0x3 = 0b11&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA972-0xA976  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;98 = 0x62 = 0b1100010&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;126 = 0x7E = 0b1111110&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;atom_i2c_data_entry of="0xA976-0xA97A  len=0x4=4"&gt;
  &lt;i2c_reg_index&gt;141 = 0x8D = 0b10001101&lt;/i2c_reg_index&gt;
  &lt;i2c_reg_data&gt;0&lt;/i2c_reg_data&gt;
&lt;/atom_i2c_data_entry&gt;
&lt;FINAL_atom_i2c_data_entry of="0xA97A-0xA97C  len=0x2=2"&gt;
  &lt;final_entry_index&gt;255 = 0xFF = 0b11111111&lt;/final_entry_index&gt;
&lt;/FINAL_atom_i2c_data_entry&gt;
&lt;atom_voltage_object_header_v4 of="0xA97C-0xA988  len=0xC=12"&gt;
  &lt;ucVoltageType&gt;VOLTAGE_TYPE_VDDC_0x1&lt;/ucVoltageType&gt;
  &lt;ucVoltageMode&gt;VOLTAGE_OBJ_SVID2_0x7&lt;/ucVoltageMode&gt;
  &lt;usSize&gt;12 = 0xC = 0b1100&lt;/usSize&gt;
&lt;/atom_voltage_object_header_v4&gt;
&lt;atom_voltage_object_header_v4 of="0xA988-0xA994  len=0xC=12"&gt;
  &lt;ucVoltageType&gt;VOLTAGE_TYPE_VDDCI_0x4&lt;/ucVoltageType&gt;
  &lt;ucVoltageMode&gt;VOLTAGE_OBJ_GPIO_LUT_0x0&lt;/ucVoltageMode&gt;
  &lt;usSize&gt;36 = 0x24 = 0b100100&lt;/usSize&gt;
&lt;/atom_voltage_object_header_v4&gt;
&lt;ATOM_GPIO_I2C_INFO of="0x9A18-0x9A1C  len=0x4=4"&gt;
  &lt;sHeader&gt;
    &lt;usStructureSize&gt;220 = 0xDC = 0b11011100&lt;/usStructureSize&gt;
    &lt;ucTableFormatRevision&gt;1&lt;/ucTableFormatRevision&gt;
    &lt;ucTableContentRevision&gt;1&lt;/ucTableContentRevision&gt;
  &lt;/sHeader&gt;
&lt;/ATOM_GPIO_I2C_INFO&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9A1C-0x9A37  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18536 = 0x4868 = 0b100100001101000&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18538 = 0x486A = 0b100100001101010&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18539 = 0x486B = 0b100100001101011&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18537 = 0x4869 = 0b100100001101001&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18536 = 0x4868 = 0b100100001101000&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18538 = 0x486A = 0b100100001101010&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18539 = 0x486B = 0b100100001101011&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18537 = 0x4869 = 0b100100001101001&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;144 = 0x90 = 0b10010000&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;0&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;144 = 0x90 = 0b10010000&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;8 = 0x8 = 0b1000&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;8 = 0x8 = 0b1000&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9A37-0x9A52  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18540 = 0x486C = 0b100100001101100&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18542 = 0x486E = 0b100100001101110&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18543 = 0x486F = 0b100100001101111&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18541 = 0x486D = 0b100100001101101&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18540 = 0x486C = 0b100100001101100&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18542 = 0x486E = 0b100100001101110&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18543 = 0x486F = 0b100100001101111&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18541 = 0x486D = 0b100100001101101&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;145 = 0x91 = 0b10010001&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;1&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;145 = 0x91 = 0b10010001&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;8 = 0x8 = 0b1000&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;8 = 0x8 = 0b1000&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9A52-0x9A6D  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18544 = 0x4870 = 0b100100001110000&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18546 = 0x4872 = 0b100100001110010&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18547 = 0x4873 = 0b100100001110011&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18545 = 0x4871 = 0b100100001110001&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18544 = 0x4870 = 0b100100001110000&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18546 = 0x4872 = 0b100100001110010&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18547 = 0x4873 = 0b100100001110011&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18545 = 0x4871 = 0b100100001110001&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;146 = 0x92 = 0b10010010&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;2 = 0x2 = 0b10&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;146 = 0x92 = 0b10010010&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;8 = 0x8 = 0b1000&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;8 = 0x8 = 0b1000&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9A6D-0x9A88  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18548 = 0x4874 = 0b100100001110100&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18550 = 0x4876 = 0b100100001110110&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18551 = 0x4877 = 0b100100001110111&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18549 = 0x4875 = 0b100100001110101&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18548 = 0x4874 = 0b100100001110100&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18550 = 0x4876 = 0b100100001110110&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18551 = 0x4877 = 0b100100001110111&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18549 = 0x4875 = 0b100100001110101&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;147 = 0x93 = 0b10010011&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;3 = 0x3 = 0b11&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;147 = 0x93 = 0b10010011&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;8 = 0x8 = 0b1000&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;8 = 0x8 = 0b1000&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9A88-0x9AA3  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18552 = 0x4878 = 0b100100001111000&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18554 = 0x487A = 0b100100001111010&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18555 = 0x487B = 0b100100001111011&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18553 = 0x4879 = 0b100100001111001&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18552 = 0x4878 = 0b100100001111000&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18554 = 0x487A = 0b100100001111010&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18555 = 0x487B = 0b100100001111011&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18553 = 0x4879 = 0b100100001111001&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;148 = 0x94 = 0b10010100&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;4 = 0x4 = 0b100&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;148 = 0x94 = 0b10010100&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;8 = 0x8 = 0b1000&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;8 = 0x8 = 0b1000&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9AA3-0x9ABE  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18556 = 0x487C = 0b100100001111100&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18558 = 0x487E = 0b100100001111110&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18559 = 0x487F = 0b100100001111111&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18557 = 0x487D = 0b100100001111101&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18556 = 0x487C = 0b100100001111100&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18558 = 0x487E = 0b100100001111110&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18559 = 0x487F = 0b100100001111111&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18557 = 0x487D = 0b100100001111101&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;149 = 0x95 = 0b10010101&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;5 = 0x5 = 0b101&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;149 = 0x95 = 0b10010101&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;8 = 0x8 = 0b1000&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;8 = 0x8 = 0b1000&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9ABE-0x9AD9  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18584 = 0x4898 = 0b100100010011000&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18586 = 0x489A = 0b100100010011010&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18587 = 0x489B = 0b100100010011011&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18585 = 0x4899 = 0b100100010011001&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18584 = 0x4898 = 0b100100010011000&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18586 = 0x489A = 0b100100010011010&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18587 = 0x489B = 0b100100010011011&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18585 = 0x4899 = 0b100100010011001&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;150 = 0x96 = 0b10010110&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;6 = 0x6 = 0b110&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;150 = 0x96 = 0b10010110&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;1&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;1&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;1&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;1&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
&lt;ATOM_GPIO_I2C_ASSIGMENT of="0x9AD9-0x9AF4  len=0x1B=27"&gt;
  &lt;usClkMaskRegisterIndex&gt;18560 = 0x4880 = 0b100100010000000&lt;/usClkMaskRegisterIndex&gt;
  &lt;usClkEnRegisterIndex&gt;18562 = 0x4882 = 0b100100010000010&lt;/usClkEnRegisterIndex&gt;
  &lt;usClkY_RegisterIndex&gt;18563 = 0x4883 = 0b100100010000011&lt;/usClkY_RegisterIndex&gt;
  &lt;usClkA_RegisterIndex&gt;18561 = 0x4881 = 0b100100010000001&lt;/usClkA_RegisterIndex&gt;
  &lt;usDataMaskRegisterIndex&gt;18560 = 0x4880 = 0b100100010000000&lt;/usDataMaskRegisterIndex&gt;
  &lt;usDataEnRegisterIndex&gt;18562 = 0x4882 = 0b100100010000010&lt;/usDataEnRegisterIndex&gt;
  &lt;usDataY_RegisterIndex&gt;18563 = 0x4883 = 0b100100010000011&lt;/usDataY_RegisterIndex&gt;
  &lt;usDataA_RegisterIndex&gt;18561 = 0x4881 = 0b100100010000001&lt;/usDataA_RegisterIndex&gt;
  &lt;sucI2cId&gt;
    &lt;gpio_id&gt;151 = 0x97 = 0b10010111&lt;/gpio_id&gt;
    &lt;bfHW_Capable&gt;true&lt;/bfHW_Capable&gt;
    &lt;bfHW_EngineID&gt;1&lt;/bfHW_EngineID&gt;
    &lt;bfI2C_LineMux&gt;7 = 0x7 = 0b111&lt;/bfI2C_LineMux&gt;
    &lt;Description&gt;151 = 0x97 = 0b10010111&lt;/Description&gt;
  &lt;/sucI2cId&gt;
  &lt;ucClkMaskShift&gt;0&lt;/ucClkMaskShift&gt;
  &lt;ucClkEnShift&gt;0&lt;/ucClkEnShift&gt;
  &lt;ucClkY_Shift&gt;0&lt;/ucClkY_Shift&gt;
  &lt;ucClkA_Shift&gt;0&lt;/ucClkA_Shift&gt;
  &lt;ucDataMaskShift&gt;8 = 0x8 = 0b1000&lt;/ucDataMaskShift&gt;
  &lt;ucDataEnShift&gt;8 = 0x8 = 0b1000&lt;/ucDataEnShift&gt;
  &lt;ucDataY_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataY_Shift&gt;
  &lt;ucDataA_Shift&gt;8 = 0x8 = 0b1000&lt;/ucDataA_Shift&gt;
  &lt;ucReserved1&gt;0&lt;/ucReserved1&gt;
  &lt;ucReserved2&gt;0&lt;/ucReserved2&gt;
&lt;/ATOM_GPIO_I2C_ASSIGMENT&gt;
</pre>
</details>


# Below is readme kept for upstream version.

#### PolarisBiosEditor tweaked by vaske version 3.8 with pro timings can buy on miningbios.com
#### https://www.miningbios.com

BTC donation address: 181dtEjhFWWxvHDmx2R3N41rnRPedSEUf5

one click timing feature should be used with care, it maybe not stable for you



### v1.7.3
- Fixed apply timings for Samsung memory
- Added support for New Samsung memory K4G80325FC
- Added timing for New Samsung K4G80325FC
- Applying from 1750 to upper

### v1.7.2
- Fixed apply timings for Hynix memory
- Added support for RX590
- Added support for New Hynix memory H5GC8H24AJ
- Added timing for New Hynix H5GC8H24AJ

### v1.7.1
- Updated Elpida Timing

### v1.7.0
- Added New timing for Hynix.
- Added Clock Stretch Amount.
- Added option for choosing timings on hynix Between Universal Hynix timing and Good hynix timing.
- Universal Hynix timing work on: H5GC8H24MJ, H5GQ8H24MJ, H5GQ4H24AJ.

### v1.6.9
- Fixed UI (updated design)
- Fixed and Updated all Timing's
- Added New strap for Micron and Hynix
- Added option for choosing timings on samsung between uber-mix 3.1 and 3.2, and on Micron between Good Micron timing and S Micron timing.
- Added Icon
- Added option for max. Mem. freq. (after one click timing patch button click automatically change max. mem. to 2300 MHz)

### v1.6.8
- Fixed Samsung Uber-Mix strap
- Added support for Hynix H5GQ4H24AJ
- Fixed fan mod option

### v1.6.7
- created solution and project files for ide
- support for device id 0x67ef
- better timings for micron memory
- firmware signature test / firmware signature in ascii
- editing of bios message (experimental)
- online check for new versions
- online display of developer notice

### v1.6.6
- support for rx550 device id 0x699F

### v1.6.5
- support up to 48 entrys in the timings table (more than 2 memory vendors)

### v1.6.4
- elpida timings fixed
- K4G41325FS memory support

### v1.6.3
- timing modification starts now at 1500 instead of 1750
- device id 67FF now also supported

### v1.6.2
- experimental: ubermix timings are now also applied to 4g SAMSUNG vram (K4G41325FC, K4G41325FE)
- timing modification starts now at 1750 instead of 2000

### v1.6.1
- hynix memory H5GC8H24MJ now recognized (same timings as H5GQ8H24MJ)

### v1.6
- window resizes properly now
- memory vendor detection
- one click timing patch (samsung, hynix, elpida, micron)

### v1.5
- added FanControlMode setting
- implemented some timing editor related code (not usable yet)

### v1.4.1
- replaced WPF components with Windows Forms to archive mono compatibility

Contribution from Sebohe:

### Build Dependencies

Ubuntu 16.04.2:

```
sudo apt-get install mono-complete
```

Arch Linux:

```
yaourt -Sy mono48
```
### Building

```
sh build.sh
```

### Executing

Just change your working directory to the PolarisBiosEditor and execute:

```
./run.sh
```
