# Echo 1-2 Loadouts

## How To Import

To import loadouts, follow these steps:

1. Start Arma 3

2. Enter the Virtual Arsenal by clicking **Tutorials** and then **Virtual Arsenal** from the main menu.

3. Click the drop-down of the loadout you want to import below, and then click the icon in the top-right to copy the loadout's script.

4. Re-open the game and click **Import** on the bottom of your screen to import the loadout from the copied script.

5. Click **Save** on the bottom of your screen to save the loadout.

6. Repeat steps **3** to **4** for each loadout. 

## Loadouts

??? note "TG Ammo Bearer"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_Kitbag_rgr";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 3 do {this addItemToVest "HandGrenade";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	this addItemToVest "SmokeShell";
	for "_i" from 1 to 22 do {this addItemToBackpack "30rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 3 do {this addItemToBackpack "HandGrenade";};
	for "_i" from 1 to 6 do {this addItemToBackpack "SmokeShell";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Anti-Air"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";
	this addWeapon "launch_B_Titan_tna_F";
	this addSecondaryWeaponItem "Titan_AA";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_AssaultPack_tna_F";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "Titan_AA";
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Anti-Tank (Heavy)"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";
	this addWeapon "launch_B_Titan_short_tna_F";
	this addSecondaryWeaponItem "Titan_AT";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_AssaultPack_tna_F";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "Titan_AT";
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Anti-Tank (Light)"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";
	this addWeapon "launch_MRAWS_green_F";
	this addSecondaryWeaponItem "MRAWS_HEAT_F";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_AssaultPack_tna_F";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	this addItemToUniform "FirstAidKit";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "FirstAidKit";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	this addItemToVest "HandGrenade";
	for "_i" from 1 to 2 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 2 do {this addItemToBackpack "MRAWS_HE_F";};
	this addItemToBackpack "MRAWS_HEAT_F";
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Assistant Anti-Air"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_Carryall_oli";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	this addItemToUniform "FirstAidKit";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "FirstAidKit";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 2 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 3 do {this addItemToBackpack "Titan_AA";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Assistant Anti-Tank (Heavy)"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_Carryall_oli";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	this addItemToUniform "FirstAidKit";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "FirstAidKit";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 2 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 3 do {this addItemToBackpack "Titan_AT";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Assistant Anti-Tank (Light)"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_Carryall_oli";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	this addItemToUniform "FirstAidKit";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "FirstAidKit";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 2 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 3 do {this addItemToBackpack "MRAWS_HEAT_F";};
	for "_i" from 1 to 3 do {this addItemToBackpack "MRAWS_HE_F";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Autorifleman"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "LMG_Mk200_black_F";
	this addPrimaryWeaponItem "muzzle_snds_H";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_blk_F";
	this addPrimaryWeaponItem "200Rnd_65x39_cased_Box";
	this addPrimaryWeaponItem "bipod_01_F_blk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_AssaultPack_tna_F";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "HandGrenade";};
	for "_i" from 1 to 2 do {this addItemToVest "200Rnd_65x39_cased_Box";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 2 do {this addItemToBackpack "200Rnd_65x39_cased_Box";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Diver"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_SDAR_F";
	this addPrimaryWeaponItem "20Rnd_556x45_UW_mag";

	comment "Add containers";
	this forceAddUniform "U_B_Wetsuit";
	this addVest "V_RebreatherB";
	this addBackpack "B_ViperHarness_blk_F";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 10 do {this addItemToUniform "20Rnd_556x45_UW_mag";};
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 8 do {this addItemToBackpack "30Rnd_556x45_Stanag";};
	for "_i" from 1 to 10 do {this addItemToBackpack "20Rnd_556x45_UW_mag";};
	for "_i" from 1 to 5 do {this addItemToBackpack "HandGrenade";};
	for "_i" from 1 to 4 do {this addItemToBackpack "DemoCharge_Remote_Mag";};
	this addGoggles "G_Diving";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_blk_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Engineer"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_Kitbag_rgr";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	this addItemToUniform "FirstAidKit";
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 4 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "FirstAidKit";};
	for "_i" from 1 to 2 do {this addItemToVest "HandGrenade";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	this addItemToBackpack "ToolKit";
	for "_i" from 1 to 2 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "MineDetector";
	this addItemToBackpack "SatchelCharge_Remote_Mag";
	for "_i" from 1 to 4 do {this addItemToBackpack "DemoCharge_Remote_Mag";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Marksman"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_SPAR_03_blk_F";
	this addPrimaryWeaponItem "muzzle_snds_B";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_AMS";
	this addPrimaryWeaponItem "20Rnd_762x51_Mag";
	this addPrimaryWeaponItem "bipod_01_F_blk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_AssaultPack_tna_F";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "HandGrenade";};
	for "_i" from 1 to 10 do {this addItemToVest "20Rnd_762x51_Mag";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "optic_Nightstalker";
	for "_i" from 1 to 8 do {this addItemToBackpack "20Rnd_762x51_Mag";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Medic"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12_lush_F";
	this addPrimaryWeaponItem "muzzle_snds_B_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "75rnd_762x39_AK12_Lush_Mag_F";
	this addPrimaryWeaponItem "bipod_01_F_khk";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier1_tna_F";
	this addBackpack "B_Kitbag_rgr";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToVest "HandGrenade";};
	for "_i" from 1 to 4 do {this addItemToVest "75rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 15 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "Medikit";
	for "_i" from 1 to 5 do {this addItemToBackpack "SmokeShellRed";};
	for "_i" from 1 to 5 do {this addItemToBackpack "SmokeShell";};
	this addItemToBackpack "75rnd_762x39_AK12_Lush_Mag_F";
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Rifleman CQB"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "arifle_AK12U_lush_F";
	this addPrimaryWeaponItem "acc_pointer_IR";
	this addPrimaryWeaponItem "optic_Arco_AK_lush_F";
	this addPrimaryWeaponItem "30rnd_762x39_AK12_Lush_Mag_F";
	this addWeapon "hgun_Pistol_heavy_01_green_F";
	this addHandgunItem "muzzle_snds_acp";
	this addHandgunItem "acc_flashlight_pistol";
	this addHandgunItem "optic_MRD_black";
	this addHandgunItem "11Rnd_45ACP_Mag";

	comment "Add containers";
	this forceAddUniform "U_B_CTRG_Soldier_3_F";
	this addVest "V_PlateCarrier2_tna_F";
	this addBackpack "B_AssaultPack_tna_F";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 5 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 2 do {this addItemToUniform "HandGrenade";};
	for "_i" from 1 to 3 do {this addItemToVest "11Rnd_45ACP_Mag";};
	for "_i" from 1 to 7 do {this addItemToVest "30rnd_762x39_AK12_Lush_Mag_F";};
	for "_i" from 1 to 4 do {this addItemToVest "HandGrenade";};
	for "_i" from 1 to 8 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "muzzle_snds_B_lush_F";
	for "_i" from 1 to 8 do {this addItemToBackpack "30rnd_762x39_AK12_Lush_Mag_F";};
	this addHeadgear "H_HelmetB_Enh_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Sniper"
	```
	comment "Exported from Arsenal by TGxSilK";

	comment "[!] UNIT MUST BE LOCAL [!]";
	if (!local this) exitWith {};

	comment "Remove existing items";
	removeAllWeapons this;
	removeAllItems this;
	removeAllAssignedItems this;
	removeUniform this;
	removeVest this;
	removeBackpack this;
	removeHeadgear this;
	removeGoggles this;

	comment "Add weapons";
	this addWeapon "srifle_LRR_F";
	this addPrimaryWeaponItem "optic_LRPS";
	this addPrimaryWeaponItem "7Rnd_408_Mag";
	this addWeapon "hgun_Pistol_heavy_01_green_F";
	this addHandgunItem "muzzle_snds_acp";
	this addHandgunItem "acc_flashlight_pistol";
	this addHandgunItem "optic_MRD_black";
	this addHandgunItem "11Rnd_45ACP_Mag";

	comment "Add containers";
	this forceAddUniform "U_B_FullGhillie_lsh";
	this addVest "V_TacVest_khk";
	this addBackpack "B_AssaultPack_rgr";

	comment "Add binoculars";
	this addMagazine "Laserbatteries";
	this addWeapon "Laserdesignator_01_khk_F";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "SmokeShell";};
	for "_i" from 1 to 2 do {this addItemToUniform "SmokeShellRed";};
	for "_i" from 1 to 2 do {this addItemToUniform "HandGrenade";};
	for "_i" from 1 to 2 do {this addItemToUniform "11Rnd_45ACP_Mag";};
	for "_i" from 1 to 7 do {this addItemToVest "7Rnd_408_Mag";};
	for "_i" from 1 to 3 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "optic_Nightstalker";
	for "_i" from 1 to 4 do {this addItemToBackpack "7Rnd_408_Mag";};
	this addHeadgear "H_HelmetB_tna_F";
	this addGoggles "G_Balaclava_TI_G_tna_F";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "ItemRadio";
	this linkItem "ItemGPS";
	this linkItem "NVGogglesB_grn_F";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```