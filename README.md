# qss-particles

copy particles folder to gamedir, `r_particledesc qssm13` to load all effects, `r_particledesc classic` to disable

**for per map effects add to a maps .ent worldspawn:**

```
e4m7 worldspawn:

{
"message" "Azure Agony"
"worldtype" "0"
"wad" "gfx/medieval.wad"
"classname" "worldspawn"
"sounds" "7"
"_texpart_sky4" "lib_effects_0_e4m7.skysnow"		//make it snow
}

ctf5 worldspawn:

{
"message" "Da Ancient War Grounds"
"classname" "worldspawn"
"wad" "texture.wad"
"_texpart_*lava1" "lib_effects_0_lava.tex_*lava1"	// add lava particle effects
}
```

**for per map effects to an entitiy add to a maps .ent:**

```{
"_color" "246 154 84"
"_tb_group" "151"
"angle" "0"
"classname" "light_flame_large_yellow"
"delay" "2"
"light" "225"
"origin" "1120 -128 407"
"wait" "1.67"
"emiteffect" "lib_effects_0_ad_smoke.DPP_ITSVELSMOKEGREY1"
}
