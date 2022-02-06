# Echo 1-2 Loadouts

Click the drop-down for each loadout to see its script. Click the icon next to the text to quickly copy the loadout.

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