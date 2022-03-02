# Echo 1-2 Loadouts

## How To Import

To import loadouts, follow these steps:

1. Start Arma 3.

2. Enter the Virtual Arsenal by clicking **Tutorials** and then **Virtual Arsenal** from the main menu.

3. Return to this site, click the drop-down of the loadout you want to import below, and click the icon in the top-right to copy the loadout's script.

4. Re-open the game and click **Import** on the bottom of your screen to import the loadout from the copied script.

5. Click **Save** on the bottom of your screen and enter the name of the loadout to save it.

6. Repeat steps **3** to **5** for each loadout. 

## Loadout Scripts

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
	this addWeapon "rhs_weap_m4a1_carryhandle_grip";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 8 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 20 do {this addItemToBackpack "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle_grip";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhs_weap_fim92";
	this addSecondaryWeaponItem "rhs_fim92_mag";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 7 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "rhs_fim92_mag";
	this addItemToBackpack "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle_grip";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhs_weap_fgm148";
	this addSecondaryWeaponItem "rhs_fgm148_magazine_AT";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 7 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle_grip";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhs_weap_maaws";
	this addSecondaryWeaponItem "rhs_optic_maaws";
	this addSecondaryWeaponItem "rhs_mag_maaws_HEAT";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 7 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "rhs_mag_maaws_HEAT";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle_grip";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "B_Carryall_mcamo";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_lerca_1200_black";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 8 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 2 do {this addItemToBackpack "rhs_fim92_mag";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle_grip";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "B_Carryall_mcamo";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_lerca_1200_black";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 8 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 4 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "rhs_fgm148_magazine_AT";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle_grip";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "B_Carryall_mcamo";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_lerca_1200_black";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 8 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 2 do {this addItemToBackpack "rhs_mag_maaws_HEAT";};
	this addItemToBackpack "rhs_mag_maaws_HE";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	[this,"TFAegis"] call BIS_fnc_setUnitInsignia;
	```

??? note "TG Autorifleman (Heavy)"
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
	this addWeapon "rhs_weap_m240B";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhsusf_100Rnd_762x51";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_machinegunner";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 2 do {this addItemToVest "rhsusf_100Rnd_762x51";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 4 do {this addItemToBackpack "rhsusf_100Rnd_762x51";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Autorifleman (Light)"
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
	this addWeapon "rhs_weap_m249_pip";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhsusf_100Rnd_556x45_soft_pouch_ucp";
	this addPrimaryWeaponItem "rhsusf_acc_saw_bipod";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_saw";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	this addItemToVest "rhsusf_200Rnd_556x45_box";
	this addItemToVest "rhsusf_100Rnd_556x45_soft_pouch_ucp";
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 4 do {this addItemToBackpack "rhsusf_100Rnd_556x45_soft_pouch_ucp";};
	this addItemToBackpack "rhsusf_200Rnd_556x45_box";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Breachman"
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
	this addWeapon "rhs_weap_M590_8RD";
	this addPrimaryWeaponItem "rhsusf_8Rnd_00Buck";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_FMJ";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 4 do {this addItemToVest "rhsusf_8Rnd_00Buck";};
	for "_i" from 1 to 2 do {this addItemToVest "rhsusf_8Rnd_Slug";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_mk84";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 3 do {this addItemToBackpack "rhsusf_8Rnd_00Buck";};
	for "_i" from 1 to 3 do {this addItemToBackpack "rhsusf_8Rnd_Slug";};
	for "_i" from 1 to 2 do {this addItemToBackpack "rhs_mag_m67";};
	for "_i" from 1 to 2 do {this addItemToBackpack "rhs_mag_mk84";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_lerca_1200_black";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 8 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "ToolKit";
	this addItemToBackpack "MineDetector";
	for "_i" from 1 to 3 do {this addItemToBackpack "rhsusf_m112_mag";};
	this addItemToBackpack "rhsusf_m112x4_mag";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Grenadier"
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
	this addWeapon "rhs_weap_m4a1_carryhandle_m203";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 3 do {this addItemToVest "rhs_mag_M441_HE";};
	for "_i" from 1 to 7 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 9 do {this addItemToBackpack "rhs_mag_M441_HE";};
	for "_i" from 1 to 6 do {this addItemToBackpack "rhs_mag_m714_White";};
	for "_i" from 1 to 4 do {this addItemToBackpack "rhs_mag_m713_Red";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_sr25";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_M8541_mrds";
	this addPrimaryWeaponItem "rhsusf_20Rnd_762x51_SR25_m118_special_Mag";
	this addPrimaryWeaponItem "rhsusf_acc_harris_bipod";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_lrf_Vector21";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 5 do {this addItemToVest "rhsusf_20Rnd_762x51_SR25_m118_special_Mag";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "rhsusf_acc_su230_mrds";
	for "_i" from 1 to 4 do {this addItemToBackpack "rhsusf_20Rnd_762x51_SR25_m118_special_Mag";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_su230_mrds";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip1";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_medic";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 7 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	this addItemToBackpack "Medikit";
	for "_i" from 1 to 15 do {this addItemToBackpack "FirstAidKit";};
	for "_i" from 1 to 4 do {this addItemToBackpack "rhs_mag_an_m8hc";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m4a1_carryhandle";
	this addPrimaryWeaponItem "rhsusf_acc_eotech_552";
	this addPrimaryWeaponItem "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	this addPrimaryWeaponItem "rhsusf_acc_grip2";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_rifleman_alt";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_m24";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	this addItemToUniform "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";
	for "_i" from 1 to 7 do {this addItemToVest "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_mk84";};
	for "_i" from 1 to 8 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "rhsusf_acc_su230_mrds";
	for "_i" from 1 to 5 do {this addItemToBackpack "rhs_mag_30Rnd_556x45_M855A1_Stanag_Tracer_Red";};
	for "_i" from 1 to 2 do {this addItemToBackpack "rhs_mag_an_m8hc";};
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

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
	this addWeapon "rhs_weap_m40a5";
	this addPrimaryWeaponItem "rhsusf_acc_anpeq15side_bk";
	this addPrimaryWeaponItem "rhsusf_acc_nxs_3515x50_md";
	this addPrimaryWeaponItem "rhsusf_5Rnd_762x51_AICS_m118_special_Mag";
	this addPrimaryWeaponItem "rhsusf_acc_harris_swivel";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp_sniper";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_lrf_Vector21";

	comment "Add items to containers";
	for "_i" from 1 to 3 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 3 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_FMJ";};
	for "_i" from 1 to 2 do {this addItemToVest "rhs_mag_m67";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 8 do {this addItemToVest "rhsusf_5Rnd_762x51_AICS_m118_special_Mag";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "rhsusf_acc_nxs_3515x50_md";
	this addItemToBackpack "rhsusf_acc_su230_mrds";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```

??? note "TG Sniper (Heavy)"
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
	this addWeapon "rhs_weap_M107";
	this addPrimaryWeaponItem "rhsusf_acc_premier_mrds";
	this addPrimaryWeaponItem "rhsusf_mag_10Rnd_STD_50BMG_M33";
	this addWeapon "rhsusf_weap_m9";
	this addHandgunItem "rhsusf_mag_15Rnd_9x19_JHP";

	comment "Add containers";
	this forceAddUniform "rhs_uniform_acu_ucp2";
	this addVest "rhsusf_spcs_ucp";
	this addBackpack "rhsusf_assault_eagleaiii_ucp";

	comment "Add binoculars";
	this addWeapon "rhsusf_bino_lrf_Vector21";

	comment "Add items to containers";
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_JHP";};
	for "_i" from 1 to 2 do {this addItemToUniform "rhsusf_mag_15Rnd_9x19_FMJ";};
	for "_i" from 1 to 4 do {this addItemToVest "rhs_mag_an_m8hc";};
	for "_i" from 1 to 5 do {this addItemToBackpack "FirstAidKit";};
	this addItemToBackpack "rhsusf_bino_lrf_Vector21";
	for "_i" from 1 to 2 do {this addItemToBackpack "rhsusf_mag_10Rnd_STD_50BMG_M33";};
	this addItemToBackpack "rhsusf_mag_10Rnd_STD_50BMG_mk211";
	this addHeadgear "rhsusf_ach_helmet_ESS_ucp_alt";

	comment "Add items";
	this linkItem "ItemMap";
	this linkItem "ItemCompass";
	this linkItem "ItemWatch";
	this linkItem "rhsusf_radio_anprc152";
	this linkItem "ItemGPS";
	this linkItem "rhsusf_ANPVS_15";

	comment "Set identity";
	[this,"RussianHead_5","male01gre"] call BIS_fnc_setIdentity;
	```