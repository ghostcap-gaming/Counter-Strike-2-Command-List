# Counter-Strike-2-Command-List
This repository contains a comprehensive list of all commands, cvars, and convars available in the newly released Counter-Strike 2. 

It aims to help players, server administrators, and modders familiarize themselves with the game's configurable settings and controls to optimize gameplay, customize user experience, and manage servers. 

Please join <https://www.ghostcap.com/> or <https://alliedmods.net/> if you're interested in learning more about the technical details of Counter-Strike 2.

If you want a nice front end where you can quickly search commands, then visit this blog post <https://www.ghostcap.com/cs2-commands/>

## How to enable sv_cheats?
You can set sv_cheats to 1 on the server, but clients will receive a message saying "[Server] Cheats cannot be enabled on this server," unless they launch the game with the -dev option. 

If launched with -dev, clients will see the message "[Developer] SetConVar: sv_cheats = "true"," and the server will allow cheats like the "give" command to be used. 

However, the client will still believe that sv_cheats is set to 0.

Thanks to domino_ mod36#3456 for this.

## Usage
If you use this table on your website then please link to the repository.

## Disclaimer
This repository is a community-driven resource and is not affiliated with the official Counter-Strike 2 developers or the game itself. Please use the information provided at your own risk and always be mindful of potential game updates that may alter the commands or their functions.

## All commands current as of 23/3/2023
| Command | Type | Flags | Description |
| --- | --- | --- | --- |
| ent_ungrab | cmd | sv, cheat | un-grabs all objects |
| ent_vcollide_wireframe | cmd | sv, cheat | Displays the interpolated vcollide wireframe pm am entity.  Arguments |
| ent_viewoffset | cmd | sv, cheat | Displays the eye position for the given entity(ies) in red.  Arguments |
| entity_log_load_unserialize | 0 | sv, cl, rep, cheat | Output unserialization of entities on map load. 0 - off, 1 - client/server, 2 - server, 3 - client |
| entity_lump_list | cmd |  | List all known entity lumps |
| entity_lump_spew | cmd |  | Dump the contents of an entity lump |
| entityreport | cmd | sv | Reports all extant entities. Optional 2nd arg is a substring of a classname that the list will be filtered by. |
| entitysummary | cmd | sv | Summarizes (by class) all extant entities. Optional 2nd arg is a substring of a classname that the list will be filtered by. |
| ents | cmd | sv | List server entities, sorted by spawn group |
| escape | cmd | clientcmd_can_execute | Escape key pressed. |
| exec | cmd | norecord | Execute a cfg file |
| exec_async | cmd | cheat, norecord | Execute a cfg file over time |
| execifexists | cmd | norecord | Execute a cfg file if file exists |
| execute_command_every_frame | 0 | cheat |  |
| explode | cmd | sv, cheat | Kills the player with explosive damage |
| explodevector | cmd | sv, cheat | Kills a player applying an explosive force. Usage |
| fadein | cmd | sv, cheat | fadein {time r g b} |
| fadeout | cmd | sv, cheat | fadeout {time r g b} |
| ff_damage_bullet_penetration | 0 | sv, cl, rep, release | If friendly fire is off, this will scale the penetration power and damage a bullet does when penetrating another friendly player |
| ff_damage_decoy_explosion | false | sv, cl, rep, release | Enables or disables team damage from decoy detonation |
| ff_damage_reduction_bullets | 0.33 | sv, cl, rep, release | How much to reduce damage done to teammates when shot.  Range is from 0 - 1 (with 1 being damage equal to what is done to an enemy) |
| ff_damage_reduction_grenade | 0.85 | sv, cl, rep, release | How much to reduce damage done to teammates by a thrown grenade.  Range is from 0 - 1 (with 1 being damage equal to what is done to an enemy) |
| ff_damage_reduction_grenade_self | 1 | sv, cl, rep, release | How much to damage a player does to himself with his own grenade.  Range is from 0 - 1 (with 1 being damage equal to what is done to an enemy) |
| ff_damage_reduction_other | 0.4 | sv, cl, rep, release | How much to reduce damage done to teammates by things other than bullets and grenades.  Range is from 0 - 1 (with 1 being damage equal to what is done to an enemy) |
| find | cmd |  | Find concommands with the specified string in their name/help text. |
| findflags | cmd |  | Find concommands by flags. |
| firetarget | cmd | sv, cheat |  |
| firstperson | cmd | cl, execute_per_tick | Switch to firstperson camera. |
| fish_debug | false | cl, cheat | Show debug info for fish |
| fish_dormant | false | sv, rep, cheat | Turns off interactive fish behavior. Fish become immobile and unresponsive. |
| fog_color | -1.000000 -1.000000 -1.000000 | cl, cheat |  |
| fog_colorskybox | -1.000000 -1.000000 -1.000000 | cl, cheat |  |
| fog_enable | true | cl, cheat | Enable fog |
| fog_enableskybox | true | cl, cheat |  |
| fog_end | -1 | cl, cheat |  |
| fog_endskybox | -1 | cl, cheat |  |
| fog_hdrcolorscale | -1 | cl, cheat |  |
| fog_hdrcolorscaleskybox | -1 | cl, cheat |  |
| fog_maxdensity | -1 | cl, cheat |  |
| fog_maxdensityskybox | -1 | cl, cheat |  |
| fog_override | 0 | cl, cheat | Overrides the map's fog settings (-1 populates fog_ vars with map's values) |
| fog_override_color | cmd | cheat | Sets the fog color override |
| fog_override_enable | false | cheat | Use fog_override convars instead of world fog data |
| fog_override_end | 3500 | cheat |  |
| fog_override_exponent | 2 | cheat |  |
| fog_override_max_density | 0.4 | cheat |  |
| fog_override_start | 1000 | cheat |  |
| fog_start | -1 | cl, cheat |  |
| fog_startskybox | -1 | cl, cheat |  |
| fov_cs_debug | 0 | cl, cheat | Sets the view fov if cheats are on. |
| fov_desired | 75 | cl, a, user | Sets the base field-of-view. |
| fp_trace | cmd |  | Toggle field path tracing to file |
| fps_max | 0 | a, release | Frame rate limiter.  0=no limit.  Does not apply to dedicated server. |
| fps_max_tools | 120 | a | Additional frame rate limit while in tools mode and a window other than the game window has focus. Note that fps_max still applies, this only allows the maximum frame rate for tools mode to be lower. 0=no tools specific limit. |
| fps_max_ui | 120 | a | Frame rate limiter while the game UI is displayed.  0=no limit.  Does not apply to dedicated server. |
| fs_clear_open_duplicate_times | cmd |  | Clear the list of files that have been opened. |
| fs_dump_open_duplicate_times | cmd |  | Set fs_report_long_reads 1 before loading to use this. Prints a list of files that were opened more than once and ~how long was spent reading from them. |
| fs_report_sync_opens | 0 | release | 0 |
| fs_spew_readfieldlist | cmd | cheat | index <threshold bytes> |
| func_break_max_pieces | 15 | sv, a, rep |  |
| g_debug_angularsensor | false | sv, cheat |  |
| g_debug_constraint_sounds | false | sv, cheat | Enable debug printing about constraint sounds. |
| g_debug_ragdoll_visualize | false | cl, cheat |  |
| game_alias | cmd | release | Set the configuration of game type and mode based on game alias like 'deathmatch'. |
| game_mode | 1 | sv, cl, rep, release | The current game mode (based on game type). See GameModes.txt. |
| game_type | 0 | sv, cl, rep, release | The current game type. See GameModes.txt. |
| gameinstructor_dump_open_lessons | cmd | cl, cheat | Gives a list of all currently open lessons. |
| gameinstructor_dump_run_lesson_counts | cmd | cl, cheat | Gives a list of lessons that been completed or shown |
| gameinstructor_enable | true | cl, a, release | Display in game lessons that teach new players. |
| gameinstructor_find_errors | false | cl, cheat | Set to 1 and the game instructor will run EVERY scripted command to uncover errors. |
| gameinstructor_reload_lessons | cmd | cl | Shuts down all open lessons and reloads them from the script file. |
| gameinstructor_teach_lesson | cmd | cl | Force a specific lesson to be triggered |
| gameinstructor_verbose | 0 | cl, cheat | Set to 1 for standard debugging or 2 (in combo with gameinstructor_verbose_lesson) to show update actions. |
| gameinstructor_verbose_lesson | 0 | cl, cheat | Display more verbose information for lessons have this name. |
| gameui_activate | cmd |  | Shows the game UI |
| gameui_allowescape | cmd |  | Escape key allowed to hide game UI |
| gameui_allowescapetoshow | cmd |  | Escape key allowed to show game UI |
| gameui_hide | cmd |  | Hides the game UI |
| gameui_preventescape | cmd |  | Escape key doesn't hide game UI |
| gameui_preventescapetoshow | cmd |  | Escape key doesn't show game UI |
| getpos | cmd | cl | dump position and angles to the console |
| getpos_exact | cmd | cl | dump origin and angles to the console |
| give | cmd | sv, vconsole_fuzzy | Give item to player.  Arguments |
| givecurrentammo | cmd | sv, cheat | Give a supply of ammo for current weapon.. |
| gl_clear_gray | false | cl, cheat | Clear the back buffer to gray every frame. |
| gl_clear_randomcolor | false | cl, cheat | Clear the back buffer to random colors every frame. Helps spot open seams in geometry. |
| global_set | cmd | sv, cheat | global_set <globalname> <state> |
| glow_outline_width | 6 | cl, cheat | Width of glow outline effect in screen space. |
| glow_use_tolerance | 0.85 | cl, rep, cheat |  |
| god | cmd | sv, cheat | Toggle by default, or 0 to disable and 1 to enable. Player becomes invulnerable. |
| gotv_theater_container | 0 | cl, release | Enables GOTV theater mode for the specified container, setting it to 'live' will play top live matches |
| grep | cmd |  | grep line for pattern, print out matching lines only |
| groups | cmd | sv | Show status of all spawn groups. |
| handforce_inner | 1 | sv, cl, rep, cheat |  |
| handforce_outer | 8 | sv, cl, rep, cheat |  |
| handforce_scale | 1.5 | sv, cl, rep, cheat |  |
| headforce_inner | 8 | sv, cl, rep, cheat |  |
| headforce_outer | 16 | sv, cl, rep, cheat |  |
| headforce_strength | 10 | sv, cl, rep, cheat |  |
| healthshot_allow_use_at_full | true | sv, cl, rep, release |  |
| healthshot_health | 50 | sv, cl, rep, release |  |
| healthshot_healthboost_damage_multiplier | 1 | sv, rep, release |  |
| healthshot_healthboost_speed_multiplier | 1 | sv, cl, rep, release |  |
| healthshot_healthboost_time | 0 | sv, cl, rep, release |  |
| help | cmd |  | Find help about a convar/concommand. |
| hideconsole | cmd | norecord | Hide the console. |
| hidehud | 0 | cl, cheat | bitmask |
| hideoverviewmap | cmd | cl | Hides the overview map |
| hideradar | cmd | cl | Hides HUD radar |
| hint_panel_fadein | 0.3 | sv, cl, rep, cheat |  |
| hint_panel_fadeout | 0.3 | sv, cl, rep, cheat |  |
| hmd_anchor_rotate | cmd | cl |  |
| host_framerate | 0 | release | Set to lock per-frame time elapse. |
| host_timescale | 1 | rep, cheat | Prescale the clock by this amount. |
| host_timescale_dec | cmd | cheat | Decrement the timescale by one step |
| host_timescale_inc | cmd | cheat | Increment the timescale by one step |
| host_workshop_collection | cmd | sv | Host a workshop map collection as a mapgroup |
| host_workshop_map | cmd | sv | Get the latest version of the map and host it on this server. |
| host_writeconfig | cmd |  | Saves out the user config values. |
| hostage_debug | 0 | sv, cheat | Show hostage AI debug information |
| hostage_is_silent | false | sv, cheat | When set, the hostage won't play any code driven response rules lines |
| hostfile | host.txt | sv, release | The HOST file to load. |
| hostip | -1062731516 | release | Host game server ip |
| hostname | star @STR | release | Hostname for server. |
| hostname_in_client_status | false | release | Show server hostname in client status. |
| hostport | 27015 | release | Host game server port |
| hud_fastswitch | 0 | cl, a |  |
| hud_reloadscheme | cmd | cl | Reloads hud layout and animation scripts. |
| hud_scaling | 1 | cl, a | Scales hud elements |
| hud_showtargetid | true | cl, a, per_user | Enables display of target names |
| hurtme | cmd | sv, cheat | Hurts the player.  Arguments |
| ic | cmd | cl | interp entity count |
| ik_debug_chain_to_filter_by | 0 | sv, cl, rep, cheat |  |
| ik_debug_fabrik_backwards_iteration_toggle | cmd |  |  |
| ik_debug_fabrik_forwards_iteration_toggle | cmd |  |  |
| ik_enable | true | cheat | Enable IK. |
| ik_hinge_debug_bone_index | -1 | sv, cl, rep, cheat |  |
| ime_hkl_info | cmd | norecord | Spew IME HKL info. |
| ime_info | cmd | norecord | Spew IME info. |
| ime_supported_info | cmd | norecord | Spew IME Supported info. |
| imgui_set_selection | cmd | sv, cheat | Sets ImGui selection |
| imgui_set_status_text | cmd | sv, cheat | Sets ImGui header status text |
| impulse | cmd | cl | Triggers impulse command |
| incrementvar | cmd | norecord | Increment specified convar value. |
| inferno_child_spawn_interval_multiplier | 0.1 | sv, cheat | Amount spawn interval increases for each child |
| inferno_child_spawn_max_depth | 4 | sv, rep, release |  |
| inferno_damage | 40 | sv, cheat | Damage per second |
| inferno_debug | false | sv, cheat |  |
| inferno_dlight_spacing | 200 | cl, cheat | Inferno dlights are at least this far apart |
| inferno_flame_lifetime | 7 | sv, rep, release | Average lifetime of each flame in seconds |
| inferno_flame_spacing | 42 | sv, cheat | Minimum distance between separate flame spawns |
| inferno_forward_reduction_factor | 0.9 | sv, cheat |  |
| inferno_friendly_fire_duration | 6 | sv, cheat | For this long, FF is credited back to the thrower. |
| inferno_initial_spawn_interval | 0.02 | sv, cheat | Time between spawning flames for first fire |
| inferno_max_child_spawn_interval | 0.5 | sv, cheat | Largest time interval for child flame spawning |
| inferno_max_flames | 16 | sv, rep, release | Maximum number of flames that can be created |
| inferno_max_range |  |  |  |
| inferno_per_flame_spawn_duration | 3 | sv, cheat | Duration each new flame will attempt to spawn new flames |
| inferno_scorch_decals | false | sv, cheat |  |
| inferno_smoke_volume_density | 0.1 | sv, cheat |  |
| inferno_spawn_angle | 45 | sv, cheat | Angular change from parent |
| inferno_surface_offset | 20 | sv, cheat |  |
| inferno_velocity_decay_factor | 0.2 | sv, cheat |  |
| inferno_velocity_factor | 0.003 | sv, cheat |  |
| inferno_velocity_normal_factor | 0 | sv, cheat |  |
| input_button_code_is_scan_code | true | a | Bind keys based on keyboard position instead of key name |
| input_filter_relative_analog_inputs | false | cl, a |  |
| input_forceuser | -1 | cheat | Force user input to this split screen player. |
| instant_replay_goto_tick | cmd |  | Goto a direct timestamp of the replay |
| instant_replay_goto_tick_relative | cmd |  | Goto a direct timestamp of the replay |
| instant_replay_live | cmd |  | If in replay, jumps back to live |
| instant_replay_pause | cmd |  | Pauses instant replay. |
| instant_replay_resume | cmd |  | Resumes instant replay. |
| instant_replay_skip | cmd |  | Number of seconds to skip back to instant replay from current position |
| instant_replay_skip_live | cmd |  | Number of seconds to skip back to instant replay from live |
| instant_replay_timescale | cmd |  | Sets instant replay speed. |
| instant_replay_togglepause | cmd |  | Toggles instant replay. |
| invnext | cmd | cl, server_can_execute |  |
| invnextselect | cmd | cl, server_can_execute |  |
| invprev | cmd | cl, server_can_execute |  |
| invprevselect | cmd | cl, server_can_execute |  |
| ip | 0 | release | Overrides IP for multihomed hosts |
| iv_debug | cmd | cl | Spew interpolated var info for entity. |
| iv_debugbone | 0 | release | Debug bone name for interpolation spew of CAnimationState. |
| iv_interp | cmd | cl | Spew interpolated var info for entity. |
| iv_off | cmd | cl | Turn off all interpolation variable spew. |
| iv_on | cmd | cl | Spew both interpolated var debug info and history for entity. |
| joy_advanced | false | cl, a |  |
| joy_advaxisr | 0 | cl, a |  |
| joy_advaxisu | 0 | cl, a |  |
| joy_advaxisv | 0 | cl, a |  |
| joy_advaxisx | 0 | cl, a |  |
| joy_advaxisy | 0 | cl, a |  |
| joy_advaxisz | 0 | cl, a |  |
| joy_axisbutton_threshold | 0.3 | a | Analog axis range before a button press is registered. |
| joy_axisr_deadzone | 0.15 | a, per_user |  |
| joy_axisr_relative | false | a, per_user |  |
| joy_axisu_deadzone | 0.15 | a, per_user |  |
| joy_axisu_relative | false | a, per_user |  |
| joy_axisv_deadzone | 0.15 | a, per_user |  |
| joy_axisv_relative | false | a, per_user |  |
| joy_axisx_deadzone | 0.15 | a, per_user |  |
| joy_axisx_relative | false | a, per_user |  |
| joy_axisy_deadzone | 0.15 | a, per_user |  |
| joy_axisy_relative | false | a, per_user |  |
| joy_axisz_deadzone | 0.15 | a, per_user |  |
| joy_axisz_relative | false | a, per_user |  |
| joy_circle_correct_mode | 1 | cl, a, per_user |  |
| joy_circle_correct_mode_vehicle | 2 | cl, a, per_user |  |
| joy_display_input |  |  |  |
| joy_forward_sensitivity | 1 | cl, a, per_user |  |
| joy_movement_stick | false | cl, a, per_user | Which stick controls movement (0 is left stick) |
| joy_name | joystick | cl, a |  |
| joy_pitch_sensitivity | 3 | cl, a, per_user |  |
| joy_pitchsensitivity | 1 | cl, a, per_user |  |
| joy_response_look | 0 | cl, a, per_user |  |
| joy_response_move | 9 | cl, a, per_user |  |
| joy_side_sensitivity | 1 | cl, a, per_user |  |
| joy_sidesensitivity | 1 | cl, a |  |
| joy_wingmanwarrior_centerhack | false | a | Wingman warrior centering hack. |
| joy_wingmanwarrior_turnhack | false | a | Wingman warrior hack related to turn axes. |
| joy_yaw_sensitivity | 3 | cl, a, per_user |  |
| joy_yawsensitivity | -1 | cl, a, per_user |  |
| joystick | false | cl, a | True if the joystick is enabled, false otherwise. |
| jpeg_screenshot | cmd |  | Take a jpeg screenshot |
| key_findbinding | cmd |  | Find key bound to specified command string. |
| key_listboundkeys | cmd |  | List bound keys with bindings. |
| key_updatelayout | cmd |  | Updates game keyboard layout to current windows keyboard setting. |
| kick | cmd | norecord | Kick a player by name. |
| kickid | cmd | norecord | Kick a player by userid or uniqueid, with a message. |
| kickid_hltv | cmd | norecord | Kick a player by userid or uniqueid, with a message. |
| kill | cmd | sv, cheat | Kills the player with generic damage |
| killvector | cmd | sv, cheat | Kills a player applying force. Usage |
| labelled_debug_helper_arc_segments | 20 | sv, cl, rep, cheat |  |
| labelled_debug_helper_enabled | true | sv, cl, rep, cheat |  |
| labelled_debug_helper_scale | 1 | sv, cl, rep, cheat |  |
| labelled_debug_helper_show_position | false | sv, cl, rep, cheat |  |
| labelled_debug_helper_show_text | true | sv, cl, rep, cheat |  |
| labelled_debug_helper_skeleton_show_bone_names | true | sv, cl, rep, cheat |  |
| lastinv | cmd | cl, server_can_execute |  |
| launch_warmup_map | cmd | cl, norecord, clientcmd_can_execute | Launches warmup map |
| lb_shadow_map_culling | true | cheat |  |
| lb_show_light_fog_clipmap_cb_cost | false | cheat | Show cost of lights in fog clipmap constant buffer. yellow = 1 cost, red = 6 cost |
| lightquery_debug_direct_lighting | true | sv, cl, rep, cheat |  |
| lightquery_debug_indirect_lighting | true | sv, cl, rep, cheat |  |
| lightquery_debug_indirect_lighting_fast | 0 | sv, cl, rep, cheat | 0 = standard sampling, 1 = fast sampling, 2 = ultra-fast sampling |
| listdemo | cmd |  | List demo file contents. |
| listid | cmd |  | Lists banned users. |
| listip | cmd |  | List IP addresses on the ban list. |
| listissues | cmd | sv | List all the issues that can be voted on. |
| listRecentNPCSpeech | cmd | sv, norecord | Displays a list of the last 5 lines of speech from NPCs. |
| load | cmd | norecord, vconsole_fuzzy | Usage |
| lobby_default_privacy_bits2 | 0 | cl, a, release | Lobby default permissions (0 |
| localization_quest_item_string_printout | cmd | cl | localization_quest_item_string_printout |
| lockMoveControllerRet | false | cl, a |  |
| log | cmd |  | Enables logging to file, console, and udp < on | off >. |
| log_color | cmd | norecord | Set the color of a logging channel. |
| log_dumpchannels | cmd | norecord | Dumps information about all logging channels. |
| log_flags | cmd | norecord | Set the flags on a logging channel. |
| log_level | cmd | norecord | Set the spew level of a logging channel. |
| log_verbosity | cmd | norecord | Set the verbosity of a logging channel. |
| logic_npc_counter_debug | false | sv, rep, cheat |  |
| +lookatweapon | cmd | cl |  |
| loop_dump | cmd |  | Print the listeners of the current loop mode |
| lrucache_flush | cmd |  | Flushes the specified cache |
| lrucache_reset_stats | cmd |  | Resets stats for the specified CUtlLRUCaches (or all if none specified) |
| lrucache_set_size | cmd |  | Sets the specified cache to the specified size |
| lrucache_stats | cmd |  | Spews information about all CUtlLRUCaches |
| lua_report_memory | cmd |  |  |
| m_pitch | 0.022 | cl, a, per_user | Mouse pitch factor. |
| m_yaw | 0.022 | cl, a, per_user | Mouse yaw factor. |
| map | cmd | vconsole_fuzzy, vconsole_set_focus | map <mapname> |
| map_enable_background_maps | cmd | cl, cheat | Enables/disables portrait background maps |
| map_setbombradius | cmd | sv, cheat | Sets the bomb radius for the map. |
| map_showbombradius | cmd | sv, cheat | Shows bomb radius from the center of each bomb site and planted bomb. |
| map_showspawnpoints | cmd | sv | Shows player spawn points (red=invalid). Optionally pass in the duration. |
| mapgroup | cmd | sv, norecord | Specify a map group |
| mapoverview_allow_client_draw | false | cl, release | Allow a client to draw on the map overview |
| mapoverview_icon_scale | 1 | cl, a, release | Sets the icon scale multiplier for the overview map. Valid values are 0.5 to 3.0. |
| maps | cmd |  | Displays list of maps. |
| markup_group_ent_bbox | cmd | sv, cheat | markup_group_ent_bbox <markup_group name> -> toggle ent_bbox for all members of the named markup group |
| markup_group_ent_text | cmd | sv, cheat | markup_group_ent_text <markup_group name> -> toggle ent_text for all members of the named markup group |
| markup_group_spew | cmd | sv, cheat | Spew all current markup groups and their members |
| mat_clearshadercache | cmd |  | Clears the shader cache used for dynamic shader compile. |
| mat_colcorrection_forceentitiesclientside | false | cl, cheat | Forces color correction entities to be updated on the client |
| mat_disable_dynamic_shader_compile | cmd |  | Reloads all shaders from vcs files until the next time mat_reloadshaders is called |
| mat_disable_normal_mapping | false | cl, cheat |  |
| mat_fullbright | 0 | cheat |  |
| mat_lpv_luxels | false | cheat |  |
| mat_luxels | false | cheat |  |
| mat_max_lighting_complexity | 8 | cheat |  |
| mat_overdraw | 0 | cheat | Visualize overdraw |
| mat_overdraw_color | 0.075000 0.150000 0.300000 | cheat |  |
| mat_print_dead_materials | cmd |  | Print loaded materials that have no valid layers due to not supporting any of the modes in gameinfo.gi. |
| mat_print_error_materials | cmd |  | Print loaded materials that are using the error shader or material. |
| mat_print_expensive_materials | cmd |  | Print materials sorted by cost heuristic |
| mat_print_material_info | cmd |  | Print info about a specific material |
| mat_print_materials | cmd |  | Print loaded materials. Takes an optional substring as an argument. |
| mat_print_materials_last_frame | cmd |  | Print materials used last frame |
| mat_print_materials_unused | cmd |  | Print materials that have never been used |
| mat_print_modes | cmd |  | Print supported rendering modes. |
| mat_print_shader_info | cmd |  | Print detailed info about a single shader. Takes a shader name (hero.vfx) as an argument. |
| mat_print_shader_quality | cmd |  | Print current shader quality setting |
| mat_print_shaders | cmd |  | Print loaded shaders. Takes a substring as an argument. |
| mat_print_textures | cmd |  | Print loaded textures in alphabetical order. Takes an optional substring as an argument. |
| mat_print_textures_size | cmd |  | Print loaded textures in ascending size order. Takes an optional substring as an argument. |
| mat_print_textures_size_in_memory | cmd |  | Print loaded textures in ascending size order as they are in memory. Takes an optional substring as an argument. |
| mat_reinitmaterials | cmd |  | Reinitializes all loaded materials, reloading their shaders. |
| mat_reloadmaterials | cmd |  | Reloads all materials. Takes an optional substring as an argument. |
| mat_reloadshaders | cmd |  | Reloads all shaders. Takes optional substrings of shader names to recompile as arguments. |
| mat_reset_material_costs | cmd |  | Reset material cost heuristic |
| mat_set_shader_quality | cmd |  | Force shader quality setting (valid values are 0 or 1) |
| mat_shading_complexity | false | cheat | Visualize shading complexity |
| mat_shading_complexity_color | 1.000000 0.500000 0.250000 | cheat |  |
| mat_shading_complexity_max_instruction_count | 1024 | cheat |  |
| mat_shading_complexity_max_register_count | 128 | cheat |  |
| mat_tonemap_bloom_scale | -1 | cheat |  |
| mat_tonemap_bloom_start_value | -1 | cheat |  |
| mat_tonemap_csgo_bloom_scale | -1 | cheat |  |
| mat_tonemap_csgo_bloom_start_value | -1 | cheat |  |
| mat_tonemap_csgo_force_accelerate_exposure_down | -1 | cheat |  |
| mat_tonemap_csgo_force_average_lum_min | -1 | cheat | Override. Old default was 3.0 |
| mat_tonemap_csgo_force_max | -1 | cheat |  |
| mat_tonemap_csgo_force_min | -1 | cheat |  |
| mat_tonemap_csgo_force_percent_bright_pixels | -1 | cheat | Override. Old value was 1.0 |
| mat_tonemap_csgo_force_percent_target | -1 | cheat | Override. Old default was 45. |
| mat_tonemap_csgo_force_rate | -1 | cheat |  |
| mat_tonemap_csgo_force_scale | 0 | cheat |  |
| mat_tonemap_csgo_force_use_alpha | -1 | cheat |  |
| mat_tonemap_csgo_uncap_exposure | false | cheat |  |
| mat_tonemap_force_accelerate_exposure_down | -1 | cheat |  |
| mat_tonemap_force_average_lum_min | -1 | cheat | Override. Old default was 3.0 |
| mat_tonemap_force_log_lum_max | -1 | cheat |  |
| mat_tonemap_force_log_lum_min | -1 | cheat |  |
| mat_tonemap_force_max | -1 | cheat |  |
| mat_tonemap_force_min | -1 | cheat |  |
| mat_tonemap_force_percent_bright_pixels | -1 | cheat | Override. Old value was 1.0 |
| mat_tonemap_force_percent_target | -1 | cheat | Override. Old default was 45. |
| mat_tonemap_force_rate | -1 | cheat |  |
| mat_tonemap_force_scale | 0 | cheat |  |
| mat_tonemap_force_use_alpha | -1 | cheat |  |
| mat_tonemap_uncap_exposure | 0 | cheat |  |
| mat_wireframe | 0 | cheat | 0=Off, 1=Surface Wireframe, 2=Transparent Wireframe |
| mem_compact | cmd |  | Compacts the heap |
| mem_dump | cmd |  | Dump memory stats to text file or <stdout>. |
| mem_test | cmd |  |  |
| memory | cmd |  | Print memory stats. |
| menuselect | cmd | cl, clientcmd_can_execute | menuselect |
| mesh_calculate_curvature_smooth_invert | false | sv, cl, rep, cheat |  |
| mesh_calculate_curvature_smooth_pass_count | 3 | sv, cl, rep, cheat |  |
| mesh_calculate_curvature_smooth_weight | 1 | sv, cl, rep, cheat |  |
| mm_csgo_community_search_players_min | 3 | a, release | When performing CSGO community matchmaking look for servers with at least so many human players |
| mm_datacenter_debugprint | cmd |  | Shows information retrieved from data center |
| mm_debugprint | cmd |  | Show debug information about current matchmaking session |
| mm_dedicated_force_servers | 0 | release | Comma delimited list of ip |
| mm_dedicated_search_maxping | 150 | a | Longest preferred ping to dedicated servers for games |
| mm_queue_show_stats | cmd | cl, clientcmd_can_execute | Display global server stats |
| mm_server_search_lan_ports | 27015,27016,27017,27018,27019,27020 | a, release | Ports to scan during LAN games discovery. Also used to discover and correctly connect to dedicated LAN servers behind NATs. |
| mm_session_search_qos_timeout | 15 | release |  |
| mm_session_sys_kick_ban_duration | 180 | release |  |
| mm_session_sys_pkey | 0 | release |  |
| mobile_fps_increase_during_charging | false | a | MOBILE_FPS_CONTROL |
| mobile_fps_increase_during_touch | true | a | MOBILE_FPS_CONTROL |
| mobile_fps_limit | 30 | a | MOBILE_FPS_CONTROL |
| model_default_preview_sequence_name | 0 | sv, cl, a, rep |  |
| model_dump_convert_info | cmd | sv, cl, linked | Print model load-time conversion info |
| molotov_throw_detonate_time | 2 | sv, cl, rep, release |  |
| motdfile | motd.txt | sv, release | The MOTD file to load. |
| mouse_inverty | false | cl, a |  |
| movie_fixwave | cmd |  | Fixup corrupted .wav file if engine crashed during startmovie/endmovie, etc. |
| mp_afterroundmoney | 0 | sv, cl, rep, release | amount of money awared to every player after each round |
| mp_anyone_can_pickup_c4 | false | sv, cl, rep, release | If set, everyone can pick up the c4, not just Ts. |
| mp_autokick | true | sv, rep, release | Kick idle/team-killing/team-damaging players |
| mp_autoteambalance | true | sv, nf, release |  |
| mp_backup_restore_list_files | cmd | sv, release | Lists recent backup round files matching the prefix, most recent files first, accepts a numeric parameter to limit the number of files displayed |
| mp_backup_restore_load_autopause | true | sv, release | Whether to automatically pause the match after restoring round data from backup |
| mp_backup_restore_load_file | cmd | sv, release | Loads player cash, KDA, scores and team scores; resets to the next round after the backup |
| mp_backup_round_auto | true | sv, release | If enabled will keep in-memory backups to handle reconnecting players even if the backup files aren't written to disk |
| mp_backup_round_file | backup | sv, release | If set then server will save all played rounds information to files filename_date_time_team1_team2_mapname_roundnum_score1_score2.txt |
| mp_backup_round_file_last | backup_round00.txt | sv, release | Every time a backup file is written the value of this convar gets updated to hold the name of the backup file. |
| mp_backup_round_file_pattern | %prefix%_round%round%.txt | sv, release | If set then server will save all played rounds information to files named by this pattern, e.g.'%prefix%_%date%_%time%_%team1%_%team2%_%map%_round%round%_score_%score1%_%score2%.txt' |
| mp_bot_ai_bt | 0 | sv, release | Use the specified behavior tree file to drive the bot behavior. |
| mp_bot_ai_bt_clear_cache | cmd | sv, release | Clears the cache for behavior tree files. |
| mp_buy_allow_grenades | true | sv, cl, rep, release | Whether players can purchase grenades from the buy menu or not. |
| mp_buy_allow_guns | 255 | sv, cl, rep, release | Whether players can purchase guns |
| mp_buy_anywhere | 0 | sv, cl, nf, rep, release | When set, players can buy anywhere, not only in buyzones. 0 = default. 1 = both teams. 2 = Terrorists. 3 = Counter-Terrorists. |
| mp_buy_during_immunity | 0 | sv, cl, nf, rep, release | When set, players can buy when immune, ignoring buytime. 0 = default. 1 = both teams. 2 = Terrorists. 3 = Counter-Terrorists. |
| mp_buytime | 20 | sv, cl, rep, release | How many seconds after round start players can buy items for. |
| mp_c4_cannot_be_defused | false | sv, cl, rep, release | If set, the planted c4 cannot be defused. |
| mp_c4timer | 40 | sv, cl, nf, rep, release | how long from when the C4 is armed until it blows |
| mp_competitive_endofmatch_extra_time | 15 | sv, release | After a competitive match finishes rematch voting extra time is given for rankings. |
| mp_consecutive_loss_aversion | 1 | sv, rep, release | How loss streak is affected with round win |
| mp_consecutive_loss_max | 4 | sv, rep, release |  |
| mp_coop_force_join_ct | false | sv, cl, rep, release | If set, real players will auto join CT on join. |
| mp_coopmission_bot_difficulty_offset | 0 | sv, rep, release | The difficulty offset modifier for bots during coop missions. |
| mp_coopmission_mission_number | 0 | sv, cl, rep, release | Which mission the map should run after it loads. |
| mp_coopterrorhunt_kill_add_time | 10 | sv, cl, rep, release | The number of seconds added to the clock when players get a kill. |
| mp_coopterrorhunt_num_enemies | 20 | sv, cl, rep, release | The number of enemies CTs have to hunt and kill. |
| mp_ct_default_grenades | 0 | sv, cl, rep, release | The default grenades that the CTs will spawn with.  To give multiple grenades, separate each weapon class with a space like this |
| mp_ct_default_melee | weapon_knife | sv, cl, rep, release | The default melee weapon that the CTs will spawn with.  Even if this is blank, a knife will be given. To give a taser, it should look like this |
| mp_ct_default_primary | 0 | sv, cl, rep, release | The default primary (rifle) weapon that the CTs will spawn with |
| mp_ct_default_secondary | weapon_hkp2000 | sv, cl, rep, release | The default secondary (pistol) weapon that the CTs will spawn with |
| mp_damage_headshot_only | false | sv, rep, release | Determines whether non-headshot hits do any damage. |
| mp_damage_scale_ct_body | 1 | sv, rep, release | Scales the damage a CT player takes by this much when they take damage in the body. (1 == 100%, 0.5 == 50%) |
| mp_damage_scale_ct_head | 1 | sv, rep, release | Scales the damage a CT player takes by this much when they take damage in the head (1 == 100%, 0.5 == 50%).  REMEMBER! headshots do 4x the damage of the body before this scaler is applied. |
| mp_damage_scale_t_body | 1 | sv, rep, release | Scales the damage a T player takes by this much when they take damage in the body. (1 == 100%, 0.5 == 50%) |
| mp_damage_scale_t_head | 1 | sv, rep, release | Scales the damage a T player takes by this much when they take damage in the head (1 == 100%, 0.5 == 50%).  REMEMBER! headshots do 4x the damage of the body before this scaler is applied. |
| mp_damage_vampiric_amount | 0 | sv, rep, release | If Set to non-0, will determine the fraction of damage dealt that will be given to attacker. |
| mp_death_drop_breachcharge | true | sv, cl, rep, release | Drop breachcharge on player death |
| mp_death_drop_c4 | true | sv, cl, rep, release | Whether c4 is droppable |
| mp_death_drop_defuser | true | sv, cl, rep, release | Drop defuser on player death |
| mp_death_drop_grenade | 2 | sv, cl, rep, release | Which grenade to drop on player death |
| mp_death_drop_gun | 1 | sv, cl, rep, release | Which gun to drop on player death |
| mp_death_drop_healthshot | true | sv, cl, rep, release | Drop healthshot on player death |
| mp_death_drop_taser | true | sv, cl, rep, release | Drop taser on player death |
| mp_deathcam_skippable | true | sv, rep, release | Determines whether a player can early-out of the deathcam. |
| mp_debug_timeouts | cmd | sv | Prints time outs to the console for debugging |
| mp_default_team_winner_no_objective | -1 | sv, cl, rep, release | If the map doesn't define an objective (bomb, hostage, etc), the value of this convar will declare the winner when the time runs out in the round. |
| mp_defuser_allocation | 0 | sv, cl, rep, release | How to allocate defusers to CTs at start or round |
| mp_disable_autokick | cmd | sv | Prevents a userid from being auto-kicked |
| mp_disconnect_kills_bots | false | sv, release | When a bot disconnects, kill them first.  Requires mp_disconnect_kills_players. |
| mp_disconnect_kills_players | true | sv, release | When a player disconnects, kill them first (triggering item drops, stats, etc.) |
| mp_display_kill_assists | true | sv, cl, rep, release | Whether to display and score player assists |
| mp_dm_bonus_length_max | 30 | sv, rep, release | Maximum time the bonus time will last (in seconds) |
| mp_dm_bonus_length_min | 30 | sv, rep, release | Minimum time the bonus time will last (in seconds) |
| mp_dm_bonus_percent | 50 | sv, cl, rep, release | Percent of points additionally awarded when someone gets a kill with the bonus weapon during the bonus period. |
| mp_dm_bonus_respawn | false | sv, cl, rep, release | When attempting to get the bonus weapon in deathmatch, whether we should respawn you with it or just give it to you directly |
| mp_dm_bonusweapon_dogtags | 0 | sv, cl, rep, release | Additional dogtags to drop when making a kill with the bonus weapon |
| mp_dm_dogtag_score | 0 | sv, cl, rep, release | Points to award for picking up a dogtag in deathmatch. |
| mp_dm_kill_base_score | 10 | sv, cl, rep, release | Number of base points to award for a kill in deathmatch.  Cheaper weapons award 1 or 2 additional points. |
| mp_dm_teammode | 0 | sv, cl, rep, release | In deathmatch, enables team DM visuals & scoring (0 |
| mp_dm_teammode_bonus_score | 1 | sv, cl, rep, release | Team deathmatch victory points to award for kill with bonus weapon |
| mp_dm_teammode_dogtag_score | 0 | sv, cl, rep, release | Team deathmatch victory points to award for collecting enemy dogtags |
| mp_dm_teammode_kill_score | 1 | sv, cl, rep, release | Team deathmatch victory points to award for enemy kill |
| mp_dm_time_between_bonus_max | 40 | sv, rep, release | Maximum time a bonus time will start after the round start or after the last bonus (in seconds) |
| mp_dm_time_between_bonus_min | 30 | sv, rep, release | Minimum time a bonus time will start after the round start or after the last bonus (in seconds) |
| mp_dogtag_despawn_on_killer_death | true | sv, rep, release | Whether dogtags should despawn when their killer dies |
| mp_dogtag_despawn_time | 120 | sv, rep, release | How many seconds dogtags should stay around before despawning automatically (0 = infinite) |
| mp_dogtag_pickup_rule | 0 | sv, rep, release | Who is eligible to pick up a dogtag (0 = killer only, 1 = killer's team, 2 = victim's team, 3 = killer & victim's team, 4 = anyone) |
| mp_dronegun_stop | false | sv, cl, rep, release | if non-zero, stops AI on all droneguns. |
| mp_drop_grenade_enable | true | sv, release | Allows players to drop grenades. |
| mp_drop_knife_enable | false | sv, release | Allows players to drop knives. |
| mp_dump_timers | cmd | sv | Prints round timers to the console for debugging |
| mp_economy_reset_rounds | 0 | sv, cl, rep, release | Reset all player money every N rounds (0 for never) |
| mp_endmatch_votenextleveltime | 20 | sv, release | If mp_endmatch_votenextmap is set, players have this much time to vote on the next map at match end. |
| mp_endmatch_votenextmap | true | sv, cl, rep, release | Whether or not players vote for the next map at the end of the match when the final scoreboard comes up |
| mp_endmatch_votenextmap_keepcurrent | true | sv, cl, rep, release | If set, keeps the current map in the list of voting options.  If not set, the current map will not appear in the list of voting options. |
| mp_endmatch_votenextmap_wargames_modes | armsrace | sv, release | Modes available for endmatch voting during War Games. Separate names with spaces. |
| mp_endmatch_votenextmap_wargames_nummaps | 3 | sv, release | Maximum number of maps to include in endmatch voting during War Games |
| mp_endmatch_votenextmap_wargames_nummodes | 1 | sv, release | Maximum number of other War Games to include in endmatch voting during War Games |
| mp_endwarmup_player_count | 0 | sv, cl, rep, release | Number of players required to be connected to end warmup early. 0 to require maximum players for mode. |
| mp_equipment_reset_rounds | 0 | sv, cl, rep, release | Reset all player equipment every N rounds (0 for never) |
| mp_fists_replace_melee | true | sv, release | If enabled then when melee weapon is dropped player will have fists, when melee weapon is picked up then fists are unavailable |
| mp_footsteps_serverside | true | sv, release | Makes the server always play footstep sounds. Clients never calculate footstep sounds locally, instead relying on the server. |
| mp_force_pick_time | 15 | sv, cl, rep, release | The amount of time a player has on the team screen to make a selection before being auto-teamed |
| mp_forcecamera | 1 | sv, cl, rep, release | Restricts spectator modes for dead players |
| mp_fraglimit | 0 | sv, nf, release |  |
| mp_free_armor | 0 | sv, cl, rep, release | Determines whether kevlar (1+) and/or helmet (2+) are given automatically. |
| mp_freezetime | 15 | sv, nf, rep, release | how many seconds to keep players frozen when the round starts |
| mp_friendlyfire | true | sv, cl, nf, rep, release | Allows team members to injure other members of their team |
| mp_ggprogressive_healthshot_killcount | 3 | sv, cl, rep, release | Grant healthshots in arms race after n kills |
| mp_ggprogressive_random_weapon_kills_needed | 2 | sv, cl, rep, release | If mp_ggprogressive_use_random_weapons is set, this is the number of kills needed with each weapon |
| mp_ggprogressive_round_restart_delay | 15 | sv, cl, rep, release | Number of seconds to delay before restarting a round after a win in gungame progessive |
| mp_ggprogressive_use_random_weapons | true | sv, cl, rep, release | If set, selects random weapons from set categories for the progression order |
| mp_ggtr_always_upgrade | false | sv, cl, rep, release | Award this many upgrade points every round in demolition mode |
| mp_ggtr_bomb_defuse_bonus | 1 | sv, cl, rep, release | Number of bonus upgrades to award the CTs when they defuse a gun game bomb |
| mp_ggtr_bomb_detonation_bonus | 1 | sv, cl, rep, release | Number of bonus upgrades to award the Ts when they detonate a gun game bomb |
| mp_ggtr_bomb_pts_for_flash | 4 | sv, cl, rep, release | Kill points required in a round to get a bonus flash grenade |
| mp_ggtr_bomb_pts_for_he | 3 | sv, cl, rep, release | Kill points required in a round to get a bonus HE grenade |
| mp_ggtr_bomb_pts_for_molotov | 5 | sv, cl, rep, release | Kill points required in a round to get a bonus molotov cocktail |
| mp_ggtr_bomb_pts_for_upgrade | 2 | sv, cl, rep, release | Kill points required to upgrade a player's weapon |
| mp_ggtr_bomb_respawn_delay | 0 | sv, cl, rep, release | Number of seconds to delay before making the bomb available to a respawner in gun game |
| mp_ggtr_end_round_kill_bonus | 1 | sv, cl, rep, release | Number of bonus points awarded in Demolition Mode when knife kill ends round |
| mp_ggtr_last_weapon_kill_ends_half | false | sv, cl, rep, release | End the half and give a team round point when a player makes a kill using the final weapon |
| mp_ggtr_num_rounds_autoprogress | 3 | sv, cl, rep, release | Upgrade the player's weapon after this number of rounds without upgrading |
| mp_give_player_c4 | true | sv, cl, rep, release | Whether this map should spawn a c4 bomb for a player or not. |
| mp_global_damage_per_second | 0 | sv, rep, release | If above 0, deal non-lethal damage to players over time. |
| mp_guardian_add_bounds_pt | cmd | sv | mp_guardian_add_bounds_pt |
| mp_guardian_add_player_spawn_pt | cmd | sv | mp_guardian_add_player_spawn_pt |
| mp_guardian_ai_bt_difficulty_adjust_wave_interval | 1 | sv, rep, release | Adjust the guardian bots' difficulty every nth guardian wave when using behavior trees. |
| mp_guardian_ai_bt_difficulty_cap_beginning_round | 2 | sv, rep, release | Starting this round a difficulty cap will be applied to the bots. |
| mp_guardian_ai_bt_difficulty_initial_value | 2 | sv, rep, release | Starting difficulty level for the gardian bots. |
| mp_guardian_ai_bt_difficulty_max_next_level_bots | 3 | sv, rep, release | How many bots to increase difficulty per wave - this many easier bots will get harder. |
| mp_guardian_bomb_plant_add_bounds_pt | cmd | sv | mp_guardian_bomb_plant_add_bounds_pt |
| mp_guardian_bomb_plant_clear_all_bounds | cmd | sv | mp_guardian_bomb_plant_clear_all_bounds |
| mp_guardian_bomb_plant_custom_x_mark_location | 0 | sv, cl, rep, release | x,y,z to display an X for the bomb plant in guardian missions with custom bomb plant boundaries. |
| mp_guardian_bomb_plant_emit_bounds_config | cmd | sv | mp_guardian_bomb_plant_emit_bounds_config |
| mp_guardian_bomb_plant_new_bounds | cmd | sv | mp_guardian_bomb_plant_new_bounds |
| mp_guardian_bot_money_per_wave | 800 | sv, rep, release | The amount of money bots get time each wave the players complete.  This # is absolute and not additive, the money is set to (this)x(wave#) for each bot on each wave. |
| mp_guardian_clear_all_bounds | cmd | sv | mp_guardian_clear_all_bounds |
| mp_guardian_clear_all_player_spawns | cmd | sv | mp_guardian_clear_all_player_spawns |
| mp_guardian_emit_bounds_config | cmd | sv | mp_guardian_emit_bounds_config |
| mp_guardian_force_collect_hostages_timeout | 50 | sv, release | Force bots to collect hostages after this amount of time if no enemy has been seen. |
| mp_guardian_give_random_grenades_to_bots | true | sv, release | If set guardian bots will be given grenades at the beginning of the wave. |
| mp_guardian_loc_string_hud | #guardian_mission_type_kills | sv, cl, rep, release | Loc string token to use on hud for this mission, otherwise default to kills with weapon. |
| mp_guardian_loc_weapon | 0 | sv, cl, rep, release | Override to weapon dialog var applied to UI |
| mp_guardian_new_bounds | cmd | sv | mp_guardian_new_bounds |
| mp_guardian_player_dist_max | 2000 | sv, rep, release | The maximum distance a player is allowed to get from the bombsite before they're killed. |
| mp_guardian_player_dist_min | 1300 | sv, rep, release | The distance at which we start to warn a player when they are too far from the guarded bombsite. |
| mp_guardian_shoot_point | cmd | sv | mp_guardian_shoot_point |
| mp_guardian_special_kills_needed | 10 | sv, rep, release | The number of kills needed with a specific weapon. |
| mp_guardian_special_weapon_needed | awp | sv, rep, release | The weapon that needs to be used to increment the kills needed to complete the mission. |
| mp_guardian_target_site | -1 | sv, release | If set to the index of a bombsite, will cause random spawns to be only created near that site. |
| mp_halftime | true | sv, cl, rep, release | Determines whether the match switches sides in a halftime event. |
| mp_halftime_duration | 15 | sv, cl, rep, release | Target number of seconds that halftime lasts; shortened if team intros are active |
| mp_halftime_pausematch | 0 | sv, cl, rep, release | Set to 1 to pause match after halftime countdown elapses. Match must be resumed by vote or admin. |
| mp_halftime_pausetimer | 0 | sv, cl, rep, release | Set to 1 to stay in halftime indefinitely. Set to 0 to resume the timer. |
| mp_heavyassaultsuit_aimpunch | true | sv, cl, rep, release | How much EXTRA aim punch will happen when a player wearing the assault suit gets when shot |
| mp_heavyassaultsuit_cooldown | 5 | sv, cl, rep, release | Determines cooldown of purchase. |
| mp_heavyassaultsuit_deploy_timescale | 0.8 | sv, cl, rep, release | How fast a player wearing the heavy assault suit will draw their weapon (1.0 = normal speed, 0.5 = half speed) |
| mp_heavyassaultsuit_speed | 130 | sv, cl, rep, release | The max speed of a player when they are wearing the heavy assault suit |
| mp_heavybot_damage_reduction_scale | 1 | sv, cl, rep, release | How much damage should scale when the player wearing the heavy assault suit is shot (1.0 = no change, 0.5 = half damage) |
| mp_hostages_max | 2 | sv, rep, release | Maximum number of hostages to spawn. |
| mp_hostages_rescuetime | 1 | sv, cl, rep, release | Additional time added to round time if a hostage is reached by a CT. |
| mp_hostages_run_speed_modifier | 1 | sv, rep, release | Default is 1.0, slow down hostages by setting this to < 1.0. |
| mp_hostages_spawn_farthest | false | sv, rep, release | When enabled will consistently force the farthest hostages to spawn. |
| mp_hostages_spawn_force_positions | 0 | sv, rep, release | Comma separated list of zero based indices to force spawn positions, e.g. '0,2' or '1,6' |
| mp_hostages_spawn_force_positions_xyz | 0 | sv, rep, release | Comma separated list of xyz locations to force spawn positions, e.g. 'x1 y1 z1,x2 y2 z2' |
| mp_hostages_spawn_same_every_round | true | sv, rep, release | 0 = spawn hostages randomly every round, 1 = same spawns for entire match. |
| mp_hostages_takedamage | false | sv, cl, rep, release | Whether or not hostages can be hurt. |
| mp_humanteam | any | sv, rep, release | Restricts human players to a single team {any, CT, T} |
| mp_ignore_round_win_conditions | false | sv, rep, release | Ignore conditions which would end the current round |
| mp_items_prohibited | 0 | sv, cl, rep, release | Set this convar to a comma-delimited list of definition indices of weapons that should be prohibited from use. |
| mp_join_grace_time | 0 | sv, cl, rep, release | Number of seconds after round start to allow a player to join a game |
| mp_limitteams | 2 | sv, nf, rep, release | Max # of players 1 team can have over another (0 disables check) |
| mp_logdetail | 0 | sv, release | Logs attacks.  Values are |
| mp_logdetail_items | false | sv, release | Logs a line any time a player acquires or loses an item. |
| mp_logdistance_2d | 250 | sv, release | Enables distance logging every so many units |
| mp_logdistance_sec | 15 | sv, release | Enables distance logging every so many seconds |
| mp_logloadouts | true | sv, release | Enables distance logging with full loadouts |
| mp_logmoney | false | sv, release | Enables money logging.  Values are |
| mp_match_can_clinch | true | sv, cl, rep, release | Can a team clinch and end the match by being so far ahead that the other team has no way to catching up? |
| mp_match_end_changelevel | false | sv, cl, rep, release | At the end of the match, perform a changelevel even if next map is the same |
| mp_match_end_restart | false | sv, cl, rep, release | At the end of the match, perform a restart instead of loading a new map |
| mp_match_restart_delay | 25 | sv, cl, rep, release | Time (in seconds) until a match restarts. |
| mp_max_armor | 2 | sv, cl, rep, release | Determines the highest level of armor allowed to be purchased. (0) None, (1) Kevlar, (2) Helmet |
| mp_maxmoney | 16000 | sv, cl, rep, release | maximum amount of money allowed in a player's account |
| mp_maxrounds | 30 | sv, cl, nf, rep, release | max number of rounds to play before server changes maps |
| mp_min_halftime_duration | 8.5 | sv, cl, rep, release | Minimum number of seconds that halftime lasts even if team intros are active |
| mp_only_cts_rescue_hostages | true | sv, rep, release |  |
| mp_overtime_enable | false | sv, cl, rep, release | If a match ends in a tie, use overtime rules to determine winner |
| mp_overtime_halftime_pausetimer | 0 | sv, cl, rep, release | If set to 1 will set mp_halftime_pausetimer to 1 before every half of overtime. Set mp_halftime_pausetimer to 0 to resume the timer. |
| mp_overtime_maxrounds | 6 | sv, cl, rep, release | When overtime is enabled play additional rounds to determine winner |
| mp_overtime_startmoney | 10000 | sv, cl, rep, release | Money assigned to all players at start of every overtime half |
| mp_pause_match | cmd | sv | Pause the match in the next freeze time |
| mp_plant_c4_anywhere | false | sv, cl, rep, release |  |
| mp_playercashawards | true | sv, cl, rep, release | Players can earn money by performing in-game actions |
| mp_playerid | 0 | sv, cl, rep, release | Controls what information player see in the status bar |
| mp_playerid_delay | 0.4 | sv, cl, rep, release | Number of seconds to delay showing information in the status bar |
| mp_playerid_hold | 0.1 | sv, cl, rep, release | Number of seconds to keep showing old information in the status bar |
| mp_randomspawn | 0 | sv, cl, rep, release | Determines whether players are to spawn. 0 = default; 1 = both teams; 2 = Terrorists; 3 = CTs. |
| mp_randomspawn_dist | 0 | sv, cl, rep, release | If using mp_randomspawn, determines whether to test distance when selecting this spot. |
| mp_randomspawn_los | false | sv, cl, rep, release | If using mp_randomspawn, determines whether to test Line of Sight when spawning. |
| mp_require_gun_use_to_acquire | false | sv, release | Whether guns must be +used to acquire or default is touch-to-pickup |
| mp_respawn_immunitytime | -1 | sv, cl, rep, release | How many seconds after respawn immunity lasts. Set to negative value to disable warmup immunity. |
| mp_respawn_on_death_ct | false | sv, cl, rep, release | When set to 1, counter-terrorists will respawn after dying. |
| mp_respawn_on_death_t | false | sv, cl, rep, release | When set to 1, terrorists will respawn after dying. |
| mp_respawnwavetime_ct | 10 | sv, cl, rep, release | Time between respawn waves for CTs. |
| mp_respawnwavetime_t | 10 | sv, cl, rep, release | Time between respawn waves for Terrorists. |
| mp_restartgame | 0 | sv, release | If non-zero, game will restart in the specified number of seconds |
| mp_retake_ct_count | 4 | sv, cl, rep, release | Number of CT's when playing retakes. |
| mp_retake_ct_loadout_bonus_card | #GameUI_Retake_Card_TheAWPortunity,1,1,rifle4 | sv, cl, rep, release | CT bonus card for full buy round when playing bomb site retake. |
| mp_retake_ct_loadout_bonus_card_availability | 1,2 | sv, cl, rep, release | CT bonus card availability pattern for full buy round when playing bomb site retake. |
| mp_retake_ct_loadout_default_pistol_round | 1|3;#GameUI_Retake_Card_4v3,0,0,secondary0|1;#GameUI_Retake_Card_FlashOut,0,0,secondary0,grenade2;#GameUI_Retake_Card_HideAndPeek,0,0,secondary0,grenade4 | sv, cl, rep, release | CT Loadouts for default pistol round when playing bomb site retake. |
| mp_retake_ct_loadout_enemy_card | #GameUI_Retake_Card_BehindEnemyLines,1,1,rifle1,grenade2 | sv, cl, rep, release | CT enemy card for full buy round when playing bomb site retake. |
| mp_retake_ct_loadout_full_buy_round | 4|2;#GameUI_Retake_Card_LightEmUp,1,1,rifle1,grenade2|2;#GameUI_Retake_Card_Kobe,1,1,rifle1,grenade3|1;#GameUI_Retake_Card_1g,1,1,rifle1,grenade0|1;#GameUI_Retake_Card_DisappearingAct,1,1,rifle1,grenade4|1;#GameUI_Retake_Card_EyesOnTarget,1,1,rifle3 | sv, cl, rep, release | CT Loadouts for full buy round when playing bomb site retake. |
| mp_retake_ct_loadout_light_buy_round | 3|2;#GameUI_Retake_Card_UmpInSmoke,1,1,smg2,grenade4|2;#GameUI_Retake_Card_FunNGun,1,1,smg0,grenade3|2;#GameUI_Retake_Card_Sharpshooter,1,1,rifle2,grenade2|2;#GameUI_Retake_Card_BurstBullpup,1,1,rifle0 | sv, cl, rep, release | CT Loadouts for force buy round when playing bomb site retake. |
| mp_retake_ct_loadout_upgraded_pistol_round | 2|2;#GameUI_Retake_Card_TakeFive,0,0,secondary3|2;#GameUI_Retake_Card_BlindFire,0,0,secondary2,grenade2|2;#GameUI_Retake_Card_OnlyTakesOne,0,0,secondary4|2;#GameUI_Retake_Card_SneakyBeakyLike,0,0,secondary2,grenade4 | sv, cl, rep, release | CT Loadouts for upgraded pistol round when playing bomb site retake. |
| mp_retake_max_consecutive_rounds_same_target_site | 2 | sv, cl, rep, release | Limit the number of consecutive rounds targeting the same site. |
| mp_retake_t_count | 3 | sv, cl, rep, release | Number of terrorists when playing retakes. |
| mp_retake_t_loadout_bonus_card | #GameUI_Retake_Card_TheAWPortunity,1,1,rifle4 | sv, cl, rep, release | T bonus card for full buy round when playing bomb site retake. |
| mp_retake_t_loadout_bonus_card_availability | 1,1,2 | sv, cl, rep, release | T bonus card availability pattern for full buy round when playing bomb site retake. |
| mp_retake_t_loadout_default_pistol_round | 0|3;#GameUI_Retake_Card_4BadGuysLeft,0,0,secondary0|1;#GameUI_Retake_Card_LookAway,0,0,secondary0,grenade2;#GameUI_Retake_Card_WhenThereIsSmoke,0,0,secondary0,grenade4 | sv, cl, rep, release | T Loadouts for default pistol round when playing bomb site retake. |
| mp_retake_t_loadout_enemy_card | #GameUI_Retake_Card_FindersKeepers,1,1,rifle1,grenade2 | sv, cl, rep, release | T enemy card for full buy round when playing bomb site retake. |
| mp_retake_t_loadout_full_buy_round | 0|2;#GameUI_Retake_Card_OlReliable,1,1,rifle1,grenade2|1;#GameUI_Retake_Card_SmokeShow,1,1,rifle1,grenade4|1;#GameUI_Retake_Card_HotShot,1,1,rifle1,grenade0|1;#GameUI_Retake_Card_EyeSpy,1,1,rifle3,grenade3 | sv, cl, rep, release | T Loadouts for full buy round when playing bomb site retake. |
| mp_retake_t_loadout_light_buy_round | 0|2;#GameUI_Retake_Card_BackInAFlash,1,1,smg2,grenade2|2;#GameUI_Retake_Card_AllIn,1,1,rifle0|1;#GameUI_Retake_Card_BoomBox,1,1,smg0,grenade3,grenade4|1;#GameUI_Retake_Card_SetThemFree,1,1,rifle2,grenade2 | sv, cl, rep, release | T Loadouts for force buy round when playing bomb site retake. |
| mp_retake_t_loadout_upgraded_pistol_round | 0|2;#GameUI_Retake_Card_BlindFire,0,0,secondary2,grenade2|2;#GameUI_Retake_Card_QueOta,0,0,secondary4|1;#GameUI_Retake_Card_SmokeScreen,0,0,secondary2,grenade4|1;#GameUI_Retake_Card_TecTecBoom,0,0,secondary3,grenade3 | sv, cl, rep, release | T Loadouts for upgraded pistol round when playing bomb site retake. |
| mp_round_restart_delay | 7 | sv, cl, rep, release | Number of seconds to delay before restarting a round after a win |
| mp_roundtime | 1.92 | sv, nf, rep, release | How many minutes each round takes. |
| mp_roundtime_defuse | 1.92 | sv, nf, rep, release | How many minutes each round of Bomb Defuse takes. If 0 then use mp_roundtime instead. |
| mp_roundtime_deployment | 5 | sv, release | How many minutes deployment for coop mission takes. |
| mp_roundtime_hostage | 1.92 | sv, nf, rep, release | How many minutes each round of Hostage Rescue takes. If 0 then use mp_roundtime instead. |
| mp_scrambleteams | cmd | sv | Scramble the teams and restart the game |
| mp_shield_speed_deployed | 170 | sv, cl, rep, release | The max speed of a player when they have a shield deployed |
| mp_shield_speed_holstered | 200 | sv, cl, rep, release | The max speed of a player when they have a shield holstered |
| mp_shorthanded_cash_bonus_ignore_kicked | true | sv, cl, rep, release | Determines whether kicked players are included in the assessment for short-handedness |
| mp_shorthanded_cash_bonus_round_delay | 2 | sv, cl, rep, release | number of previous rounds that a team needs to have been shorthanded before they are eligible for the short-handed bonus |
| mp_solid_teammates | 1 | sv, cl, rep, release | How solid are teammates |
| mp_spawnprotectiontime | 5 | sv, rep, release | Kick players who team-kill within this many seconds of a round restart. |
| mp_spec_swapplayersides | false | sv, cl, rep, release | Toggle set the player names and team names to the opposite side in which they are are on the spectator panel. |
| mp_spectators_max | 2 | sv, cl, rep, release | How many spectators are allowed in a match. |
| mp_starting_losses | 1 | sv, rep, release | Determines what the initial loss streak is. |
| mp_startmoney | 800 | sv, cl, rep, release | amount of money each player gets when they reset |
| mp_suicide_penalty | true | sv, release | Punish players for suicides |
| mp_swapteams | cmd | sv | Swap the teams and restart the game |
| mp_t_default_grenades | 0 | sv, cl, rep, release | The default grenades that the Ts will spawn with. To give multiple grenades, separate each weapon class with a space like this |
| mp_t_default_melee | weapon_knife | sv, cl, rep, release | The default melee weapon that the Ts will spawn with |
| mp_t_default_primary | 0 | sv, cl, rep, release | The default primary (rifle) weapon that the Ts will spawn with |
| mp_t_default_secondary | weapon_glock | sv, cl, rep, release | The default secondary (pistol) weapon that the Ts will spawn with |
| mp_tagging_scale | 1 | sv, rep, release | Scalar for player tagging modifier when hit. Lower values for greater tagging. |
| mp_taser_recharge_time | -1 | sv, cl, rep, release | Determines recharge time for taser. -1 = disabled. |
| mp_td_dmgtokick | 300 | sv, rep, release | The damage threshhold players have to exceed in a match to get kicked. |
| mp_td_dmgtowarn | 200 | sv, rep, release | The damage threshhold players have to exceed in a match to get warned that they are about to be kicked. |
| mp_td_spawndmgthreshold | 50 | sv, rep, release | The damage threshold players have to exceed at the start of the round to be warned/kick. |
| mp_tdm_healthshot_killcount | 3 | sv, cl, rep, release | Grant healthshots in team deathmatch after n kills |
| mp_team_intro_time | 6.5 | sv, nf, rep, release | How many seconds for team intro |
| mp_team_timeout_max | 1 | sv, cl, rep, release | Number of timeouts each team gets per match. |
| mp_team_timeout_time | 60 | sv, cl, rep, release | Duration of each timeout. |
| mp_teamcashawards | true | sv, cl, rep, release | Teams can earn money by performing in-game actions |
| mp_teamflag_1 | 0 | sv, release | Enter a country's alpha 2 code to show that flag next to team 1's name in the spectator scoreboard. |
| mp_teamflag_2 | 0 | sv, release | Enter a country's alpha 2 code to show that flag next to team 2's name in the spectator scoreboard. |
| mp_teamlogo_1 | 0 | sv, release | Enter a team's shorthand image name to display their logo. Images can be found here |
| mp_teamlogo_2 | 0 | sv, release | Enter a team's shorthand image name to display their logo. Images can be found here |
| mp_teammatchstat_1 | 0 | sv, release | A non-empty string sets first team's match stat. |
| mp_teammatchstat_2 | 0 | sv, release | A non-empty string sets second team's match stat. |
| mp_teammatchstat_cycletime | 45 | sv, release | Cycle match stats after so many seconds |
| mp_teammatchstat_holdtime | 5 | sv, release | Decide on a match stat and hold it additionally for at least so many seconds |
| mp_teammatchstat_txt | 0 | sv, release | A non-empty string sets the match stat description, e.g. 'Match 2 of 3'. |
| mp_teammates_are_enemies | false | sv, cl, nf, rep, release | When set, your teammates act as enemies and all players are valid targets. |
| mp_teamname_1 | 0 | sv, release | A non-empty string overrides the first team's name. |
| mp_teamname_2 | 0 | sv, release | A non-empty string overrides the second team's name. |
| mp_teamprediction_pct | 0 | sv, release | A value between 1 and 99 will show predictions in favor of CT team. |
| mp_teamprediction_txt | #SFUIHUD_Spectate_Predictions | sv, release | A value between 1 and 99 will set predictions in favor of first team. |
| mp_teamscore_1 | 0 | sv, release | A non-empty string for best-of-N maps won by the first team. |
| mp_teamscore_2 | 0 | sv, release | A non-empty string for best-of-N maps won by the second team. |
| mp_teamscore_max | 0 | sv, release | How many maps to win the series (bo3 max=2; bo5 max=3; bo7 max=4) |
| mp_technical_timeout_duration_s | 120 | sv, cl, rep, release | How many seconds is a full technical timeout? |
| mp_technical_timeout_per_team | 1 | sv, cl, rep, release | How many technical timeouts are there per team? |
| mp_timelimit | 0 | sv, cl, nf, rep, release | game time per map in minutes |
| mp_tkpunish | 0 | sv, rep, release | Will TK'ers and team damagers be punished in the next round?  {0=no,  1=yes} |
| mp_unpause_match | cmd | sv | Resume the match |
| mp_use_respawn_waves | 0 | sv, cl, rep, release | When set to 1, and that player's team is set to respawn, they will respawn in waves. If set to 2, teams will respawn when the whole team is dead. |
| mp_verbose_changelevel_spew | 1 | sv, cl, rep, release |  |
| mp_warmup_end | cmd | sv | End warmup immediately. |
| mp_warmup_offline_enabled | false | sv, cl, rep, release | Whether or not to do a warmup period at the start of a match in an offline (bot) match. |
| mp_warmup_online_enabled | true | sv, cl, rep, release | Whether or not to do a warmup period at the start of an online match. |
| mp_warmup_pausetimer | 0 | sv, cl, rep, release | Set to 1 to stay in warmup indefinitely. Set to 0 to resume the timer. |
| mp_warmup_start | cmd | sv | Start warmup. |
| mp_warmuptime | 300 | sv, cl, rep, release | How long the warmup period lasts. Changing this value resets warmup. |
| mp_warmuptime_all_players_connected | 60 | sv, cl, rep, release | Warmup time to use when all players have connected. 0 to disable. |
| mp_weapon_melee_touch_time_after_hit | 5 | sv, cheat, release |  |
| mp_weapon_next_owner_touch_time | 1.3 | sv, cheat, release |  |
| mp_weapon_prev_owner_touch_time | 1.5 | sv, cheat, release |  |
| mp_weapon_self_inflict_amount | 0 | sv, rep, release | If Set to non-0, will hurt the attacker by the specified fraction of max damage if they miss. |
| mp_weapons_allow_heavy | -1 | sv, cl, rep, release | Determines which team, if any, can purchase Heavy guns. -1 = any; 0 = non; 2 = Ts; 3 = CTs. |
| mp_weapons_allow_heavyassaultsuit | false | sv, cl, rep, release | Determines whether heavyassaultsuit is permitted. |
| mp_weapons_allow_map_placed | true | sv, cl, rep, release | If this convar is set, when a match starts, the game will not delete weapons placed in the map. |
| mp_weapons_allow_pistols | -1 | sv, cl, rep, release | Determines which team, if any, can purchase Pistols. -1 = any; 0 = non; 2 = Ts; 3 = CTs. |
| mp_weapons_allow_rifles | -1 | sv, cl, rep, release | Determines which team, if any, can purchase Rifles. -1 = any; 0 = non; 2 = Ts; 3 = CTs. |
| mp_weapons_allow_smgs | -1 | sv, cl, rep, release | Determines which team, if any, can purchase SMGs. -1 = any; 0 = non; 2 = Ts; 3 = CTs. |
| mp_weapons_allow_typecount | 5 | sv, cl, rep, release | Determines how many purchases of each weapon type allowed per player per round (0 to disallow purchasing, -1 to have no limit). |
| mp_weapons_allow_zeus | 5 | sv, cl, rep, release | Determines how many Zeus purchases a player can make per round (0 to disallow, -1 to have no limit). |
| mp_weapons_glow_on_ground | false | sv, cl, rep, release | If this convar is set, weapons on the ground will have a glow around them. |
| mp_weapons_max_gun_purchases_per_weapon_per_match | -1 | sv, cl, rep, release | Max number of times a player may purchase any weapon per match |
| mp_win_panel_display_time | 3 | sv, cl, rep, release | The amount of time to show the win panel between matches / halfs |
| multvar | cmd | norecord | Multiply specified convar value. |
| name | star @STR | a, per_user |  |
| nav_add_to_selected_set | cmd | sv, cheat | Add current area to the selected set. |
| nav_add_to_selected_set_by_id | cmd | sv, cheat | Add specified area id to the selected set. |
| nav_avoid | cmd | sv, cheat | Toggles the 'avoid this area when possible' flag used by the AI system. |
| nav_avoid_obstacles | true | sv, cheat |  |
| nav_begin_deselecting | cmd | sv, cheat | Start continuously removing from the selected set. |
| nav_begin_drag_deselecting | cmd | sv, cheat | Start dragging a selection area. |
| nav_begin_drag_selecting | cmd | sv, cheat | Start dragging a selection area. |
| nav_begin_selecting | cmd | sv, cheat | Start continuously adding to the selected set. |
| nav_bfs_debug | 0 | sv, cheat |  |
| nav_check_connectivity | cmd | sv, cheat | Checks to be sure every (or just the marked) nav area can get to every goal area for the map (hostages or bomb site). |
| nav_clear_attribute | cmd | sv, cheat | Remove given nav attribute from all areas in the selected set. |
| nav_clear_attributes | cmd | sv, cheat | Clear all nav attributes of selected area. |
| nav_clear_selected_set | cmd | sv, cheat | Clear the selected set. |
| nav_corner_adjust_adjacent | 18 | cheat | radius used to raise/lower corners in nearby areas when raising/lowering corners. |
| nav_curve_alt | false | sv, cheat |  |
| nav_curve_iter | 0 | sv, cheat |  |
| nav_curve_lock | -1 | sv, cheat |  |
| nav_curve_max_step | 10 | sv, cheat |  |
| nav_curve_set | -1 | sv, cheat |  |
| nav_curve_step | 0.02 | sv, cheat |  |
| nav_debug_blocked | false | sv, cheat |  |
| nav_delete | cmd | sv, cheat | Deletes the currently highlighted Area. |
| nav_delete_all_hull | cmd | sv, cheat | Deletes all areas with given hull category. |
| nav_delete_marked | cmd | sv, cheat | Deletes the currently marked Area (if any). |
| nav_disconnect | cmd | sv, cheat | To disconnect two Areas, mark an Area, highlight a second Area, then invoke the disconnect command. This will remove all connections between the two Areas. |
| nav_draw_area_filled | true | sv, cheat |  |
| nav_draw_area_ground | false | sv, cheat |  |
| nav_draw_area_ztest | false | sv, cheat |  |
| nav_draw_attribute_dynamic | 0 | sv, cheat | Draw all nav areas with this dynamic attribute |
| nav_draw_attribute_game | 0 | sv, cheat | Draw all nav areas with this game attribute |
| nav_draw_blocked | true | sv, cheat |  |
| nav_draw_blocked_connections | false | sv, cheat |  |
| nav_draw_connected_area_radius | 1000 | sv, cheat |  |
| nav_draw_connections | false | sv, cheat |  |
| nav_draw_dangerareas | false | sv, cheat |  |
| nav_draw_externally_created | false | sv, cheat |  |
| nav_draw_hidingspots | false | sv, cheat |  |
| nav_draw_hull_support | false | sv, cheat |  |
| nav_draw_indices | false | sv, cheat |  |
| nav_draw_inset_margin | 0 | sv, cheat |  |
| nav_draw_jump_links | false | sv, cheat |  |
| nav_draw_limit | 300 | sv, cheat | The maximum number of areas to draw in edit mode |
| nav_draw_link_alignment | false | sv, cheat |  |
| nav_draw_links | false | sv, cheat |  |
| nav_draw_markup | true | sv, cheat |  |
| nav_draw_markup_offset | 4 | sv, cheat |  |
| nav_draw_mesh | true | sv, cheat |  |
| nav_draw_mesh_grid | false | sv, cheat | Draw the mesh's spatial grid structure around the edit cursor position. |
| nav_draw_mesh_offset | 1 | sv, cheat | Vertical offset for drawing the mesh (useful for flat planes where the mesh is often a fixed offset from the physical ground |
| nav_draw_should_be_destroyed | false | sv, cheat |  |
| nav_draw_space_bounds | false | sv, cheat |  |
| nav_draw_space_fly | false | sv, cheat |  |
| nav_draw_space_neighbors | false | sv, cheat |  |
| nav_draw_space_portals | false | sv, cheat |  |
| nav_draw_space_swim | false | sv, cheat |  |
| nav_draw_split_by_nav_link_mgr | false | sv, cheat |  |
| nav_draw_split_by_obstacle_mgr | false | sv, cheat |  |
| nav_draw_vert_hotspots | false | sv, cheat |  |
| nav_draw_vertex_normal | false | sv, cheat |  |
| nav_edit | 0 | sv, cheat | Set to one to interactively edit the Navigation Mesh. Set to zero to leave edit mode. |
| nav_edit_validate | false | sv, cheat | Validate navmesh structures. |
| nav_end_deselecting | cmd | sv, cheat | Stop continuously removing from the selected set. |
| nav_end_drag_deselecting | cmd | sv, cheat | Stop dragging a selection area. |
| nav_end_drag_selecting | cmd | sv, cheat | Stop dragging a selection area. |
| nav_end_selecting | cmd | sv, cheat | Stop continuously adding to the selected set. |
| nav_gen_add_jumps | true | cheat |  |
| nav_gen_agent_radius_buffer | 0.75 | cheat | Buffer to add to agent radius before passing to nav gen |
| nav_gen_clip_polys_to_clearance | true | cheat |  |
| nav_gen_clip_polys_to_clearance_debug | false | cheat |  |
| nav_gen_connect_allow_multiple | true | cheat |  |
| nav_gen_connect_angle | 0.75 | cheat |  |
| nav_gen_connect_angle_ignore_z | true | cheat |  |
| nav_gen_connect_dist_a | 1 | cheat |  |
| nav_gen_connect_dist_b | 1.5 | cheat |  |
| nav_gen_connect_dist_z_mult | 0.5 | cheat |  |
| nav_gen_connect_overlap | 0.5 | cheat |  |
| nav_gen_degen_limit | 0.001 | cheat |  |
| nav_gen_false | false | cheat | Always false |
| nav_gen_island_removal | false | cheat |  |
| nav_gen_island_removal_all_hulls | true | cheat |  |
| nav_gen_join_nonzup | true | cheat |  |
| nav_gen_jump_connection_min_overlap_ratio | 0.1 | cheat | Minimum edge overlap required for jump connection consideration as a percentage of agent radius |
| nav_gen_markup_split_expand | 2 | cheat |  |
| nav_gen_markup_split_tol_base | 1 | cheat |  |
| nav_gen_markup_split_tol_nonav | 1 | cheat |  |
| nav_gen_markup_split_tol_nonentity | 8 | cheat |  |
| nav_gen_match_ground | false | cheat |  |
| nav_gen_max_bottleneck_width | 128 | cheat |  |
| nav_gen_max_bottleneck_width_do_clip | true | cheat |  |
| nav_gen_max_edge_len | 512 | cheat |  |
| nav_gen_max_edge_len_do_clip | true | cheat |  |
| nav_gen_max_edge_len_split_tol | 24 | cheat |  |
| nav_gen_opt_to_quads | true | cheat |  |
| nav_gen_opt_to_quads_angle_limit | 8 | cheat |  |
| nav_gen_opt_to_quads_num_steps | 6 | cheat |  |
| nav_gen_opt_to_quads_planar_deviation_limit | 4 | cheat |  |
| nav_gen_opt_to_quads_se_limit_end | 0.1 | cheat |  |
| nav_gen_opt_to_quads_se_limit_start | 0.000010 | cheat |  |
| nav_gen_opt_to_quads_weld_limit_end | 0.01 | cheat |  |
| nav_gen_opt_to_quads_weld_limit_start | 0 | cheat |  |
| nav_gen_remove_vertical_polys | true | cheat |  |
| nav_gen_split_boundary_polys | false | cheat |  |
| nav_gen_split_multi_connection_polys | true | cheat |  |
| nav_gen_split_multi_connection_polys_tol | 0.01 | cheat |  |
| nav_gen_tr_max_acceptable_cost_1 | 900 | cheat |  |
| nav_gen_tr_max_acceptable_cost_2 | 900 | cheat |  |
| nav_gen_tri_reduce_all | false | cheat |  |
| nav_gen_true | true | cheat | Always true |
| nav_gen_vertical_limit | 88 | cheat |  |
| nav_genrt_debug | false | sv, cheat |  |
| nav_genrt_no_splice | false | sv, cheat |  |
| nav_genrt_no_split | false | sv, cheat |  |
| nav_genrt_step | -1 | sv, cheat |  |
| nav_lower_drag_volume_max | cmd | sv, cheat | Lower the top of the drag select volume. |
| nav_lower_drag_volume_min | cmd | sv, cheat | Lower the bottom of the drag select volume. |
| nav_mark | cmd | sv, cheat | Marks the Area or Ladder under the cursor for manipulation by subsequent editing commands. |
| nav_mark_attribute | cmd | sv, cheat | Set nav attribute for all areas in the selected set. |
| nav_max_view_distance | 0 | sv, cheat | Maximum range for precomputed nav mesh visibility (0 = default 1500 units) |
| nav_max_vis_delta_list_length | 64 | cheat |  |
| nav_obstacle_genrt | false | sv, cheat |  |
| nav_obstacle_validate | false | sv, cheat |  |
| nav_obstruction_draw | 0 | sv, cheat |  |
| nav_obstruction_draw_change | false | sv, cheat |  |
| nav_obstruction_draw_dist | -1 | sv, cheat |  |
| nav_obstruction_draw_fail_block | false | sv, cheat |  |
| nav_path_debug | false | sv, cheat |  |
| nav_path_debug_compute_with_open_goal | 0 | sv, cheat |  |
| nav_path_draw_areas | false | sv, cheat |  |
| nav_path_draw_arrow | true | sv, cheat |  |
| nav_path_draw_climb_segments | true | sv, cheat |  |
| nav_path_draw_connected_areas | false | sv, cheat |  |
| nav_path_draw_ground_segments | true | sv, cheat |  |
| nav_path_draw_jump_segments | true | sv, cheat |  |
| nav_path_draw_ladder_segments | true | sv, cheat |  |
| nav_path_draw_link_segments | true | sv, cheat |  |
| nav_path_draw_tick | 0 | sv, cheat |  |
| nav_path_fixup_climb_up_segments | true | sv, cheat |  |
| nav_path_fixup_gap_segments | false | sv, cheat |  |
| nav_path_jump_process_debug | false | sv, cheat |  |
| nav_path_optimize | true | sv, cheat |  |
| nav_path_optimize_portals | true | sv, cheat |  |
| nav_path_optimizer_debug | 0 | sv, cheat |  |
| nav_path_record_draw_last_fail | false | sv, cheat |  |
| nav_path_record_enable | 1 | sv, cheat |  |
| nav_pathfind_debug_draw | 0 | sv, cheat |  |
| nav_pathfind_debug_draw_costs | false | sv, cheat |  |
| nav_pathfind_debug_draw_errors | 0 | sv, cheat |  |
| nav_pathfind_debug_draw_total_costs | false | sv, cheat |  |
| nav_pathfind_debug_log | 0 | sv, cheat |  |
| nav_pathfind_inadmissable_heuristic_factor | 1 | sv, cheat |  |
| nav_potentially_visible_dot_tolerance | 0.98 | sv, cheat |  |
| nav_precise | cmd | sv, cheat | Toggles the 'dont avoid obstacles' flag used by the AI system. |
| nav_raise_drag_volume_max | cmd | sv, cheat | Raise the top of the drag select volume. |
| nav_raise_drag_volume_min | cmd | sv, cheat | Raise the bottom of the drag select volume. |
| nav_recall_selected_set | cmd | sv, cheat | Re-selects the stored selected set. |
| nav_remove_from_selected_set | cmd | sv, cheat | Remove current area from the selected set. |
| nav_select_allow_blocked | true | sv, cheat | When selecting an area under nav_edit, allow area marked as blocked. |
| nav_select_area_id | -1 | sv, cheat | Select nav area with matching ID. |
| nav_select_block_id | -1 | sv, cheat | Select nav space block with matching ID. |
| nav_select_hull | 0 | sv, cheat | Restrict area selection to areas that can support a hull of the given category |
| nav_select_radius | cmd | sv, cheat | Adds all areas in a radius to the selection set |
| nav_select_with_attribute | cmd | sv, cheat | Selects areas with the given attribute. |
| nav_show_area_connections | true | sv, cheat | Show connections to selected area when true |
| nav_show_area_info_font | Consolas | sv, cheat |  |
| nav_show_area_info_font_size | -1 | sv, cheat |  |
| nav_show_area_info_font_voffset | -11 | sv, cheat |  |
| nav_show_area_verts | true | sv, cheat | Show area vertex positions |
| nav_show_area_water_info | true | sv, cheat |  |
| nav_show_potentially_visible | 0 | cheat | Show areas that are potentially visible from the current nav area |
| nav_smooth_calc_z | true | sv, cheat |  |
| nav_smooth_constrain_results | true | sv, cheat |  |
| nav_smooth_constrain_results_relax | 0.006 | sv, cheat |  |
| nav_smooth_constrain_spring | 2 | sv, cheat |  |
| nav_smooth_constrain_spring_relax | 0.01 | sv, cheat |  |
| nav_smooth_draw_accel | 0 | sv, cheat |  |
| nav_smooth_draw_boundary | 0 | sv, cheat |  |
| nav_smooth_draw_calc | false | sv, cheat |  |
| nav_smooth_draw_constraint_spline | false | sv, cheat |  |
| nav_smooth_draw_constraint_spring | 0 | sv, cheat |  |
| nav_smooth_draw_speed | 0 | sv, cheat |  |
| nav_smooth_enable | true | sv, cheat |  |
| nav_smooth_relax | true | sv, cheat |  |
| nav_smooth_relax_use_timesteps | false | sv, cheat |  |
| nav_smooth_separating_dist_override | 0 | sv, cheat |  |
| nav_smooth_spring_const_override | -1 | sv, cheat |  |
| nav_smooth_spring_factor_deriv | 0 | sv, cheat |  |
| nav_smooth_spring_factor_dist | 0 | sv, cheat |  |
| nav_smooth_spring_factor_speed | 0 | sv, cheat |  |
| nav_smooth_spring_forward_dist_base | 50 | sv, cheat |  |
| nav_smooth_spring_forward_dist_time_limit | 1 | sv, cheat |  |
| nav_smooth_spring_max_dist | 36 | sv, cheat |  |
| nav_smooth_spring_tension_max_override | -1 | sv, cheat |  |
| nav_smooth_spring_timestep_factor_accel | 100 | sv, cheat |  |
| nav_smooth_spring_timestep_factor_speed | 100 | sv, cheat |  |
| nav_smooth_spring_timestep_max | 0.5 | sv, cheat |  |
| nav_smooth_spring_timestep_min | 0.1 | sv, cheat |  |
| nav_smooth_spring_yaw_rotation_speed | 50 | sv, cheat |  |
| nav_smooth_spring_yaw_threshold | 20 | sv, cheat |  |
| nav_smooth_use_opt | true | sv, cheat |  |
| nav_space_select_dist | 200 | sv, cheat |  |
| nav_split | cmd | sv, cheat | To split an Area into two, align the split line using your cursor and invoke the split command. |
| nav_split_place_on_ground | false | cheat | If true, nav areas will be placed flush with the ground when split. |
| nav_split_show_line | false | sv, cheat | Show the free split line. |
| nav_store_selected_set | cmd | sv, cheat | Stores the current selected set for later retrieval. |
| nav_switch | cmd | sv | Switches to navmesh for the specified spawngroup |
| nav_test_bfs_lattice_dist_0 | -1 | sv, cheat |  |
| nav_test_bfs_lattice_dist_1 | -1 | sv, cheat |  |
| nav_test_bfs_lattice_dist_2 | -1 | sv, cheat |  |
| nav_test_bfs_lattice_hex | false | sv, cheat | Demonstrates searching hexagonal lattice over nav mesh. |
| nav_test_bfs_lattice_mark | 2 | sv, cheat |  |
| nav_test_bfs_lattice_simple | false | sv, cheat |  |
| nav_test_bfs_lattice_spacing_0 | 24 | sv, cheat |  |
| nav_test_bfs_lattice_spacing_1 | 48 | sv, cheat |  |
| nav_test_bfs_lattice_spacing_2 | 96 | sv, cheat |  |
| nav_test_bfs_simple | false | sv, cheat |  |
| nav_test_boundary_zone_circle | 0 | sv, cheat |  |
| nav_test_boundary_zone_force | false | sv, cheat |  |
| nav_test_boundary_zone_grid_dim | 90 | sv, cheat |  |
| nav_test_boundary_zone_path | 0 | sv, cheat |  |
| nav_test_boundary_zone_rays | 100 | sv, cheat |  |
| nav_test_boundary_zone_rays_margin | -1 | sv, cheat |  |
| nav_test_boundary_zone_rays_random | false | sv, cheat |  |
| nav_test_curve_opt | 0 | sv, cheat |  |
| nav_test_detour | false | sv, cheat |  |
| nav_test_find_nearest | false | sv, cheat | Calculate the nearest point on the navmesh to the trace point.  Uses selection from nav_select_hull. |
| nav_test_find_nearest_clear | false | sv, cheat | Calculate the nearest point on the navmesh to the trace point.  Uses selection from nav_select_hull. |
| nav_test_find_random_connected | false | sv, cheat | Demonstrates finding random points that are connected in the nav mesh to the start point. |
| nav_test_find_random_connected_dist_max | 1000 | sv, cheat |  |
| nav_test_find_random_connected_dist_min | 100 | sv, cheat |  |
| nav_test_find_z | 0 | sv, cheat |  |
| nav_test_force_npc_repath | false | sv, cheat |  |
| nav_test_genrt | false | sv, cheat |  |
| nav_test_genrt_place | false | sv, cheat |  |
| nav_test_level_hull | cmd | sv, cheat | Find entities that intrude into the nav mesh.  List those entities in console output, and display bounding boxes around them for a while. |
| nav_test_level_hull_move | cmd | sv, cheat |  |
| nav_test_multi_connection | false | sv, cheat |  |
| nav_test_npc_area | 0 | sv, cheat |  |
| nav_test_npc_collision | 0 | sv, cheat |  |
| nav_test_npc_collision_show_geometry | false | sv, cheat |  |
| nav_test_path | false | sv, cheat | Calculate and draw a path from player/camera position to the test position. |
| nav_test_path_expansion_search | 0 | sv, cheat | Extend nav_test_path by doing an expansion search on that path.  Convar value defines dist. |
| nav_test_path_lock_goal | false | sv, cheat | Lock the pathfinding goal to the current intersection point. |
| nav_test_path_lock_start | false | sv, cheat | Lock the pathfinding start to the current intersection point. |
| nav_test_path_move | false | sv, cheat |  |
| nav_test_path_opt | true | sv, cheat | Enable path optimization for nav_edit_path paths. |
| nav_test_path_opt_transitions | false | sv, cheat |  |
| nav_test_path_return | false | sv, cheat | Calculate a return path from cursor position to the path calculated by nav_test_path. |
| nav_test_path_space | 0 | sv, cheat | Should nav_test_path test 3d navigation?  1 = space to space, 2 = multi-modal space/ground |
| nav_test_path_space_fly | true | sv, cheat | Test flight paths |
| nav_test_path_space_swim | true | sv, cheat | Test swim paths |
| nav_test_ray_space | false | sv, cheat |  |
| nav_test_rays | false | sv, cheat |  |
| nav_test_smooth | false | sv, cheat |  |
| nav_test_smooth_extern_push | 0 | sv, cheat |  |
| nav_test_smooth_in_speed | 120 | sv, cheat |  |
| nav_test_smooth_in_yaw | 0 | sv, cheat |  |
| nav_test_smooth_path_speed | -1 | sv, cheat |  |
| nav_test_smooth_separating_dist | -1 | sv, cheat |  |
| nav_test_smooth_spring_const | -1 | sv, cheat |  |
| nav_test_smooth_spring_tension_max | -1 | sv, cheat |  |
| nav_test_spline | 0 | sv, cheat |  |
| nav_test_split_obstacle | 0 | sv, cheat |  |
| nav_test_split_obstacle_dirty | false | sv, cheat |  |
| nav_test_split_obstacle_leave | false | sv, cheat |  |
| nav_test_split_obstacle_size | 30 | sv, cheat |  |
| nav_test_split_obstacle_update_pos | true | sv, cheat |  |
| nav_toggle_deselecting | cmd | sv, cheat | Start or stop continuously removing from the selected set. |
| nav_toggle_in_selected_set | cmd | sv, cheat | Remove current area from the selected set. |
| nav_toggle_selected_set | cmd | sv, cheat | Toggles all areas into/out of the selected set. |
| nav_toggle_selecting | cmd | sv, cheat | Start or stop continuously adding to the selected set. |
| nav_unmark | cmd | sv, cheat | Clears the marked Area or Ladder. |
| nav_validate | 0 | cheat | Level of validation for nav system.  Higher will be slower. |
| nav_volume_debug | 0 | sv, cheat | Draw or print debug information about nav volume queries. |
| navspace_block_size_max | 1024 | sv, cheat |  |
| navspace_create_tactial_connections | true | sv, cheat |  |
| navspace_create_water_smooth_connections | true | sv, cheat |  |
| navspace_create_water_transition_connections | true | sv, cheat |  |
| navspace_debug_pathfind | -1 | sv, cheat |  |
| navspace_debug_stringpull | 1 | sv, cheat |  |
| navspace_debug_trace | 0 | sv, cheat |  |
| navspace_debug_transition_calc | 0 | sv, cheat |  |
| navspace_draw_cluster | -1 | sv, cheat |  |
| navspace_draw_cluster_neighbor | -1 | sv, cheat |  |
| navspace_draw_water_changes | 0 | sv, cheat | Draw changes in water volumes |
| net_allow_multicast | true | a, release |  |
| net_captureculldata | cmd |  | Captures low-level data to replay path culling algorithm behavior in controlled unit test environment |
| net_channels | cmd |  | Shows net channel info |
| net_client_steamdatagram_enable_override | 0 | cl, release | 0 |
| net_connections_stats | cmd |  | Print detailed network statistics for each network connection |
| net_fakelag | cmd |  | Shorthand for 'net_option FakePacketLag_Recv' |
| net_listallmessages | cmd | cheat | List all registered net messages |
| net_maxroutable | 1200 | a, user | Requested max packet size before packets are 'split'. |
| net_messageinfo | cmd | cheat | Display info about a message (by classname or id) |
| net_option | cmd |  | Get or set SteamNetworkingSockets options such as fake packet lag and loss |
| net_public_adr | 0 | release | For servers behind NAT/DHCP meant to be exposed to the public internet, this is the public facing ip address string |
| net_serializedentitymemory | cmd |  | Spew CSerializedEntity memory |
| net_serializedentitymetadatainfo | cmd |  | Spew CSerializedEntity metadata information |
| net_showudp | false | release | Dump UDP packets summary to console |
| net_showudp_remoteonly | true | release | Dump non-loopback udp only |
| net_spewcounts | cmd |  | Spew serializer counts |
| net_stats_json | cmd |  | Output server networking statistics in json format |
| net_status | cmd |  | Shows current network status |
| net_validatemessages | cmd | cheat | Activates/deactivates net message validation |
| nextdemo | cmd |  | Play next demo in sequence. |
| nextlevel | 0 | sv, nf, release | If set to a valid map name, will trigger a changelevel to the specified map at the end of the round |
| nextmap_print_enabled | false | sv, release | When enabled prints next map to clients |
| nextmode | 0 | sv, nf, rep, release | Sets the game mode to be played when the next level loads |
| noclip | cmd | sv, cheat | Toggle. Player becomes non-solid and flies.  Optional argument of 0 or 1 to force enable/disable |
| noclip_fixup | true | sv, cheat |  |
| notarget | cmd | sv, cheat | Toggle. Player becomes hidden to NPCs. |
| observer_use | cmd | sv |  |
| open_asset | cmd |  | Opens an asset in it's primary editor of choice. Specify the full path to the asset from the mod directory. |
| option_duck_method | false | cl, a, user, per_user | Input toggle control |
| option_speed_method | false | cl, a, user, per_user | Input toggle control |
| p2p_listpeers | cmd |  | List currently known peers. |
| p2p_ping | cmd | cl | Ping a peer. |
| panorama_debugger_theme | Light | cl, a |  |
| panorama_focus_world_panels | false | cl, a | when set request key focus when a world panel is enabled |
| particle_profile | cmd |  | Profile particle |
| particle_profile_spike | cmd |  | Profile particle spike |
| particle_test_attach_attachment | 0 | sv, cheat | Attachment index for attachment mode |
| particle_test_attach_mode | follow_attachment | sv, cheat | Possible Values |
| particle_test_create | cmd | sv, cheat | Creates the named particle system where the player is looking.  Arguments |
| particle_test_destroy | cmd | sv, cheat | Destroys all particle systems matching the specified name.  Arguments |
| particle_test_file | 0 | sv, cheat | Name of the particle system to dynamically spawn |
| particle_test_start | cmd | sv, cheat | Dispatches the test particle system with the parameters specified in particle_test_file,  particle_test_attach_mode and particle_test_attach_param on the entity the player is looking at.  Arguments |
| particle_test_stop | cmd | sv, cheat | Stops all particle systems on the selected entities.  Arguments |
| particles_multiplier | 1 | cheat | Multiply # of rendered particles by this for perf testing |
| password | 0 | a, norecord, server_cant_query | Current server access password |
| path | cmd |  | Show the filesystem path. |
| pause | cmd |  | Toggle the server pause state. |
| phys_create_test_character_proxy | cmd | sv | Create test character proxy |
| phys_debug_draw | cmd |  | Set up debug-draw of physics internal state |
| phys_debug_showdefaultmaterial | false | cheat | If enabled, surfaces with default material are highlighted in physics debug geometry. |
| phys_dump_intersection_controller | cmd | sv | Dump intersection controller status |
| phys_dynamic_scaling | true | sv, cl, rep, cheat |  |
| phys_joint_teleport | true | sv, cheat | Teleport joint anchors if connected to world |
| phys_length_damping_ratio | 2 | sv, cheat | Spring damping ratio for length constraint |
| phys_length_frequency | 5 | sv, cheat | Spring stiffness for length constraint |
| phys_list | cmd | sv | List all physics component contents of every entity in the game;     -stream [1|0] |
| phys_mark_debug | cmd | sv, cheat | Mark object for debug |
| phys_shoot | cmd | sv, cheat | Shoots a phys object. |
| phys_sleep | cmd | sv | Put all physics in all the worlds to sleep |
| phys_use_block_solver | true | sv, cheat | Use block solving for constraint entities |
| phys_visualize_traces | false | sv, cl, rep, cheat |  |
| phys_wakeup | cmd | sv | Wake all physics objects in the Main physics up |
| physics_add_test | cmd | sv | add test object |
| physics_debug_entity | cmd | sv | Dumps debug info for an entity |
| physics_highlight_active | cmd | sv | Turns on the absbox for all active physics objects.   0 |
| physics_remove_test | cmd | sv | remove test object |
| physics_report_active | cmd | sv | Lists all active physics objects   -more |
| pixelvis_debug | cmd | cheat | Dump debug info |
| play | cmd | server_can_execute | Play a sound. |
| playcast | cmd |  | Play a broadcast |
| playdemo | cmd |  | Play a recorded demo file (.dem ). |
| player0_using_joystick | false | a |  |
| player_botdifflast_s | 4 | cl, a, release |  |
| player_competitive_maplist_2v2_10_0_DBAEB932 | mg_de_train,mg_de_lake,mg_de_inferno,mg_de_nuke,mg_de_vertigo,mg_de_shortdust,mg_de_overpass | cl, a |  |
| player_competitive_maplist_8_10_0_FB803604 | mg_de_dust2 | cl, a |  |
| player_debug_off_nav | false | sv, cheat |  |
| player_debug_print_damage | false | sv, cheat | When true, print amount and type of all damage received by player to console. |
| player_nevershow_communityservermessage | 0 | cl, a, per_user |  |
| player_ping | cmd | sv | Creates a ping notification where the player is looking. |
| player_ping_token_cooldown | 20 | sv, cheat, release | Cooldown for how long it takes for a player's ping token to refresh allowing them to ping again (they get 5 tokens). |
| player_survival_list_10_0_303 | mg_dz_blacksite,mg_dz_sirocco,mg_dz_vineyard,mg_dz_ember | cl, a |  |
| player_teamplayedlast | 2 | cl, a, per_user |  |
| player_use_radius | 80 | sv, cl, rep, cheat |  |
| player_wargames_list2_10_0_DC207394 | mg_skirmish_armsrace | cl, a |  |
| playsound | cmd |  | playsound <soundname> |
| playsoundscape | cmd | cl, cheat | Forces a soundscape to play |
| playvol | cmd |  | Play a sound at a specified volume. |
| png_screenshot | cmd |  | Take a .png screenshot |
| pop_var_values | cmd |  | Restore previously pushed convars and config values |
| print_mapgroup | cmd | cl, release | Prints the current mapgroup and the contained maps |
| print_mapgroup_sv | cmd | sv, release | Prints the current mapgroup and the contained maps |
| print_model_bind_pose | cmd |  | Prints the bind pose of the specified model. Optionally limits to a particular bone and its parent chain, otherwise prints the entire skeleton. |
| progress_enable | cmd |  |  |
| prop_debug | cmd | sv, cheat | Toggle prop debug mode. If on, props will show colorcoded bounding boxes. Red means ignore all damage. White means respond physically to damage but never break. Green maps health in the range of 100 down to 1. |
| prop_debug_vr_collision | false | sv, cheat | Highlights props based on their collision group |
| prop_dynamic_create | cmd | sv, cheat | Creates a dynamic prop with a specific .vmdl aimed away from where the player is looking.  Arguments |
| prop_physics_create | cmd | sv, cheat | Creates a physics prop with a specific .vmdl aimed away from where the player is looking.  Arguments |
| push_var_values | cmd |  | Save convars and config values |
| pvs_debugentity | -1 | sv, release | Verbose spew for this entity when doing IsInPVS computation. |
| pvs_flowtype | 0 | sv, release | Flow through spawn groups for vis (0 == default, 1 == always visible, 2 == never visible. |
| pwatchent | -1 | cl, cheat | Entity to watch for prediction system changes. |
| pwatchvar | 0 | cl, cheat | Entity variable to watch in prediction system for changes. |
| +quickbuyradial | cmd | cl |  |
| +quickgearradial | cmd | cl |  |
| +quickgrenaderadial | cmd | cl |  |
| +quickinv | cmd | cl |  |
| quit | cmd | vconsole_set_focus | Quit the game |
| r_AirboatViewDampenDamp | 1 | sv, cl, nf, rep, cheat |  |
| r_AirboatViewDampenFreq | 7 | sv, cl, nf, rep, cheat |  |
| r_AirboatViewZHeight | 0 | sv, cl, nf, rep, cheat |  |
| r_aoproxy_debug | false | cl, cheat |  |
| r_camerapos | cmd | linked | Prints out the current camera position + orientation to the console |
| r_csgo_cubemap_normalization | true | cl, cheat |  |
| r_csgo_debug_reflection_rects | 0 | cl, cheat |  |
| r_csgo_decal_debug | false | cl, cheat |  |
| r_csgo_depth_prepass | true | cl, cheat |  |
| r_csgo_depth_prepass_cull_threshold | 60 | cl, cheat |  |
| r_csgo_depth_prepass_players | true | cl, cheat |  |
| r_csgo_depth_prepass_reflections_large | true | cl, cheat |  |
| r_csgo_depth_prepass_reflections_small | true | cl, cheat |  |
| r_csgo_depth_prepass_skybox_alpha_tested | true | cl, cheat |  |
| r_csgo_depth_prepass_small_cull_threshold | 10 | cl, cheat |  |
| r_csgo_depth_prepass_viewmodel | true | cl, cheat |  |
| r_csgo_directional_lightmaps | true | cl, cheat |  |
| r_csgo_effects_bloom | true | cl, cheat |  |
| r_csgo_effects_bloom_when_smoked | false | cl, cheat |  |
| r_csgo_enable_glows | true | cl, cheat |  |
| r_csgo_enable_high_precision_lighting | true | cl, cheat |  |
| r_csgo_enable_outlines | true | cl, cheat |  |
| r_csgo_enable_tonemapping | true | cl, cheat |  |
| r_csgo_enable_translucent_screen_space | true | cl, cheat |  |
| r_csgo_mboit | true | cl, cheat |  |
| r_csgo_mboit_bias | 0.000005 | cl, cheat |  |
| r_csgo_mboit_debug | false | cl, cheat |  |
| r_csgo_mboit_overestimation | 0.01 | cl, cheat |  |
| r_csgo_mboit_use_4_moments | false | cl, cheat |  |
| r_csgo_mixed_resolution_color_slices | false | cl, cheat |  |
| r_csgo_mixed_resolution_particles_minmax | false | cl, cheat |  |
| r_csgo_mixed_resolution_particles_scale | 2 | cl, cheat |  |
| r_csgo_no_shader_resolve | false | cl, cheat |  |
| r_csgo_override_global_time | true | cl, cheat |  |
| r_csgo_postprocess_enable | true | cl, cheat |  |
| r_csgo_readonly_depth_stencil_enable | true | cl, cheat |  |
| r_csgo_reflection_min_far_plane | 5000 | cl, cheat |  |
| r_csgo_render_decals | true | cl, cheat |  |
| r_csgo_render_decals_on_translucent | true | cl, cheat |  |
| r_csgo_render_dynamic_objects | true | cl, cheat |  |
| r_csgo_render_inferno_decals | true | cl, cheat |  |
| r_csgo_render_opaque | true | cl, cheat |  |
| r_csgo_render_overlays | true | cl, cheat |  |
| r_csgo_render_post_bloom_strength | -1 | cl, cheat |  |
| r_csgo_render_post_local_contrast | true | cl, cheat |  |
| r_csgo_render_translucent | true | cl, cheat |  |
| r_csgo_shadows_debug | 0 | cl, cheat |  |
| r_csgo_volume_mboit_optimization | true | cl, cheat |  |
| r_csgo_water_effects | true | cl, cheat |  |
| r_csgo_water_refraction | true | cl, cheat |  |
| r_cubemap_debug_colors | 0 | cheat |  |
| r_debug_particle_shadows | false | cl, cheat |  |
| r_debug_precipitation | false | cl, cheat | Show precipitation volumes |
| r_directlighting | true | cheat | Set to use direct lighting |
| r_dof_override | false | cheat |  |
| r_dof_override_far_blurry | 2000 | cheat |  |
| r_dof_override_far_crisp | 180 | cheat |  |
| r_dof_override_near_blurry | -100 | cheat |  |
| r_dof_override_near_crisp | 0 | cheat |  |
| r_dof_override_tilt_to_ground | 0.5 | cheat |  |
| r_dopixelvisibility | true | cheat |  |
| r_draw_first_tri_only | false | cheat |  |
| r_draw_instances | true | cheat |  |
| r_draw_particle_children_with_parents | -1 | cheat | Draw particle children with parents (-1=use gameinfo, 0=no, 1=yes) |
| r_drawblankworld | false | cheat | Render blank instead of the game world |
| r_drawchickens | true | cl, cheat | Render chickens |
| r_drawcsplayers | true | cl, cheat | Render CS players |
| r_drawdecals | true | cheat | Set to render decals |
| r_drawdevvisualizers | false | cl, cheat | Render dev visualizers |
| r_drawpanorama | true | cheat | Enable the rendering of panorama UI |
| r_drawparticles | true | cheat | Enable/disable particle rendering |
| r_drawropes | true | cl, cheat |  |
| r_drawskybox | true | cheat | Render the 2d skybox. |
| r_drawsprites | true | cl, cheat |  |
| r_drawtracers | true | cl, cheat |  |
| r_drawviewmodel | true | cl, cheat | Render view model |
| r_drawworld | true | cheat | Render the world. |
| r_dx11_report_live_objects | cmd |  | Prints out live D3D11 objects (requires -dx11debug) |
| r_entpos | cmd | linked | Moves the camera position + orientation to the named entity |
| r_extra_render_frames | 0 | cheat |  |
| r_fallback_texture_lod_scale | 2 | cheat | Scale factor for requested texture size (texture streaming) - used for geo that doesn't have a precomputed UV density measure |
| r_farz | -1 | cl, cheat | Override the far clipping plane. -1 means to use the value in env_fog_controller. |
| r_flashlightambient | 0 | cl, cheat |  |
| r_flashlightbacktraceoffset | 0.4 | cl, cheat |  |
| r_flashlightbrightness | 1 | cl, rep, cheat |  |
| r_flashlightconstant | 0 | cl, rep, cheat |  |
| r_flashlightfar | 1500 | cl, rep, cheat |  |
| r_flashlightfov | 53 | cl, rep, cheat |  |
| r_flashlightladderdist | 40 | cl, cheat |  |
| r_flashlightlinear | 100 | cl, rep, cheat |  |
| r_flashlightlockposition | false | cl, cheat |  |
| r_flashlightmuzzleflashfov | 120 | cl, cheat |  |
| r_flashlightnear | 4 | cl, rep, cheat |  |
| r_flashlightnearoffsetscale | 1 | cl, cheat |  |
| r_flashlightoffsetforward | 0 | cl, rep, cheat |  |
| r_flashlightoffsetright | 5 | cl, rep, cheat |  |
| r_flashlightoffsetup | -5 | cl, rep, cheat |  |
| r_flashlightquadratic | 0 | cl, rep, cheat |  |
| r_flashlightshadowatten | 0.35 | cl, cheat |  |
| r_flashlighttracedistcutoff | 128 | cl, cheat |  |
| r_flashlighttracedistwatercutoff | 80 | cl, cheat |  |
| r_flashlightvisualizetrace | false | cl, cheat |  |
| r_force_engine_render_frame | cmd |  | Force a single render of the engine viewport. |
| r_force_no_present | false | cheat | Force the render device to not present frames. |
| r_force_zprepass | -1 | cheat | 0 |
| r_freezeparticles | false | cheat | Pause particle simulation |
| r_fullscreen_gamma | 2.2 | a | Screen Gamma (only in fullscreen modes) |
| r_gpu_mem_stats | cmd | linked | Display GPU memory usage. |
| r_incrementlodscale | cmd | linked | Modifies the LOD scale |
| r_indirectlighting | true | cheat | Set to use indirect lighting |
| r_JeepViewDampenDamp | 1 | sv, cl, nf, rep, cheat |  |
| r_JeepViewDampenFreq | 7 | sv, cl, nf, rep, cheat |  |
| r_JeepViewZHeight | 10 | sv, cl, nf, rep, cheat |  |
| r_light_probe_volume_debug_colors | 0 | cheat |  |
| r_light_probe_volume_debug_grid | false | cheat | Show LPV debug grid, 0 |
| r_light_probe_volume_debug_grid_albedo | 128 128 128 | cheat | albedo for LPV debug grid |
| r_light_probe_volume_debug_grid_bbox | true | cheat | Show LPV bounding box when debug grid is on, 0 |
| r_light_probe_volume_debug_grid_metalness | 0 | cheat | metalness for LPV debug grid |
| r_light_probe_volume_debug_grid_prim | 0 | cheat | 0 |
| r_light_probe_volume_debug_grid_roughness | 0.5 | cheat | roughness for LPV debug grid |
| r_light_probe_volume_debug_grid_samplesize | 4 | cheat | sphere radius (world) for LPV debug grid |
| r_lightBinnerFarPlane | 4096 | cheat |  |
| r_lightmap_set | lightmaps | cheat | Lightmap set to use, only works on map load |
| r_mapextents | 16384 | cl, cheat | Set the max dimension for the map.  This determines the far clipping plane |
| r_morphing_enabled | true | cheat |  |
| r_muzzleflashbrightness | 0.4 | cl, rep, cheat |  |
| r_muzzleflashlinear | 0.05 | cl, rep, cheat |  |
| r_nearz | -1 | cl, cheat | Override the near clipping plane. -1 means use the default. |
| r_particle_max_draw_distance | 1000000.000000 | cheat | The maximum distance that particles will render |
| r_pixelvisibility_partial | true | cheat |  |
| r_pixelvisibility_spew | false | cheat |  |
| r_player_visibility_mode | 1 | cl, a, release |  |
| r_print_texture_stats | cmd |  | Texture stats |
| r_printdecalinfo | cmd | cl | Prints info about decals currently in the scene |
| r_refraction_clip_plane_adjust | -1 | cl, cheat |  |
| r_render_coordination_state | cmd |  | Prints out the current render coordination state. |
| r_render_world_node_bounds | false | cheat | Render world node bounds |
| r_renderdoc_capture_frame | cmd | linked | Triggers a RenderDoc capture |
| r_rendersun | true | cheat | Render sun lighting |
| r_replay_post_effect | -1 | cl, cheat |  |
| r_setpos | cmd | linked | Moves the camera position + orientation to the specified position |
| r_shadows | true | cheat |  |
| r_show_ao_proxies | false | cl, cheat |  |
| r_show_hipoly_draw_calls | 0 | cheat | Transparent wireframe overlay for draw calls with triangle count higher than specified number |
| r_showdebugoverlays | false | cheat | Set to render debug overlays |
| r_showdebugrendertarget | false | cheat | Set the debug render target to show, 0 == disable |
| r_showsceneobjectbounds | false | cheat | Show scenesystem object bounding boxes |
| r_showsunshadowdebugrendertargets | false | cheat | Set to render sun shadow render targets |
| r_showsunshadowdebugsplitvis | false | cheat | Set to render sun shadow split visibility debugger |
| r_size_cull_threshold_shadow | 0.2 | cheat | Threshold of sun shadow map size percentage below which objects get culled |
| r_skinning_enabled | true | cheat |  |
| r_stereo_multiview_instancing | false | cheat | Use multiview instancing for stereo rendering. |
| r_texture_lod_scale | 1 | cheat | Scale factor for requested texture size (texture streaming) |
| r_textures_evict_all | cmd | linked | Evict all resident texture. |
| r_toggleviewportsize | cmd |  | Toggles viewport size between small + full window. |
| r_translucent | true | cheat | Enable rendering of translucent geometry |
| r_viewport | cmd |  | Slams viewport size to a specified value. |
| r_worldlod | true | cheat | Set to enable world LOD |
| r_zprepass_normals | false | cheat | 0 |
| radarvisdistance | 1000 | sv, cheat | at this distance and beyond you need to be point right at someone to see them |
| radarvismaxdot | 0.996 | sv, cheat | how closely you have to point at someone to see them beyond max distance |
| radarvismethod | 1 | sv, cheat | 0 for traditional method, 1 for more realistic method |
| radarvispow | 0.4 | sv, cheat | the degree to which you can point away from a target, and still see them on radar. |
| +radialradio | cmd | cl |  |
| +radialradio2 | cmd | cl |  |
| +radialradio3 | cmd | cl |  |
| radio | cmd | cl | Opens a radio menu |
| radio1 | cmd | cl | Opens a radio menu |
| radio2 | cmd | cl | Opens a radio menu |
| radio3 | cmd | cl | Opens a radio menu |
| ragdoll_friction_scale | 0.6 | sv, cl, rep, cheat |  |
| ragdoll_gravity_scale | 1 | sv, cl, rep, cheat |  |
| ragdoll_lru_debug_removal | false | sv, cl, rep, cheat |  |
| ragdoll_lru_min_age | 10 | sv, cl, rep, cheat |  |
| rangefinder | cmd | sv, cheat | Measures distance along a ray |
| rate | 786432 | a, user | Min bytes/sec the host can receive data |
| ray_bench | cmd | sv | Load the rays and run the benchmark |
| rcon | cmd | norecord | Issue an rcon command. |
| rcon_address | 0 | norecord, release, server_cant_query | Address of remote server if sending unconnected rcon commands (format x.x.x.x |
| rcon_connected_clients_allow | true | rep, release | Allow clients to use rcon commands on server. |
| rcon_password | 0 | norecord, release, server_cant_query | remote console password. |
| rebuy | cmd | cl, clientcmd_can_execute | Attempt to repurchase items with the order listed in cl_rebuy |
| recast_mark_overhang | true | rep, cheat | Enable/disable overhang detection |
| recast_partitioning | 0 | rep, cheat | 0 = watershed, 1 = monotone, 2 = layers |
| record | cmd | norecord | Record a demo. |
| refresh_ui_audio_state | cmd | cl, cheat | Restores audio DSP state for the UI. |
| regenerate_weapon_skins | cmd | cl, cheat |  |
| reload_model | cmd |  | Force a reload of a vmdl resource |
| reload_store_config | cmd | cl |  |
| reloadgame | cmd | cheat, vconsole_set_focus | Reload the most recent saved game. |
| remove_weapon | cmd | sv, cheat | Remove a weapon held by the player.  Arguments |
| removeid | cmd |  | Remove a user ID from the ban list. |
| removeip | cmd |  | Remove an IP address from the ban list. |
| repeat_last_console_command | cmd |  | Repeat last console command. |
| replay_death | cmd | sv, cheat | start hltv replay of last death |
| replay_debug | 0 | rep, release |  |
| replay_start | cmd | sv, cheat | Start GOTV replay |
| replay_stop | cmd | sv | stop hltv replay |
| report_cliententitysim | false | cl, cheat | List all clientside simulations and time - will report and turn itself off. |
| report_clientthinklist | false | cl, cheat | List all clientside entities thinking and time - will report and turn itself off. |
| report_soundpatch | cmd | sv | reports sound patch count |
| reset_gameconvars | cmd | cheat | Reset game convars to default values |
| resource_leaks | cmd |  | resource_leaks <resource_name> |
| resource_list | cmd |  | List loaded resources matching a substring |
| resource_log_allocate_timing | cmd |  | Log time spent in Allocate for all resource types |
| resource_manifest_validate_modules | cmd |  | Scan all of the loaded modules and validate any resource manifests found |
| resource_repeated_reload | cmd |  | resource_repeated_reload <count> <resource_name> (<resource name> ...) |
| resource_reset_allocate_timing | cmd |  | Reset tracked time spent in Allocate (see resource_log_allocate_timing) |
| respawn_player | cmd | sv, cheat | Respawns the player from death! |
| restart | cmd | cheat, vconsole_set_focus | Poor man's restart |
| rpestats | cmd |  | dump rpe |
| rr_findrules | cmd | sv | Search and list rules by substring. |
| rr_findrules_verbose | cmd | sv | Search and list rules by substring. |
| rr_followup_maxdist | 1800 | sv, cheat | 'then ANY' or 'then ALL' response followups will be dispatched only to characters within this distance. |
| rr_forceconcept | cmd | sv, cheat | fire a response concept directly at a given character. USAGE |
| rr_reloadresponsesystems | cmd | sv, cheat | Reload all response system scripts. |
| rr_thenany_score_slop | 0 | sv, a, cheat | When computing respondents for a 'THEN ANY' rule, all rule-matching scores within this much of the best score will be considered. |
| run_perftest | cmd | cheat, norecord | Execute perftest.cfg |
| safezonex | 1 | cl, a | The percentage of the screen width that is considered safe from overscan. Cannot result in a width less than the height. |
| safezoney | 1 | cl, a | The percentage of the screen height that is considered safe from overscan |
| save | cmd | sv, norecord | Save Game |
| save_animgraph_recording | cmd | sv, cheat | Saves all active animgraph recordings to disk |
| save_clear_subdirectory | cmd | sv, rep |  |
| save_finish_async | cmd | sv |  |
| save_maxarray_spew | 10 | sv, release | Max number of array entries to spew when using SaveRestoreIO spewing. |
| save_set_subdirectory | cmd | sv, rep |  |
| save_showelapsedtime | cmd | sv | display up-to-date elapsed play time |
| save_watchclass | cmd | sv | Restrict spew to entities with matching classname |
| save_watchentity | cmd | sv | Restrict spew to entity index |
| say | cmd | sv | Display player message |
| say_team | cmd | sv | Display player message to team |
| sc_check_world | false | cheat |  |
| sc_disable_culling_boxes | false | cheat |  |
| sc_disable_procedural_layer_rendering | false | cheat |  |
| sc_disable_shadow_fastpath | false | cheat |  |
| sc_disable_shadow_materials | false | cheat |  |
| sc_disable_spotlight_shadows | false | cheat |  |
| sc_disable_world_materials | false | cheat |  |
| sc_disableThreading | false | cheat |  |
| sc_dump_lists | false | cheat |  |
| sc_dumpworld | cmd | cheat | Dump a list of the objects in a sceneworld (Usage |
| sc_dumpworld3d | cmd | cheat | Dump the objects in a sceneworld into a 3d geoview buffer (Usage |
| sc_extended_stats | false | cheat |  |
| sc_force_lod_level | -1 | cheat |  |
| sc_force_materials_batchable | false | cheat |  |
| sc_force_translation_in_projection | false | cheat | If enabled, the camera's translation will be included in the projection matrix. |
| sc_list_extradata_allocations | cmd |  | Prints out the overall extra data allocation counts |
| sc_listworlds | cmd | cheat | List all the active sceneworlds |
| sc_lod_distance_scale_override | -1 | cheat |  |
| sc_log_submits | false | cheat | Log out display list submits from scenesystem |
| sc_only_render_opaque | false | cheat |  |
| sc_only_render_shadowcasters | false | cheat |  |
| sc_override_shadow_fade_max_dist | -1 | cheat |  |
| sc_override_shadow_fade_min_dist | -1 | cheat |  |
| sc_reject_all_objects | false | cheat |  |
| sc_setclassflags | cmd | cheat | Low level command to set the flags byte associated with an object class. sc_SetClassFlags <classname> <value> |
| sc_showclasses | cmd | cheat | List the object class names known by scenesystem |
| sc_skip_traversal | false | cheat |  |
| scene_flush | cmd | sv | Flush all .vcds from the cache and reload from disk. |
| scene_playvcd | cmd | sv, cheat | Play the given VCD as an instanced scripted scene. |
| screenmessage_show | -1 | cheat | Enable display of console messages on screen. 1 = Enabled, 0 = Disabled, -1 = Enabled if vgui is not present |
| screenshot | cmd |  | Take a screenshot |
| script_add_debug_filter | cmd | sv, cheat | Add a filter to the game debug overlay |
| script_add_watch | cmd | sv, cheat | Add a watch to the game debug overlay |
| script_add_watch_pattern | cmd | sv, cheat | Add a watch to the game debug overlay |
| script_attach_debugger | cmd | sv, cheat | Connect the vscript VM to the script debugger |
| script_clear_watches | cmd | sv, cheat | Clear all watches from the game debug overlay |
| script_debug | cmd | sv, cheat | Toggle the in-game script debug features |
| script_dump_all | cmd | sv, cheat | Dump the state of the VM to the console |
| script_find | cmd | sv, cheat | Find a key in the VM |
| script_help | cmd | sv, cheat | Output help for script functions |
| script_help2 | cmd | sv | Output help for script functions suitable for auto-completion |
| script_reload | cmd | sv, cheat | Reload scripts |
| script_reload_code | cmd | sv, cheat | Execute a vscript file, replacing existing functions with the functions in the run script |
| script_reload_entity_code | cmd | sv, cheat | Execute all of this entity's VScripts, replacing existing functions with the functions in the run scripts |
| script_remove_debug_filter | cmd | sv, cheat | Remove a filter from the game debug overlay |
| script_remove_watch | cmd | sv, cheat | Remove a watch from the game debug overlay |
| script_remove_watch_pattern | cmd | sv, cheat | Remove a watch from the game debug overlay |
| script_resurrect_unreachable | cmd | sv, cheat | Use the garbage collector to track down reference cycles |
| script_trace_disable | cmd | sv, cheat | Turn off a particular trace output by file or function name |
| script_trace_disable_all | cmd | sv, cheat | Turn off all trace output |
| script_trace_disable_key | cmd | sv, cheat | Turn off a particular trace output by table/instance |
| script_trace_enable | cmd | sv, cheat | Turn on a particular trace output by file or function name |
| script_trace_enable_all | cmd | sv, cheat | Turn on all trace output |
| script_trace_enable_key | cmd | sv, cheat | Turn on a particular trace output by table/instance |
| scrubber | cmd |  | Scrub system off - not a dev build |
| sdr | cmd |  | An old command that has been renamed to 'net_option' |
| sensitivity | 2.64322 | cl, a, per_user | Mouse sensitivity. |
| server_game_time | cmd | sv | Gives the game time in seconds (server's curtime) |
| server_snd_cast | cmd | sv, cheat | Casts a ray and starts a sound event where the ray hits. The sound event will retrigger periodically. Usage |
| servercfgfile | server.cfg | sv, release |  |
| servervoice_clear | cmd | cl | servervoice_clear |
| servervoice_dump | cmd | cl | servervoice_dump |
| setang | cmd | sv, cheat | Snap player eyes to specified pitch yaw <roll |
| setang_exact | cmd | sv, cheat | Snap player eyes and orientation to specified pitch yaw <roll |
| setinfo | cmd | clientcmd_can_execute | Adds a new user info value |
| setmodel | cmd | sv, cheat | Changes's player's model |
| setpause | cmd |  | Set the pause state of the server. |
| setpos | cmd | sv, cheat | Move player to specified origin (must have sv_cheats). |
| setpos_exact | cmd | sv, cheat | Move player to an exact specified origin (must have sv_cheats). |
| setpos_player | cmd | sv, cheat | Move specified player to specified origin (must have sv_cheats). |
| shake | cmd | sv, cheat | Shake the screen. |
| shake_stop | cmd | cl, cheat | Stops all active screen shakes. |
| shake_testpunch | cmd | cl, cheat | Test a punch-style screen shake. |
| shatterglass_break | cmd | sv, cheat |  |
| shatterglass_cleanup | true | sv, cl, rep, cheat |  |
| shatterglass_cleanup_max | 150 | sv, cl, rep, cheat |  |
| shatterglass_debug | false | sv, cl, rep, cheat |  |
| shatterglass_distort | true | sv, cl, rep, cheat |  |
| shatterglass_edge_uv_scale | 0.05 | sv, cl, rep, cheat |  |
| shatterglass_hit_tolerance | 2 | sv, cl, rep, cheat |  |
| shatterglass_restore | cmd | sv, cheat |  |
| shatterglass_shard_lifetime | 15 | sv, cl, rep, cheat |  |
| shatterglass_subdiv_size | 1.5 | sv, cl, rep, cheat |  |
| shatterglass_voronoi_size | 15 | sv, cl, rep, cheat |  |
| show_loadout_toggle | cmd | cl, clientcmd_can_execute | Toggles loadout display |
| show_visibility_boxes | false | cl, cheat | Enable or Disable debug display of visibility boxes |
| showconsole | cmd | norecord | Show the console. |
| showtriggers | cmd | sv, cheat | Enable or Disable showing trigger entities |
| showtriggers_toggle | cmd | sv, cheat | Displays the movement bounding box for the triggers in orange.  Some entites will also display entity specific overlays.  Arguments |
| silence_dsp | false | cheat | When on, silences all DSP mixes. |
| sk_autoaim_mode | 1 | sv, cl, a, rep |  |
| skel_constraints_enable | true | rep, cheat |  |
| skeleton_instance_smear_boneflags | false | sv, cheat | Smear boneflags across the model.  Costs computation, but tests to make sure your bone flags are consistent. |
| skill | 1 | sv, cl, a, rep, per_user | Game skill level. |
| slot0 | cmd | cl, server_can_execute |  |
| slot1 | cmd | cl, server_can_execute |  |
| slot10 | cmd | cl, server_can_execute |  |
| slot11 | cmd | cl, server_can_execute |  |
| slot12 | cmd | cl, server_can_execute |  |
| slot13 | cmd | cl, server_can_execute |  |
| slot2 | cmd | cl, server_can_execute |  |
| slot3 | cmd | cl, server_can_execute |  |
| slot4 | cmd | cl, server_can_execute |  |
| slot5 | cmd | cl, server_can_execute |  |
| slot6 | cmd | cl, server_can_execute |  |
| slot7 | cmd | cl, server_can_execute |  |
| slot8 | cmd | cl, server_can_execute |  |
| slot9 | cmd | cl, server_can_execute |  |
| snapto | cmd | cl |  |
| snd_arrangement_start | cmd | cheat | Starts the specified arrangement. |
| snd_async_flush | cmd |  | Flush all unlocked async audio data |
| snd_async_showmem | cmd |  | Show async memory stats |
| snd_async_showmem_music | cmd |  | Show async memory stats for just non-streamed music |
| snd_async_showmem_summary | cmd |  | Show brief async memory stats |
| snd_autodetect_latency | true | a |  |
| snd_break_on_start_soundevent | 0 | sv, cl, rep, cheat | Use to debug break on any soundevent that is started matching this name |
| snd_cast | cmd | cheat | Casts a ray and starts a sound event where the ray hits. The sound event will retrigger periodically if cl_snd_cast_retrigger is set. The sound event will clear previous snd_cast events if cl_snd_cast_clear is set. Usage |
| snd_compare_soundevents | cmd | cheat | Compare the compiled and loaded contents of 2 soundevents. |
| snd_deathcamera_volume | 0.2 | cl, a, release | Volume of death camera music |
| snd_disable_mixer_duck | false | cheat |  |
| snd_disable_mixer_solo | false | cheat |  |
| snd_dsp_distance_max | 2000 | cheat |  |
| snd_dsp_distance_min | 20 | cheat |  |
| snd_duckerattacktime | 0.5 | a |  |
| snd_duckerreleasetime | 2.5 | a |  |
| snd_duckerthreshold | 0.15 | a |  |
| snd_ducktovolume | 0.55 | a |  |
| snd_envelope_rate | 0.9 | cheat |  |
| snd_filter | 0 | cheat |  |
| snd_foliage_db_loss | 4 | sv, cheat | foliage dB loss per 1200 units |
| snd_front_headphone_position | cmd |  | Specifies the position (in degrees) of the virtual front left/right headphones. |
| snd_front_stereo_speaker_position | cmd |  | Specifies the position (in degrees) of the virtual front left/right speakers. |
| snd_front_surround_speaker_position | cmd |  | Specifies the position (in degrees) of the virtual front left/right speakers. |
| snd_gain | 1 | a |  |
| snd_gain_max | 1 | cheat |  |
| snd_gain_min | 0.01 | cheat |  |
| snd_gamevoicevolume | 1 | a | Game v.o. volume |
| snd_gamevolume | 1 | a | Game volume |
| snd_get_physics_surface_properties | cmd | cheat | Get physics surface properties for all the materials. |
| snd_headphone_eq | 1 | cl, a, clientcmd_can_execute | Select Headphone EQ Preset |
| snd_headphone_pan_exponent | cmd |  | Specifies the exponent for the pan xfade from phone to phone if the 'exp' pan law is being used. |
| snd_headphone_pan_radial_weight | cmd |  | Apply cos(angle) * weight before pan law |
| snd_list | 0 | cheat |  |
| snd_list_deferred_soundevents | cmd | cheat | List all current deferred load soundevents |
| snd_list_soundevents | cmd | cheat | List all available soundevents |
| snd_list_soundevents_by_stack | cmd | cheat | List all available soundevents using specified stack name |
| snd_mainmenu_music_break_time_max | 0 | cl, cheat | Maximum amount of time to pause between playing main menu music |
| snd_mainmenu_music_break_time_min | 0 | cl, cheat | Minimum amount of time to pause between playing main menu music |
| snd_mapobjective_volume | 0.434693 | cl, a, release | Volume of map objective music |
| snd_menumusic_volume | 0.440528 | cl, a, release | Volume of main menu music |
| snd_mixahead | 0.001 | a |  |
| snd_mixer_master_dsp | 1 | cheat |  |
| snd_mixer_master_level | 1 | cheat |  |
| snd_music_selection | 1 | cl, a | Tracking rotating music for players with no music packs equipped. |
| snd_musicvolume | 0 | a | Music volume |
| snd_mute_losefocus | true | a |  |
| snd_mute_mvp_music_live_players | false | cl, a, release | If set, MVP music is muted if players from both teams are still alive. |
| snd_mvp_volume | 0.2 | cl, a, release | Volume of round MVP music |
| snd_new_visualize | false | sv, cheat | Displays soundevent name played at it's 3d position |
| snd_occlusion_bounces | 1 | rep, cheat |  |
| snd_occlusion_debug | false | sv, cl, rep, cheat |  |
| snd_occlusion_min_wall_thickness | 4 | rep, cheat |  |
| snd_occlusion_rays | 4 | rep, cheat |  |
| snd_op_test_convar | 720 | cheat |  |
| snd_opvar_set_point_debug | false | sv, cl, rep, cheat |  |
| snd_othermusic_volume | 0.2 | cl, a, release | Volume of unclassified music |
| snd_print_activetracks | cmd | cheat | List all active tracks |
| snd_print_arrangements | cmd | cheat | List all available sequence arrangments |
| snd_print_current_mixer_mixgroup | cmd |  | Get data related to mix group matching string |
| snd_print_samplers | cmd | cheat | List all available samplers |
| snd_print_sequences | cmd | cheat | List all available midi sequences |
| snd_rear_headphone_position | cmd |  | Specifies the position  (in degrees) of the virtual rear left/right headphones. |
| snd_rear_stereo_speaker_position | cmd |  | Specifies the position (in degrees) of the virtual rear left/right speakers. |
| snd_rear_surround_speaker_position | cmd |  | Specifies the position (in degrees) of the virtual rear left/right speakers. |
| snd_refdb | 60 | cheat | Reference dB at snd_refdist |
| snd_refdist | 36 | cheat | Reference distance for snd_refdb |
| snd_remove_all_soundevents | cmd | cheat | Remove all soundevents |
| snd_remove_soundevent | cmd | cheat | Remove the specified soundevent |
| snd_report_verbose_error | false | cheat | If set to 1, report more error found when playing sounds. |
| snd_roundaction_volume | 0.380879 | cl, a, release | Volume of round action music |
| snd_roundend_volume | 0.386714 | cl, a, release | Volume of round end music |
| snd_roundstart_volume | 0.410053 | cl, a, release | Volume of round start music |
| snd_samplers_play_note | cmd | cheat | Play a note from a specified sampler |
| snd_samplers_stop_note | cmd | cheat | Stop a note from a specified sampler |
| snd_sequence_set_track_bpm | cmd | cheat | Sets the tempo of the specified track |
| snd_sequence_set_track_transpose | cmd | cheat | Sets the transposition of the specified track |
| snd_sequence_stop_all_tracks | cmd | cheat | Stops all currently playing sequences |
| snd_sequence_stop_track | cmd | cheat | Stops the specified track |
| snd_sequencer_show_bpm | false | cheat |  |
| snd_sequencer_show_events | false | cheat |  |
| snd_sequencer_show_quantize_queue | false | cheat |  |
| snd_set_physics_surface_properties | cmd | cheat | Set physics surface properties for materials. Usage |
| snd_setmixer | cmd | cheat | Set named Mixgroup of current mixer to mix vol, mute, solo. |
| snd_setmixlayer | cmd | cheat | Set named Mixgroup of named mix layer to mix vol, mute, solo. |
| snd_showclassname | 0 | cheat |  |
| snd_showstart | 0 | cheat |  |
| snd_side_surround_speaker_position | cmd |  | Specifies the position (in degrees) of the virtual rear left/right speakers. |
| snd_sos_block_global_stack | false | cheat |  |
| snd_sos_block_stop_global_stack | true | cheat |  |
| snd_sos_calc_angle_debug | false | rep, cheat |  |
| snd_sos_cl_soundevent_pause_last | cmd | cl | Test |
| snd_sos_cl_soundevent_start | cmd | cl | Test |
| snd_sos_cl_soundevent_stop_last | cmd | cl | Test |
| snd_sos_cl_soundevent_unpause_last | cmd | cl | Test |
| snd_sos_flush_operators | cmd | cheat | Flush and re-parse the sound operator system |
| snd_sos_get_operator_field_info | cmd | cheat | Currently gets info for a single operator field |
| snd_sos_ingame_debug | false | cheat |  |
| snd_sos_list_operator_updates | false | cheat |  |
| snd_sos_opvar_debug | false | cheat |  |
| snd_sos_pause_soundevent | cmd | cheat | Pause the specified soundevent in the list |
| snd_sos_pause_system | false | cheat |  |
| snd_sos_print_class_sizes | cmd | cheat | Prints the sizes of relevant sos classes. |
| snd_sos_print_field_name_strings | cmd | cheat | Prints a list of currently cached field name strings |
| snd_sos_print_field_references | false | cheat |  |
| snd_sos_print_full_field_info | false | cheat |  |
| snd_sos_print_groups | cmd | cheat | Prints the current state of the groups system |
| snd_sos_print_operator_stack | cmd | cheat | Prints a master list of currently exposed variables |
| snd_sos_print_operator_stack_opeator | cmd | cheat | Prints an operator from a stack |
| snd_sos_print_operator_stacks | cmd | cheat | Prints a list of currently available stacks |
| snd_sos_print_operators | cmd | cheat | Prints a list of currently available operators |
| snd_sos_print_stack_exec_list | cmd | cheat | Prints the current stack execution list |
| snd_sos_print_strings | cmd | cheat | Prints a list of currently cached strings |
| snd_sos_print_tool_properties | cmd | cheat | Prints the current state of tool properties. |
| snd_sos_resolve_execute_operator | cmd | cheat | Resolve the inputs and execute one specified operator from a specified stack |
| snd_sos_set_operator_field | cmd | cheat | Currently sets a single float operator field |
| snd_sos_set_operator_field_by_guid | cmd | cheat | Currently sets a single float operator field |
| snd_sos_show_block_debug | false | cheat | Spew data about the list of block entries. |
| snd_sos_show_operator_event_and_stack | true | cheat |  |
| snd_sos_show_operator_event_filter | 0 | cheat |  |
| snd_sos_show_operator_field_filter | 0 | cheat |  |
| snd_sos_show_operator_init | false | cheat |  |
| snd_sos_show_operator_not_executing | true | cheat |  |
| snd_sos_show_operator_operator_filter | 0 | cheat |  |
| snd_sos_show_operator_pause_entry | false | cheat |  |
| snd_sos_show_operator_shutdown | false | cheat |  |
| snd_sos_show_operator_stop_entry | false | cheat |  |
| snd_sos_show_operator_updates | false | cheat |  |
| snd_sos_show_opvar_updates | false | cheat |  |
| snd_sos_show_opvar_updates_filter | 0 | cheat |  |
| snd_sos_show_queuetotrack | false | cheat |  |
| snd_sos_show_soundevent_param_overwrite | false | cheat |  |
| snd_sos_show_soundevent_start | false | cheat |  |
| snd_sos_soundevent_filter | 0 | cheat |  |
| snd_sos_soundevent_profile | cmd | cheat | Dump a record of current soundevents and profile data |
| snd_sos_start_soundevent | cmd | cheat | Starts a specified soundevent |
| snd_sos_start_soundevent_at_pos | cmd | cheat | Starts a specified soundevent at the given position |
| snd_sos_stop_all_soundevents | cmd | cheat | Stops all soundevents currently on the execution list |
| snd_sos_stop_soundevent_guid | cmd | cheat | Stops a specified soundevent |
| snd_sos_stop_soundevent_index | cmd | cheat | Stops a specified soundevent |
| snd_sos_sv_soundevent_pause_last | cmd | sv | Test |
| snd_sos_sv_soundevent_start | cmd | sv | Test |
| snd_sos_sv_soundevent_stop_last | cmd | sv | Test |
| snd_sos_sv_soundevent_unpause_last | cmd | sv | Test |
| snd_sos_sv_test_gender | cmd | sv | Test |
| snd_sos_test_soundmessage | cmd | cheat | test |
| snd_sos_unpause_soundevent | cmd | cheat | UnPause the first soundevent in the list |
| snd_sound_areas_debug | false | cl, rep, cheat |  |
| snd_sound_areas_debug_interval | 0.2 | cl, rep, cheat |  |
| snd_soundevent_clear_deferred | cmd | cheat | Clear the list of deferred soundevents for loading. |
| snd_soundmixer_flush | cmd |  | Reload soundmixers.txt file. |
| snd_soundmixer_list_mix_groups | cmd |  | List all mix groups to dev console. |
| snd_soundmixer_list_mix_layers | cmd |  | List all mix layers to dev console. |
| snd_soundmixer_list_mixers | cmd |  | List all mixers to dev console. |
| snd_soundmixer_set_trigger_factor | cmd | cheat | Set named mix layer / mix group, trigger amount. |
| snd_soundmixer_setmixlayer_amount | cmd | cheat | Set named mix layer mix amount. |
| snd_steamaudio_ambisonics_order | 1 | cheat | The amount of directional detail in the simulated by Steam Audio. |
| snd_steamaudio_enable_pathing | false | cheat | This variable is checked by soundstack to globally enabling pathing for audio processing. |
| snd_steamaudio_export_scene | cmd | cheat | Exports scene currently used by Steam Audio as a phononscene file. |
| snd_steamaudio_halton_sequence | cmd | cheat | Generate Halton Sequence for a given order and number of samples. |
| snd_steamaudio_ir_duration | 2 | cheat | The time delay between a sound being emitted and the last audible reflection in Steam Audio. |
| snd_steamaudio_load_pathing_data | true | cheat | If set, baked pathing data is loaded. Steam Audio Hammer entities can successfully use pathing in this case. |
| snd_steamaudio_load_reverb_data | true | cheat | If set, baked reverb data is loaded. Reset it to zero during an format changes of baked data until all data is updated. |
| snd_steamaudio_max_convolution_sources | 4 | cheat | The maximum number of simultaneous sources that can be modeled by Steam Audio. |
| snd_steamaudio_max_occlusion_samples | 64 | cheat | The maximum number of rays that can be traced for volumetric occlusion by Steam Audio. |
| snd_steamaudio_num_bounces | 128 | cheat | The maximum number of times any ray can bounce when using Steam Audio. |
| snd_steamaudio_num_diffuse_samples | 2048 | cheat | The number of directions considered for ray bounce by Steam Audio. |
| snd_steamaudio_num_rays | 65536 | cheat | The number of rays to trace for reflection modeling by Steam Audio. |
| snd_steamaudio_num_threads | 2 | cheat | Sets the number of threads used for realtime reflection by Steam Audio. |
| snd_steamaudio_pathing_enablevalidationvis | false | cheat | Enable visualization for pathing validation. |
| snd_steamaudio_pathing_enablevis | false | cheat | Enable visualization for pathing. |
| snd_steamaudio_probes_nearby | cmd |  | Load all the probes from a file and log the nearby probes within the radius. |
| snd_stereo_speaker_pan_exponent | cmd |  | Specifies the exponent for the pan xfade from speaker to speaker if the 'exp' pan law is being used. |
| snd_stereo_speaker_pan_radial_weight | cmd |  | Apply cos(angle) * weight before pan law |
| snd_surround_speaker_pan_exponent | cmd |  | Specifies the exponent for the pan xfade from speaker to speaker if the 'exp' pan law is being used. |
| snd_surround_speaker_pan_radial_weight | cmd |  | Apply cos(angle) * weight before pan law |
| snd_tensecondwarning_volume | 0.2 | cl, a, release | Volume of ten-second warning music |
| snd_toolvolume | 1 | a | Volume of sounds in tools (e.g. Hammer, SFM) |
| snd_vmidi_flush | cmd | cheat | Purge and reload all vmidi data and files. |
| snd_vmix_override_mix_decay_time | -1 | cheat | If set > 0, overrides how long the decay time is on all mix graphs (in seconds). |
| snd_vmix_show_input_updates | false | cheat | If set to 1, show all incoming updates to vmix inputs. |
| snd_voipvolume | 1 | a | Voice volume |
| sndplaydelay | cmd |  |  |
| sound_device_override | 0 | a, release | ID of the sound device to use |
| soundinfo | cmd |  | Describe the current sound device with an active voice list. |
| soundlist | cmd |  | List all known sounds. |
| soundscape_debug | false | sv, cheat | When on, draws lines to all env_soundscape entities. Green lines show the active soundscape, red lines show soundscapes that aren't in range, and white lines show soundscapes that are in range, but not the active soundscape. |
| soundscape_dumpclient | cmd | cl, cheat | Dumps the client's soundscape data. |
| soundscape_fadetime | 3 | cl, cheat | Time to crossfade sound effects between soundscapes |
| soundscape_flush | cmd | sv | Flushes the server & client side soundscapes |
| soundscape_radius_debug | false | cl, cheat | Prints current volume of radius sounds |
| soundsysteminfo | cmd |  | Describe the current sound device without an active voice list. |
| spawn_group_activate | cmd | sv, cheat | Activate specified spawngroup. |
| spawn_group_list | cmd | sv, cheat | List all spawn groups |
| spawn_group_load | cmd | sv, cheat | Load named spawn group. |
| spawn_group_unload | cmd | sv, cheat | Unload named spawn group. |
| speaker_config | -1 | a |  |
| spec_centerchasecam | false | cl, a | Looks at the target player's center, instead of his eye position, in chase came mode |
| spec_dz_group_teams | true | cl, release | If set, will group players into their teams for spectating, if 0, spectating numbers will be the default individual players |
| spec_freeze_deathanim_time | 0.8 | sv, cl, rep, release | The time that the death cam will spend watching the player's ragdoll before going into the freeze death cam. |
| spec_freeze_time | 2 | sv, cl, rep, release | Time spend frozen in observer freeze cam. |
| spec_freeze_time_lock | 1 | sv, cl, rep, release | Time players are prevented from skipping the freeze cam |
| spec_freeze_traveltime | 0.3 | sv, cl, rep, release | Time taken to zoom in to frame a target in observer freeze cam. |
| spec_glow_decay_time | 2 | cl, release | Time to decay glow from 1.0 to spec_glow_silent_factor after spec_glow_full_time. |
| spec_glow_full_time | 1 | cl, release | Noisy players stay at full brightness for this long. |
| spec_glow_silent_factor | 0.6 | cl, release | Lurking player xray glow scaling. |
| spec_glow_spike_factor | 1.2 | cl, release | Noisy player xray glow scaling (pop when noise is made).  Make >1 to add a 'spike' to noise-making players |
| spec_glow_spike_time | 0 | cl, release | Time for noisy player glow 'spike' to show that they made noise very recently. |
| spec_hide_players | false | cl, release, clientcmd_can_execute | Toggle the visibility of scoreboard players. |
| spec_pos | cmd | cl | dump position and angles to the console |
| spec_replay_autostart | true | cl, a | Auto-start Killer Replay when available |
| spec_replay_bot | false | sv, release | Enable Spectator Hltv Replay when killed by bot |
| spec_replay_enable | 0 | rep, release | Enable Killer Replay, requires hltv server running (0 |
| spec_replay_leadup_time | 5.3438 | rep, release | Replay time in seconds before the highlighted event |
| spec_replay_message_time | 9.5 | rep, release | How long to show the message about Killer Replay after death. The best setting is a bit shorter than spec_replay_autostart_delay + spec_replay_leadup_time + spec_replay_winddown_time |
| spec_replay_on_death | false | rep, release | When > 0, sets the mode whereas players see delayed replay, and are segregated into a domain of chat and voice separate from the alive players |
| spec_replay_rate_base | 1 | rep, release | Base time scale of Killer Replay.Experimental. |
| spec_replay_rate_limit | 3 | rep, release | Minimum allowable pause between replay requests in seconds |
| spec_replay_round_delay | 0 | sv, release | Round can be delayed by this much due to someone watching a replay; must be at least 3-4 seconds, otherwise the last replay will always be interrupted by round start, assuming normal pause between round_end and round_start events (7 seconds) and freezecam delay (2 seconds) and 7.4 second full replay (5.4 second pre-death and ~2 seconds post-death) and replay in/out switching (up to a second) |
| spec_replay_winddown_time | 2 | sv, release | The trailing time, in seconds, of replay past the event, including fade-out |
| spec_show_xray | 1 | cl, a, release | If set to 1, you can see player outlines and name IDs through walls - who you can see depends on your team and mode |
| spec_usenumberkeys_nobinds | true | cl, a | If set to 1, map voting and spectator view use the raw number keys instead of the weapon binds (slot1, slot2, etc). |
| spec_xray_dropped_defusekits | false | cl, release | Whether to X-ray dropped defuse kits. |
| spec_xray_dropped_unoccluded | false | cl, release | Whether to always X-ray dropped c4 and defuse kits. |
| spew_fonts | cmd |  | Spew information about font manager fonts |
| splitscreen_mode | 0 | a |  |
| +spray_menu | cmd | cl |  |
| ss_add | cmd |  | Adds a splitscreen user. |
| ss_remove | cmd |  | Removes a splitscreen user. |
| startdemos | cmd |  | Play demos in demo sequence. |
| startmovie | cmd | norecord | Start recording movie frames. |
| stats | cmd |  | Prints server performance variables |
| stats_print | cmd |  | Prints out perf statistics to the console, clears perf history |
| stats_print_gpu | cmd |  | Prints out GPU perf statistics to the console.  Requires stats_display > 0, and stats_collect_gpu = true.  Optional argument of CSV filename |
| status | cmd |  | Print connection status |
| status_json | cmd |  | Print status in JSON format |
| steam_controller_haptics | true | cl, release |  |
| stop | cmd |  | Finish recording demo. |
| stopdemos | cmd |  | Stop looping demos (current demo will complete). |
| stopsound | cmd | cheat |  |
| stopsoundscape | cmd | cl, cheat | Stops all soundscape processing and fades current looping sounds |
| subclass_change | cmd | sv, cheat, vconsole_fuzzy | Changes the subclass of the given entity.  Arguments |
| subclass_create | cmd | sv, cheat, vconsole_fuzzy | Creates an entity of the given subclass where the player is looking. |
| surfaceprop | cmd | sv, cheat | Reports the surface properties at the cursor |
| survival_check_num_possible_final_zone | cmd | sv | print out a number of all possible final zone |
| sv_accelerate | 5.5 | sv, cl, nf, rep, release |  |
| sv_accelerate_debug_speed | false | sv, cl, nf, rep, release |  |
| sv_accelerate_use_weapon_speed | true | sv, cl, nf, rep, release |  |
| sv_air_max_horizontal_parachute_speed | 240 | sv, cl, rep, release |  |
| sv_air_max_wishspeed | 30 | sv, cl, rep, release |  |
| sv_air_pushaway_dist | 0 | sv, cl, rep, release |  |
| sv_airaccelerate | 12 | sv, cl, nf, rep, release |  |
| sv_airaccelerate_parachute | 2.6 | sv, cl, rep, release |  |
| sv_airaccelerate_rappel | 2.2 | sv, cl, rep, release |  |
| sv_allchat | true | sv, nf, release | Players can receive all other players' text chat, no death restrictions |
| sv_allow_thirdperson | false | sv, cl, rep, release | Allows the server set players in third person mode without the client slamming it back (if cheats are on, all clients can set thirdperson without this convar being set) |
| sv_allow_votes | true | sv, release | Allow voting? |
| sv_alltalk | false | sv, nf, release | Players can hear all other players' voice communication, no team restrictions |
| sv_alternateticks | false | sp, release | If set, server only simulates entities on even numbered ticks. |
| sv_arms_race_vote_to_restart_disallowed_after | 0 | sv, rep, release | Arms Race gun level after which vote to restart is disallowed |
| sv_auto_adjust_bot_difficulty | true | sv, release | Adjust the difficulty of bots each round based on contribution score. |
| sv_auto_full_alltalk_during_warmup_half_end | false | sv, release | When enabled will automatically turn on full all talk mode in warmup, at halftime and at the end of the match |
| sv_autobunnyhopping | true | sv, cl, rep, release | Players automatically re-jump while holding jump button |
| sv_autobuyammo | false | sv, nf, rep, release | Enable automatic ammo purchase when inside buy zones during buy periods |
| sv_autoexec_mapname_cfg | false | sv, release | Execute a mapname cfg file on the server automatically in custom game modes that require it. |
| sv_banid_enabled | true | release | Whether server supports banid command |
| sv_bot_buy_decoy_weight | 1 | sv, release | Given a bot will buy a grenade, controls the odds of the grenade type. Proportional to all other sv_bot_buy_*_weight convars. |
| sv_bot_buy_flash_weight | 1 | sv, release | Given a bot will buy a grenade, controls the odds of the grenade type. Proportional to all other sv_bot_buy_*_weight convars. |
| sv_bot_buy_grenade_chance | 33 | sv, release | Chance bots will buy a grenade with leftover money (after prim, sec and armor). Input as percent (0-100.0) |
| sv_bot_buy_hegrenade_weight | 6 | sv, release | Given a bot will buy a grenade, controls the odds of the grenade type. Proportional to all other sv_bot_buy_*_weight convars. |
| sv_bot_buy_molotov_weight | 1 | sv, release | Given a bot will buy a grenade, controls the odds of the grenade type. Proportional to all other sv_bot_buy_*_weight convars. |
| sv_bot_buy_smoke_weight | 1 | sv, release | Given a bot will buy a grenade, controls the odds of the grenade type. Proportional to all other sv_bot_buy_*_weight convars. |
| sv_bots_get_easier_each_win | 0 | sv, release | If > 0, some # of bots will lower thier difficulty each time they win. The argument defines how many will lower their difficulty each time. |
| sv_bots_get_harder_after_each_wave | 0 | sv, release | If > 0, some # of bots will raise thier difficulty each time CTs beat a Guardian wave. The argument defines how many will raise their difficulty each time |
| sv_bounce | 0 | sv, cl, nf, rep, release | Bounce multiplier for when physically simulated objects collide with other objects. |
| sv_breachcharge_arm_delay | 0.3 | sv, release |  |
| sv_breachcharge_delay_max | 0.8 | sv, release |  |
| sv_breachcharge_delay_min | 0 | sv, release |  |
| sv_breachcharge_distance_max | 1200 | sv, release |  |
| sv_breachcharge_distance_min | 600 | sv, release |  |
| sv_breachcharge_fuse_max | 1 | sv, release |  |
| sv_breachcharge_fuse_min | 0.7 | sv, release |  |
| sv_bumpmine_arm_delay | 0.3 | sv, release |  |
| sv_bumpmine_detonate_delay | 0.25 | sv, release |  |
| sv_buy_status_override | -1 | sv, rep, release | Override for buy status map info. 0 = everyone can buy, 1 = ct only, 2 = t only 3 = nobody |
| sv_chat_proximity | -1 | sv, cl, rep, release |  |
| sv_cheats | true | nf, rep, release | Allow cheats on server |
| sv_clientrates | cmd |  | Show client rates. |
| sv_clockcorrection_msecs | 30 | sv, release | The server tries to keep each player's m_nTickBase withing this many msecs of the server absolute tickcount |
| sv_cluster | 0 | release | Data center cluster this server lives in. |
| sv_competitive_minspec | true | sv, cl, nf, rep, release | Enable to force certain client convars to minimum/maximum values to help prevent competitive advantages. |
| sv_cs_dump_econ_item_stringtable | cmd | sv | sv_cs_dump_econ_item_stringtable |
| sv_cs_player_speed_has_hostage | 200 | sv, cl, rep, release |  |
| sv_damage_print_enable | 1 | sv, cl, rep, release | 0 |
| sv_deadtalk | true | sv, cl, nf, rep, release | Dead players can speak (voice, text) to the living |
| sv_debug_overlays_bandwidth | 65536 | release | Broadcast server debug overlays traffic |
| sv_debug_overlays_broadcast | false | nf, cheat, release | Broadcast server debug overlays |
| sv_dev_simulate_gcdown | cmd | sv | <state> Turn on/off simulated GC communications failure (GC is down in a way that we know it is down) |
| sv_disable_immunity_alpha | false | sv, cl, rep, release | If set, clients won't slam the player model render settings each frame for immunity [mod authors use this] |
| sv_disable_observer_interpolation | false | sv, cl, rep, release | Disallow interpolating between observer targets on this server. |
| sv_disable_radar | 0 | sv, cl, rep, release | 0 |
| sv_disconnected_player_data_hold_time | 60 | sv, cl, rep, release | Duration, in seconds, to hold onto the data of disconnected players, for scoreboard display. |
| sv_dz_cash_bundle_size | 50 | sv, rep, release | Size of a cash bundle |
| sv_dz_cash_mega_bundle_size | 13 | sv, rep, release | Size of a mega cash bundle |
| sv_dz_contractkill_reward | 10 | sv, rep, release | Cash bundles to award for a successful contract kill |
| sv_dz_enable_respawn | true | sv, cl, rep, release |  |
| sv_dz_enable_respawn_solos | false | sv, cl, rep, release |  |
| sv_dz_exploration_payment_amount | 2 | sv, rep, release | Number of cash bundles to award for exploring a new sector |
| sv_dz_exploration_payment_amount_bonus | 2 | sv, rep, release | Number of BONUS cash bundles to award for exploring (if the player has the item/upgrade) |
| sv_dz_force_zone | false | sv, cl, rep, cheat |  |
| sv_dz_hostage_rescue_reward | 18 | sv, cl, rep, release | Number of cash bundles to award for rescuing a hostage |
| sv_dz_jointeam_allowed | false | sv, release | Whether non-server admins are allowed to use the dz_jointeam command |
| sv_dz_parachute_reuse | true | sv, rep, release |  |
| sv_dz_paradrop | cmd | sv |  |
| sv_dz_player_max_health | 120 | sv, release |  |
| sv_dz_player_spawn_armor | 0 | sv, release |  |
| sv_dz_player_spawn_health | 120 | sv, release |  |
| sv_dz_reset_danger_zone | cmd | sv |  |
| sv_dz_show_enemy_name_scope_range | 800 | sv, release |  |
| sv_dz_squad_wipe_reward | 2 | sv, cl, rep, release | Number of cash bundles to award for eliminating a squad |
| sv_dz_team_count | 1 | sv, cl, rep, release | Max players allowed per team |
| sv_dz_warmup_tablet | true | sv, release |  |
| sv_dz_zone_bombdrop_money_reward | 15 | sv, cl, rep, release | How many money stacks players are rewarded each danger zone wave |
| sv_dz_zone_bombdrop_money_reward_bonus | 5 | sv, cl, rep, release | How many bonus money stacks players are rewarded each danger zone wave when they have the bonus item |
| sv_dz_zone_damage | true | sv, cheat, release |  |
| sv_dz_zone_hex_radius | 2200 | sv, cl, rep, release |  |
| sv_enable_alternate_baselines | 1 | release | Allow alternate baseline system, set to 2 for debugging spew. |
| sv_enable_delta_packing | true | release | When enabled, this allows for entity packing to use the property changes for building up the data. This is many times faster, but can be disabled for error checking. |
| sv_enablebunnyhopping | true | sv, cl, rep, release | Allow player speed to exceed maximum running speed |
| sv_ent_showonlyhitbox | -1 | sv, cheat |  |
| sv_ents_write_alarm | 0 | release | Print callstack every time CNetworkGameServerBase |
| sv_exojump_jumpbonus_forward | 0.4 | sv, cl, rep, release | ExoJump forwards velocity bonus when duck jumping |
| sv_exojump_jumpbonus_up | 0.58 | sv, cl, rep, release | ExoJump upwards bonus when holding the jump button |
| sv_exostaminajumpcost | 0.04 | sv, cl, rep, release | Stamina penalty for jumping with exo legs |
| sv_exostaminalandcost | 0.015 | sv, cl, rep, release | Stamina penalty for landing with exo legs |
| sv_extract_ammo_from_dropped_weapons | false | sv, cl, rep, release |  |
| sv_fade_player_visibility_farz | false | sv, cl, rep, release |  |
| sv_falldamage_exojump_multiplier | 0.4 | sv, cl, rep, release | ExoJump fall damage multiplier |
| sv_falldamage_scale | 1 | sv, cl, rep, release |  |
| sv_falldamage_to_below_player_multiplier | 1 | sv, cl, rep, release | Scale damage when distributed across two players |
| sv_falldamage_to_below_player_ratio | 0 | sv, cl, rep, release | Landing on a another player's head gives them this ratio of the damage. |
| sv_force_reflections | false | sv, cl, rep, release |  |
| sv_friction | 5.2 | sv, cl, nf, rep, release | World friction. |
| sv_full_alltalk | false | sv, cl, rep, release | Any player (including Spectator team) can speak to any other player |
| sv_fullupdate | cmd |  | Force a full update for all clients. |
| sv_game_mode_convars | cmd | sv | Display the values of the convars for the current game_mode. |
| sv_game_mode_flags | 0 | sv, release | Dedicated server game mode flags to run |
| sv_gameinstructor_disable | false | sv, cl, rep, release | Force all clients to disable their game instructors. |
| sv_ggprogressive_autosniper_first | true | sv, release | Should auto snipers go first or regular snipers? |
| sv_ggprogressive_shotgun_last | true | sv, release | Should auto snipers go first or regular snipers? |
| sv_ghostcap | true | sv, release | Shows on player join if a player has the copy tables cheat enabled. |
| sv_grassburn | false | sv, cl, rep, release |  |
| sv_gravity | 800 | sv, cl, nf, rep, release | World gravity. |
| sv_grenade_trajectory_prac_pipreview | false | sv, cl, rep, release | Shows grenade trajectory practice picture-in-picture preview. |
| sv_grenade_trajectory_prac_trailtime | 0 | sv, cl, rep, release | Shows grenade trajectory practice visualization for this number of seconds. |
| sv_grenade_trajectory_time_spectator | 4 | sv, cl, rep, release | Length of time grenade trajectory remains visible as a spectator. |
| sv_guardian_extra_equipment_ct | 0 | sv, release | Extra starting equipment for CT players in guardian modes |
| sv_guardian_extra_equipment_t | 0 | sv, release | Extra starting equipment for Terrorist players in guardian modes |
| sv_guardian_health_refresh_per_wave | 50 | sv, release | Health given to survivors per wave in guardian mode. |
| sv_guardian_heavy_all | false | sv, release |  |
| sv_guardian_heavy_count | 0 | sv, release |  |
| sv_guardian_max_wave_for_heavy | 0 | sv, release |  |
| sv_guardian_min_wave_for_heavy | 0 | sv, release |  |
| sv_guardian_refresh_ammo_for_items_on_waves | 0 | sv, release | List of additional weapons to refill ammo on waves. |
| sv_guardian_reset_c4_every_wave | false | sv, release |  |
| sv_guardian_respawn_health | 50 | sv, release | Starting health of guardian players when respawned. |
| sv_guardian_spawn_health_ct | 100 | sv, release | Starting health in guardian modes. |
| sv_guardian_spawn_health_t | 100 | sv, release | Starting health in guardian modes. |
| sv_guardian_starting_equipment_humans | 0 | sv, release | Extra starting equipment for human players in guardian modes |
| sv_health_approach_enabled | true | sv, rep, release |  |
| sv_health_approach_speed | 10 | sv, rep, release |  |
| sv_hegrenade_damage_multiplier | 1 | sv, rep, release |  |
| sv_hegrenade_radius_multiplier | 1 | sv, rep, release |  |
| sv_hibernate_postgame_delay | 5 | release | # of seconds to wait after final client leaves before hibernating. |
| sv_hibernate_when_empty | true | release | Puts the server into extremely low CPU usage mode when no clients connected |
| sv_hide_roundtime_until_seconds | 0 | sv, cl, rep, release |  |
| sv_highlight_distance | 500 | sv, cl, rep, release |  |
| sv_highlight_duration | 3.5 | sv, cl, rep, release |  |
| sv_holiday_mode | 0 | sv, cl, rep, release | 0 = OFF, 1 = Halloween, 2 = Winter |
| sv_ignoregrenaderadio | false | sv, release | Turn off Fire in the hole messages |
| sv_infinite_ammo | 0 | sv, cl, rep, cheat, release | Player's active weapon will never run out of ammo |
| sv_invites_only_mainmenu | false | sv, cl, rep, release | If turned on, will ignore all invites when user is playing a match |
| sv_jump_impulse | 301.993 | sv, cl, rep, release | Initial upward velocity for player jumps; sqrt(2*gravity*height). |
| sv_jump_impulse_exojump_multiplier | 1.05 | sv, cl, rep, release | ExoJump impulse multiplier |
| sv_kick_ban_duration | 15 | sv, cl, nf, rep, release | How long should a kick ban from the server should last (in minutes) |
| sv_kick_players_with_cooldown | 1 | sv, rep, release | (0 |
| sv_knife_attack_extend_from_player_aabb | 0 | sv, cl, rep, release |  |
| sv_ladder_scale_speed | 0.78 | sv, cl, rep, release | Scale top speed on ladders |
| sv_ladder_slack_z_mult | 0.026 | sv, cl, rep, cheat | Difference in Z increases toward the middle of the slack ladder. |
| sv_lagcompensationforcerestore | true | sv, cheat | Don't test validity of a lag comp restore, just do it. |
| sv_lan | false | release | Server is a lan server ( no heartbeat, no authentication, no non-class C addresses ) |
| sv_lightquery_debug | false | sv, cheat |  |
| sv_load_forced_client_names_file | cmd | sv, release | Loads a file containing SteamID64 names for clients |
| sv_load_random_client_names_file | cmd | sv, release | Loads a file containing random name words for clients |
| sv_log_onefile | false | a | Log server information to only one file. |
| sv_logbans | false | a | Log server bans in the server logs. |
| sv_logblocks | false | release | If true when log when a query is blocked (can cause very large log files) |
| sv_logecho | true | a | Echo log information to the console. |
| sv_logfile | false | a | Log server information in the log file. |
| sv_logflush | false | a | Flush the log file to disk on each write (slow). |
| sv_logsdir | logs | a | Folder in the game directory where server logs will be stored. |
| sv_mapvetopickvote_maps | de_anubis,de_inferno,de_mirage,de_vertigo,de_overpass,de_nuke,de_ancient | sv, release | Which maps are used for map veto pick sequence |
| sv_mapvetopickvote_phase_duration | [1 | 12][2 | 25][5 |
| sv_matchend_drops_enabled | true | sv, release | Rewards gameplay time is always accumulated for players, but drops at the end of the match can be prevented |
| sv_matchpause_auto_5v5 | false | sv, cl, rep, release | When enabled will automatically pause the match at next freeze time if less than 5 players are connected on each team. |
| sv_max_allowed_net_graph | 1 | sv, cl, nf, rep, release | Determines max allowed net_graph value for clients. |
| sv_max_queries_sec | 3 | release | Maximum queries per second to respond to from a single IP address. |
| sv_max_queries_sec_global | 60 | release | Maximum queries per second to respond to from anywhere. |
| sv_max_queries_window | 30 | release | Window over which to average queries per second averages. |
| sv_maxrate | 0 | rep, release | Max bandwidth rate allowed on server, 0 == unlimited |
| sv_maxspeed | 320 | sv, cl, nf, rep, release |  |
| sv_maxunlag | 1 | sv, release | Maximum lag compensation in seconds |
| sv_maxupdaterate | 60 | sv, cl, rep, release | Maximum updates per second that the server will allow |
| sv_maxvelocity | 3500 | sv, cl, rep, release | Maximum speed any ballistically moving object is allowed to attain per axis. |
| sv_memlimit | 0 | cheat, release | If set, whenever a game ends, if the total memory used by the server is greater than this # of megabytes, the server will exit. |
| sv_metaduplication | cmd | cheat | Check serializer meta for duplication, add verbose to command for full spew |
| sv_min_jump_landing_sound | 260 | sv, cl, rep, release |  |
| sv_minrate | 98304 | rep, release | Min bandwidth rate allowed on server, 0 == unlimited |
| sv_minupdaterate | 10 | sv, cl, rep, release | Minimum updates per second that the server will allow |
| sv_networkvar_perfieldtracking | true | release | Track individual field offset changes, rather than a single dirty flag for the whole entity. |
| sv_networkvar_validate | false | release | Validate each StateChanged against known offsets. |
| sv_noclipaccelerate | 5 | sv, cl, a, nf, rep |  |
| sv_noclipduringpause | false | sv, cl, rep, cheat | If cheats are enabled, then you can noclip with the game paused (for doing screenshots, etc.). |
| sv_noclipfriction | 4 | sv, cl, a, nf, rep | Friction during noclip move. |
| sv_noclipspeed | 1200 | sv, cl, a, nf, rep |  |
| sv_outofammo_indicator | false | sv, cl, rep, release |  |
| sv_packstats | cmd | release | Show entity packing stats, pass 'clear' as argument to reset counts. |
| sv_parallel_packentities | 2 | release | Set to 1 to use threaded snapshot sending on listen servers, 2 for dedicated servers. |
| sv_parallel_sendsnapshot | 2 | release | Set to 1 to use threading snapshot sending on listen servers, 2 for dedicated servers. |
| sv_party_mode | false | sv, cl, rep, release | Party!! |
| sv_password | 0 | prot, nf, norecord, release | Server password for entry into multiplayer games |
| sv_pausable | 0 | release | Is the server pausable. |
| sv_pause_on_console_open | false | a | 1 = Pause the game when pressing ~ to open the console. CTRL+~ opens the console without pause. |
| sv_phys_debug_callback_entities | false | sv, cheat | Print all entities that get touch callbacks. Each entity is printed only once. |
| sv_phys_enabled | true | sv, cheat | Enable all physics simulation |
| sv_phys_sleep_enable | true | sv, cheat | Enable sleeping for dynamic physics bodies. |
| sv_phys_stop_at_collision | 0 | sv, cheat |  |
| sv_player_parachute_velocity | -200 | sv, rep, release |  |
| sv_prime_accounts_only | false | sv, release | When this setting is enabled only prime users can connect to this game server. |
| sv_pure | cmd |  | Show user data. |
| sv_pure_kick_clients | true | release | If set to 1, the server will kick clients with mismatching files. Otherwise, it will issue a warning to the client. |
| sv_pure_trace | 0 | release | If set to 1, the server will print a message whenever a client is verifying a CRC for a file. |
| sv_pushaway_hostage_force | 20000 | sv, rep, cheat | How hard the hostage is pushed away from physics objects (falls off with inverse square of distance). |
| sv_pushaway_max_hostage_force | 1000 | sv, rep, cheat | Maximum of how hard the hostage is pushed away from physics objects. |
| sv_pvs_max_distance | 0 | rep, release | if set, adds a maximum range to PVS/PAS checks |
| sv_querycache_stats | cmd | sv | Display status of the query cache (client only) |
| sv_radio_throttle_window | 10 | sv, release | The number of seconds before radio command tokens refresh. |
| sv_ragdoll_lru_debug | false | sv, rep, cheat |  |
| sv_record_item_time_data | false | sv, release | Turn on recording of per player item time data into the server log. |
| sv_regeneration_force_on | false | sv, cheat | Cheat to test regenerative health systems |
| sv_region | -1 | release | The region of the world to report this server in. |
| sv_rethrow_last_grenade | cmd | sv, cheat | Emit the last grenade thrown on the server. |
| sv_search_key | 0 | release |  |
| sv_search_team_key | public | release | When initiating team search, set this key to match with known opponents team |
| sv_server_graphic1 | 0 | sv, cl, rep, release | A 360x60 (<16kb) image file in /csgo/ that will be displayed to spectators. |
| sv_server_graphic2 | 0 | sv, cl, rep, release | A 220x45 (<16kb) image file in /csgo/ that will be displayed to spectators. |
| sv_server_verify_blood_on_player | true | sv, cl, rep, cheat |  |
| sv_shield_bash_damage_to_nonplayer | 30 | sv, cl, rep, release |  |
| sv_shield_bash_damage_to_players | 90 | sv, cl, rep, release |  |
| sv_shield_explosive_damage_cap | 99 | sv, cl, rep, release |  |
| sv_shield_explosive_damage_crouch_bonus | 10 | sv, cl, rep, release |  |
| sv_shield_explosive_damage_mindist | 30 | sv, cl, rep, release |  |
| sv_shield_explosive_damage_mult | 4 | sv, cl, rep, release |  |
| sv_shield_explosive_damage_scale | 0.5 | sv, cl, rep, release |  |
| sv_shield_hitpoints | 850 | sv, cl, rep, release |  |
| sv_show_ragdoll_playernames | false | cl, rep, release |  |
| sv_show_team_equipment_force_on | false | sv, cl, rep, release | Force on if not prohibited |
| sv_show_team_equipment_prohibit | false | sv, cl, nf, rep, release | Determines whether +cl_show_team_equipment is prohibited. |
| sv_show_voip_indicator_for_enemies | false | sv, rep, release | Makes it so the voip icon is shown over enemies as well as allies when they are talking |
| sv_showbullethits | 0 | sv, cl, rep, release | 1=show hits and near misses, 2=show hits only |
| sv_showhitregistration | 0 | sv, cl, rep, cheat | Display lag_compensated hitboxes. 0 = off, 1 = server only, 2 = client only, 3 = both server and client |
| sv_showimpacts | 0 | sv, cl, rep, release | Shows client (red) and server (blue) bullet impact point (1=both, 2=client-only, 3=server-only) |
| sv_showimpacts_penetration | 0 | sv, cl, rep, release | Shows extra data when bullets penetrate. (use sv_showimpacts_time to increase time shown) |
| sv_showimpacts_time | 4 | sv, cl, rep, release | Duration bullet impact indicators remain before disappearing |
| sv_showtags | cmd |  | Describe current gametags. |
| sv_shutdown | cmd |  | Sets the server to shutdown when all games have completed |
| sv_skel_constraints_enable | false | rep, cheat |  |
| sv_skirmish_id | 0 | sv, cl, rep, release | Dedicated server skirmish id to run |
| sv_skyname | sky_urb01 | sv, cl, a, rep | Current name of the skybox texture |
| sv_snapshot_unlimited | false | rep, release | For debugging, don't throw away old snapshots so that if you break in debugger (on remote client or server) it won't require an uncompressed update to resume.  You may run out of memory of course... |
| sv_soundscape_printdebuginfo | cmd | sv, cheat | print soundscapes |
| sv_spawn_afk_bomb_drop_time | 15 | sv, rep, release | Players that have never moved since they spawned will drop the bomb after this amount of time. |
| sv_spawn_rappel_min_duration | 8 | sv, rep, release |  |
| sv_spawn_rappel_min_duration_with_chute | 2.5 | sv, rep, release |  |
| sv_spec_hear | 1 | sv, cl, nf, rep, release | Determines who spectators can hear |
| sv_spec_use_tournament_content_standards | false | sv, cl, rep, release |  |
| sv_specaccelerate | 5 | sv, cl, a, nf, rep |  |
| sv_specnoclip | true | sv, cl, a, nf, rep |  |
| sv_specspeed | 1200 | sv, cl, a, nf, rep |  |
| sv_spewmeta | cmd | cheat | Spew serializer meta |
| sv_staminajumpcost | 0.08 | sv, cl, rep, release | Stamina penalty for jumping |
| sv_staminalandcost | 0.05 | sv, cl, rep, release | Stamina penalty for landing |
| sv_staminamax | 80 | sv, cl, rep, release | Maximum stamina penalty |
| sv_staminarecoveryrate | 60 | sv, cl, rep, release | Rate at which stamina recovers (units/sec) |
| sv_steamgroup | 0 | nf, release | The ID of the steam group that this server belongs to. You can find your group's ID on the admin profile page in the steam community. |
| sv_steamgroup_exclusive | false | release | If set, only members of Steam group will be able to join the server when it's empty, public people will be able to join the server only if it has players. |
| sv_stopspeed | 80 | sv, cl, nf, rep, release | Minimum stopping speed when on ground. |
| sv_stressbots | false | release | If set to 1, the server calculates data and fills packets to bots. Used for perf testing. |
| sv_tablet_show_path_to_nearest_resq | false | sv, cl, rep, release |  |
| sv_tags | 0 | nf, release | Server tags. Used to provide extra information to clients when they're browsing for servers. Separate tags with a comma. |
| sv_talk_after_dying_time | 0 | sv, cl, rep, release | The number of seconds a player can continue talking after dying as if they were still alive |
| sv_talk_enemy_dead | false | sv, cl, rep, release | Dead players can hear all dead enemy communication (voice, chat) |
| sv_talk_enemy_living | false | sv, cl, rep, release | Living players can hear all living enemy communication (voice, chat) |
| sv_teamid_overhead | true | sv, cl, nf, rep, release | Shows teamID over player's heads.  0 = off, 1 = on |
| sv_teamid_overhead_always_prohibit | false | sv, cl, nf, rep, release | Determines whether cl_teamid_overhead_always is prohibited. |
| sv_teamid_overhead_maxdist | 0 | sv, cl, rep, release | If >0, server will override cl_teamid_overhead_maxdist |
| sv_teamid_overhead_maxdist_spec | 0 | sv, cl, rep, release | If >0, server will override cl_teamid_overhead_maxdist_spec |
| sv_timebetweenducks | 0.4 | sv, cl, rep, release | Minimum time before recognizing consecutive duck key |
| sv_tripwirefire_trace_length | 180 | sv, release |  |
| sv_turning_inaccuracy_angle_min | 4 | sv, cl, rep, cheat, release |  |
| sv_turning_inaccuracy_decay | 0.8 | sv, cl, rep, cheat, release |  |
| sv_turning_inaccuracy_enabled | false | sv, cl, rep, cheat, release |  |
| sv_unlockedchapters | 1 | a | Highest unlocked game chapter. |
| sv_update_animgraph_movement_in_finish | true | sv, cl, rep, cheat | Whether we should update animgraph movement in FinishMove. |
| sv_usercmd_queue_spew_threshold | 10 | sv, release | Spew warning if command queue has grown above this many backlogged commands. |
| sv_versus_screen_scene_id | 0 | sv, release | Determines which scene is used for the versus screen. |
| sv_visiblemaxplayers | -1 | release | Overrides the max players reported to prospective clients |
| sv_voice_proximity | -1 | sv, cl, rep, release |  |
| sv_voicecodec | vaudio_speex | release | Specifies which voice codec DLL to use in a game. Set to the name of the DLL without the extension. |
| sv_voiceenable | true | a, nf, release |  |
| sv_vote_allow_in_warmup | false | sv, release | Allow voting during warmup? |
| sv_vote_allow_spectators | false | sv, release | Allow spectators to initiate votes? |
| sv_vote_command_delay | 2 | sv, release | How long after a vote passes until the action happens |
| sv_vote_count_spectator_votes | false | sv, release | Allow spectators to vote on issues? |
| sv_vote_creation_timer | 120 | sv, release | How often someone can individually call a vote. |
| sv_vote_disallow_kick_on_match_point | false | sv, release | Disallow vote kicking on the match point round. |
| sv_vote_failure_timer | 300 | sv, release | A vote that fails cannot be re-submitted for this long |
| sv_vote_issue_kick_allowed | true | sv, nf, rep, release | Can people hold votes to kick players from the server? |
| sv_vote_issue_loadbackup_allowed | true | sv, nf, rep, release | Can people hold votes to load match from backup? |
| sv_vote_issue_loadbackup_spec_authoritative | false | sv, release | When enabled, admins load match from backup without players vote |
| sv_vote_issue_loadbackup_spec_only | false | sv, nf, rep, release | When enabled, only admins load match from backup |
| sv_vote_issue_loadbackup_spec_safe | true | sv, release | When enabled, admins load match from backup in safe time of the round only |
| sv_vote_issue_pause_match_spec_only | false | sv, nf, rep, release | When enabled, only admins start technical pause |
| sv_vote_issue_restart_game_allowed | false | sv, release | Can people hold votes to restart the game? |
| sv_vote_kick_ban_duration | 15 | sv, nf, rep, release | How long should a kick vote ban someone from the server? (in minutes) |
| sv_vote_quorum_ratio | 0.501 | sv, release | The minimum ratio of players needed to vote on an issue to resolve it. |
| sv_vote_timer_duration | 15 | sv, release | How long to allow voting on an issue |
| sv_vote_to_changelevel_before_match_point | false | sv, rep, release | Restricts vote to change level to rounds prior to match point (default 0, vote is never disallowed) |
| sv_warmup_to_freezetime_delay | 4 | sv, cl, rep, release | Delay between end of warmup and start of match. |
| sv_watchtransmit | -2 | sv, release | Watch NetworkStateChanged info for this entity index. |
| sv_wateraccelerate | 10 | sv, cl, nf, rep, release |  |
| sv_waterfriction | 1 | sv, cl, nf, rep, release |  |
| sv_weapon_encumbrance_per_item | 0.85 | sv, cl, rep, release |  |
| sv_weapon_encumbrance_scale | 0 | sv, cl, rep, release |  |
| sv_weapon_require_use_grace_period | 1 | sv, release |  |
| sv_workshop_allow_other_maps | true | sv, release | When hosting a workshop collection, users can play other workshop map on this server when it is empty and then mapcycle into this server collection. |
| sys_info | cmd |  | Print system information to the console |
| sys_minidumpspewlines | 2000 | release | Lines of crash dump console spew to keep. |
| tablet_c4_dist_max | 3000 | sv, cl, rep, release |  |
| tablet_c4_dist_min | 400 | sv, cl, rep, release |  |
| teammenu | cmd | cl, server_can_execute | Show team selection window |
| telemetry_message | cmd | sv, cheat | Place a message in the telemetry timeline |
| telemetry_toggle_timespan | cmd | sv, cheat | Starts/stops a timespan with an ever increasing name. |
| tenfoot_match | cmd | cl, linked | [prefix] |
| tenfoot_pickle_dictionaries | cmd | cl, linked | compiles daisy wheel input dictionaries to more performant form |
| tenfoot_pickle_single_dictionary | cmd | cl, linked | [language] compiles one daisy wheel input dictionary |
| tenfoot_text_hotspots | cmd | cl, linked | find text autosuggest hot spots |
| Test_Checkpoint | cmd |  | Indicate to a test script that a checkpoint has been reached |
| Test_CreateEntity | cmd | sv, cheat |  |
| test_dispatcheffect | cmd | sv, cheat | Test a clientside dispatch effect.  Usage |
| Test_EHandle | cmd | sv, cheat |  |
| test_entity_blocker | cmd | sv, cheat | Test command that drops an entity blocker out in front of the player. |
| Test_ExitProcess | cmd | cheat | Test_ExitProcess <exit code> - immediately kill the process. |
| test_list_entities | cmd | sv, cheat | test-list entities |
| Test_Loop | cmd |  | Test_Loop <loop name> - loop back to the specified loop start point unconditionally. |
| Test_LoopCount | cmd |  | Test_LoopCount <loop name> <count> - loop back to the specified loop start point the specified # of times. |
| Test_LoopForNumSeconds | cmd |  | Test_LoopForNumSeconds <loop name> <time> - loop back to the specified start point for the specified # of seconds. |
| Test_RandomChance | cmd |  | Test_RandomChance <percent chance, 0-100> <token1> <token2...> - Roll the dice and maybe run the command following the percentage chance. |
| Test_RandomPlayerPosition | cmd | sv, cheat |  |
| Test_StartLoop | cmd |  | Test_StartLoop <loop name> - Denote the start of a loop. Really just defines a named point you can jump to. |
| Test_StartScript | cmd |  | Start a test script running.. |
| think_limit | 10 | sv, cl, rep, release | Maximum think time in milliseconds, warning is printed if this is exceeded. |
| thirdperson | cmd | cl, cheat, execute_per_tick | Switch to thirdperson camera. |
| thirdperson_lockcamera | false | cl, rep, cheat |  |
| thirdperson_mayamode | cmd | cl, cheat | Switch to thirdperson Maya-like camera controls. |
| thirdpersonshoulder | cmd | cl | Switch to thirdperson-shoulder camera. |
| timedemo | cmd |  | Play a demo and report performance info. |
| timedemoquit | cmd |  | Play a demo, report performance info, and then exit |
| timeleft | cmd | sv | prints the time remaining in the match |
| timeout_ct_start | cmd | sv |  |
| timeout_terrorist_start | cmd | sv |  |
| toggle | cmd | norecord | Toggles specified convar value on and off. |
| toggleconsole | cmd | norecord | Show/hide the console. |
| tr_do_reduce | true | rep, cheat |  |
| tr_epsilon_t_junction | 0.01 | rep, cheat |  |
| tr_max_acceptable_edge_length | 10000 | rep, cheat |  |
| tr_openedge_penalty | 10 | rep, cheat |  |
| traceattack | cmd | sv | traceattack damage hitgroup |
| trusted_launch | 0 | cl, a | Trusted launch status |
| tv_advertise_watchable | false | prot, nf, norecord, release | GOTV advertises the match as watchable via game UI, clients watching via UI will not need to type password |
| tv_allow_autorecording_index | -1 | sv, release | When >=0 restricts autorecording only to the specified TV index |
| tv_allow_camera_man_override | false | release | Allows cameraman_override to have effect. When this is set, the primary interactive caster will have all the relevant fields present in all network packets, in every snapshot. This allows the secondary cameraman (-interactivecaster that connects to a tv port) to override those fields some seconds later regardless of whether they changed originally or not. |
| tv_allow_camera_man_steamid | 0 | sv, release | Allows tournament production cameraman to run csgo.exe -interactivecaster on SteamID 7650123456XXX and be the camera man. |
| tv_allow_camera_man_steamid2 | 0 | sv, release | Allows tournament production tv cameraman to run csgo.exe -interactivecaster on SteamID 7650123456XXX and be the tv camera man. |
| tv_allow_static_shots | true | sv, release | Auto director uses fixed level cameras for shots |
| tv_autorecord | false | release | Automatically records all games as SourceTV demos. |
| tv_autoretry | true | release | Relay proxies retry connection after network timeout |
| tv_broadcast | false | release | Automatically broadcasts all games as GOTV demos through Steam. |
| tv_broadcast1 | false | release | Automatically broadcasts all games as GOTV[1] demos through Steam. |
| tv_broadcast_keyframe_interval | 3 | release | The frequency, in seconds, of sending keyframes and delta fragments to the broadcast relay server |
| tv_broadcast_keyframe_interval1 | 3 | release | The frequency, in seconds, of sending keyframes and delta fragments to the broadcast1 relay server |
| tv_broadcast_max_requests | 20 | release | Max number of broadcast http requests in flight. If there is a network issue, the requests may start piling up, degrading server performance. If more than the specified number of requests are in flight, the new requests are dropped. |
| tv_broadcast_max_requests1 | 20 | release | Max number of broadcast1 http requests in flight. If there is a network issue, the requests may start piling up, degrading server performance. If more than the specified number of requests are in flight, the new requests are dropped. |
| tv_broadcast_resend | cmd |  | resend broadcast data to broadcast relay |
| tv_broadcast_startup_resend_interval | 10 | release | The interval, in seconds, of re-sending startup data to the broadcast relay server (useful in case relay crashes, restarts or startup data http request fails) |
| tv_broadcast_status | cmd |  | Print out broadcast status |
| tv_broadcast_url | http | //localhost | 8080 |
| tv_broadcast_url1 | http | //localhost | 8080 |
| tv_chatgroupsize | 0 | release | Set the default chat group size |
| tv_chattimelimit | 0.2 | release | Limits spectators to chat only every n seconds |
| tv_clients | cmd |  | Shows list of connected SourceTV clients. |
| tv_debug | 0 | release | SourceTV debug info. |
| tv_delay | 105 | sv, release | SourceTV broadcast delay in seconds |
| tv_delaymapchange | true | sv, release | Delays map change until broadcast is complete |
| tv_deltacache | 2 | release | Enable delta entity bit stream cache |
| tv_dispatchmode | 1 | release | Dispatch clients to relay proxies |
| tv_enable | false | nf, release | Activates SourceTV on server. |
| tv_enable1 | false | nf, release | Activates SourceTV[1] on server. |
| tv_enable_delta_frames | true | release | Indicates whether or not the tv should use delta frames for storage of intermediate frames. This takes more CPU but significantly less memory. |
| tv_listen_voice_indices | 0 | cl, user | Bitfield of playerslots to listen to voice messages from when connected to SourceTV, default is none |
| tv_listen_voice_indices_h | 0 | cl, user | High 32 bits of bitfield of playerslots to listen to voice messages from when connected to SourceTV, default is none |
| tv_maxclients | 128 | release | Maximum client number on SourceTV server. |
| tv_maxclients_relayreserved | 0 | release | This number of relay client connections are reserved for SourceTV relays. |
| tv_maxrate | 0 | release | Max SourceTV spectator bandwidth rate allowed, 0 == unlimited |
| tv_mem | cmd |  | hltv memory statistics. Use with 'ent 10' (dump entity 10 memory usage) or 'top 8' (dump top 8 memory users) or 'class' CWorld (dump CWorld class) |
| tv_msg | cmd | sv | Send a screen message to all clients. |
| tv_name | SourceTV | release | SourceTV host name |
| tv_nochat | false | a, user | Don't receive chat messages from other SourceTV spectators |
| tv_overridemaster | false | release | Overrides the SourceTV master root address. |
| tv_password | 0 | prot, nf, norecord, release | SourceTV password for all clients |
| tv_playcast_delay_prediction | true | release |  |
| tv_playcast_delay_resync | 0 | release | To alleviate intermittent network connectivity problems, this is the number of seconds to wait before actually re-syncing the stream after failure |
| tv_playcast_retry_timeout | 12 | release | In case of intermittent network problems, how long should playcast retry fragment retrieval before resorting to resync |
| tv_port | 27020 | release | Host SourceTV port |
| tv_record | cmd |  | Starts SourceTV demo recording. |
| tv_relay | cmd |  | Connect to SourceTV server and relay broadcast. |
| tv_relaypassword | 0 | prot, nf, norecord, release | SourceTV password for relay proxies |
| tv_relayradio | false | sv, release | Relay team radio commands to TV |
| tv_relayvoice | true | release | Relay voice data |
| tv_retry | cmd |  | Reconnects the SourceTV relay proxy. |
| tv_show_allchat | true | sv, release |  |
| tv_snapshotrate | 20 | rep, release | Snapshots broadcast per second |
| tv_snapshotrate1 | 32 | release | Snapshots broadcast per second, GOTV[1] |
| tv_spectator_port_offset | 0 | cl, release |  |
| tv_status | cmd |  | Show SourceTV server status. |
| tv_stop | cmd |  | Stops the SourceTV broadcast. |
| tv_stoprecord | cmd |  | Stops SourceTV demo recording. |
| tv_time_remaining | cmd | sv, release | Print remaining tv broadcast time |
| tv_timeout | 20 | release | SourceTV connection timeout in seconds. |
| tv_title | SourceTV | release | Set title for SourceTV spectator UI |
| tv_transmitall | false | rep, release | Transmit all entities (not only director view) |
| ui_deepstats_radio_heat_figurine | 0 | cl, a, release |  |
| ui_deepstats_radio_heat_tab | 0 | cl, a, release |  |
| ui_deepstats_radio_heat_team | 0 | cl, a, release |  |
| ui_deepstats_toplevel_mode | 0 | cl, a, release |  |
| ui_inventorysettings_recently_acknowledged | 0 | cl, a, release |  |
| ui_lobby_draft_enabled | false | cl, release |  |
| ui_mainmenu_bkgnd_movie_94408AE3 | dust2 | cl, a, release | Main menu background movie |
| ui_nearbylobbies_filter3 | competitive | cl, a, release |  |
| ui_news_last_read_link | 0 | cl, a, release |  |
| ui_playsettings_custom_preset | mg_de_dust2 | cl, a, release |  |
| ui_playsettings_directchallengekey | SCA6R-G3PG-S23GT-VQ6Q | cl, a, release |  |
| ui_playsettings_flags_listen_casual | 0 | cl, a, release |  |
| ui_playsettings_flags_listen_competitive | 32 | cl, a, release |  |
| ui_playsettings_flags_listen_cooperative | 0 | cl, a, release |  |
| ui_playsettings_flags_listen_deathmatch | 32 | cl, a, release |  |
| ui_playsettings_flags_listen_scrimcomp2v2 | 0 | cl, a, release |  |
| ui_playsettings_flags_listen_skirmish | 0 | cl, a, release |  |
| ui_playsettings_flags_listen_survival | 0 | cl, a, release |  |
| ui_playsettings_flags_official_casual | 0 | cl, a, release |  |
| ui_playsettings_flags_official_competitive | 16 | cl, a, release |  |
| ui_playsettings_flags_official_cooperative | 0 | cl, a, release |  |
| ui_playsettings_flags_official_deathmatch | 32 | cl, a, release |  |
| ui_playsettings_flags_official_scrimcomp2v2 | 0 | cl, a, release |  |
| ui_playsettings_flags_official_skirmish | 0 | cl, a, release |  |
| ui_playsettings_flags_official_survival | 0 | cl, a, release |  |
| ui_playsettings_maps_listen_casual | mg_de_dust2 | cl, a, release |  |
| ui_playsettings_maps_listen_competitive | mg_de_dust2 | cl, a, release |  |
| ui_playsettings_maps_listen_deathmatch | mg_de_dust2 | cl, a, release |  |
| ui_playsettings_maps_listen_scrimcomp2v2 | mg_de_inferno | cl, a, release |  |
| ui_playsettings_maps_listen_skirmish | mg_skirmish_armsrace | cl, a, release |  |
| ui_playsettings_maps_official_casual | mg_dust247 | cl, a, release |  |
| ui_playsettings_maps_official_deathmatch | mg_dust247 | cl, a, release |  |
| ui_playsettings_maps_workshop | 0 | cl, a, release |  |
| ui_playsettings_mode_listen | competitive | cl, a, release |  |
| ui_playsettings_mode_official_v20 | competitive | cl, a, release |  |
| ui_playsettings_prime | 1 | cl, a, release |  |
| ui_playsettings_survival_solo | 0 | cl, a, release |  |
| ui_playsettings_warmup_map_name | de_mirage | cl, a, release |  |
| ui_popup_weaponupdate_version | 2303 | cl, a, release |  |
| ui_setting_advertiseforhire_auto | 1 | cl, a, release | Whether users will automatically advertise for invites (0 |
| ui_setting_advertiseforhire_auto_last | /competitive | cl, a, release | Which game mode users last used to advertise for invites |
| ui_show_subscription_alert | 0 | cl, a, release |  |
| ui_show_unlock_competitive_alert | 0 | cl, a, release |  |
| ui_steam_overlay_notification_position | bottomleft | cl, a | Steam overlay notification position |
| ui_steam_overlay_notification_position_horz | 0 | cl, a | Steam overlay notification position horizontal offset |
| ui_steam_overlay_notification_position_vert | 0 | cl, a | Steam overlay notification position vertical offset |
| ui_vanitysetting_loadoutslot_ct | melee | cl, a, release |  |
| ui_vanitysetting_loadoutslot_t | smg0 | cl, a, release |  |
| ui_vanitysetting_team | ct | cl, a, release |  |
| unbind | cmd | release | Unbind a key. |
| unbindall | cmd | release | Unbind all keys. |
| unpause | cmd |  | Clear the pause state of the server. |
| UpdateBinarySizes | cmd |  | Dumps the binary sizes to use for the game in loadaddress.vpc |
| url_execute | cmd | cl | Executes url-based commands, used for incoming commands from url-based launches when the game's already running. |
| users | cmd |  | Show user info for players on server. |
| vconsole_rcon_server_details | 0 | norecord, release, server_cant_query | when non-empty allows for easy vconsole connection to the dedicated server. |
| view_punch_decay | 18 | sv, cl, rep, cheat, release | Decay factor exponent for view punch |
| viewmodel_always_on | false | cl, cheat | Force the view model to draw, even when in 3rd person |
| viewmodel_fov | 60 | cl, a | Viewmodel FOV |
| viewmodel_offset_randomize | false | cl, cheat | randomly change viewmodel offsets to visualize range |
| viewmodel_offset_x | 1 | cl, a | viewmodel_offset_x |
| viewmodel_offset_y | 1 | cl, a | viewmodel_offset_y |
| viewmodel_offset_z | -1 | cl, a | viewmodel_offset_z |
| viewmodel_presetpos | 1 | cl, a | 1 |
| violence_ablood | true | a | Draw alien blood |
| violence_agibs | true | a | Show alien gib entities |
| violence_hblood | true | a | Draw human blood |
| violence_hgibs | true | a | Show human gib entities |
| vis_debug_currentcluster | cmd |  | Show the current cluster number |
| vis_debug_drawcluster | cmd |  | Add cluster # to visualization, (-1) to clear |
| vis_debug_dumpvisibleclusters | cmd |  | Show the list of visible clusters |
| vis_debug_find_los | cmd |  | Find or clear the vis LOS to here |
| vis_debug_lock | cmd |  | Lock vis LOS origin to current |
| vis_debug_record_start | cmd |  | Record a path to debug vis |
| vis_debug_record_stop | cmd |  | Record a path to debug vis |
| vis_debug_show | cmd |  | Show/hide the vis debug visualization |
| vis_debug_sphere | cmd |  | Draw clusters in a sphere of radius around the camera |
| vis_debug_sunclusters | cmd |  | Showing clusters for sun/csm rendering. Red (full sun csm & lighting), Orange (no viewmodel sun or csm), Green (no sun at all) |
| vis_debug_tracelos | cmd |  | Trace rays and check vis from the current camera |
| vis_force | false | sv, cheat |  |
| vismon_poll_frequency | 0.5 | sv, cheat |  |
| vismon_trace_limit | 12 | sv, cheat |  |
| vmem_dump | cmd |  | Dump memory stats to log. |
| vmix_debug_list | cmd |  | Debug dump the list of available vmix graphs |
| vmix_input | cmd | cheat | Set an input mix value |
| vmix_output | cmd | cheat | Dump main graph control output values |
| voice_always_sample_mic | false | a | For systems experiencing a hang/stall when using voice chat. |
| voice_loopback | false | user |  |
| voice_modenable | true | cl, a, clientcmd_can_execute | Enable/disable voice in this mod. |
| voice_modenable_toggle | cmd | cl | Toggle the voice_modenable convar. |
| voice_mute | cmd |  | Mute a specific Steam user |
| voice_player_speaking_delay_threshold | 0.5 | sv, cheat |  |
| voice_reset_mutelist | cmd |  | Reset all mute information for all players who were ever muted. |
| voice_scale | 0.6 | cl, a, release | Volume of incoming VOIP |
| voice_show_mute | cmd |  | Show whether current players are muted. |
| voice_test_log_send | false | release |  |
| voice_threshold | 4000 | cl, a |  |
| voice_unmute | cmd |  | Unmute a specific Steam user, or `all` to unmute all connected players. |
| voice_vox | 0 | cl, a, per_user | Voice chat uses a vox-style always on |
| volume | 1 | a | Sound volume |
| volume_fog_clipmap_update | 1 | cheat |  |
| volume_fog_clipmaps_enabled | true | cheat |  |
| volume_fog_disable | false | cheat |  |
| volume_fog_dither_scale | 3 | cheat |  |
| volume_fog_enable_jitter | true | cheat |  |
| volume_fog_enable_stereo | true | cheat |  |
| volume_fog_enlarge_frusta | 2 | cheat |  |
| volume_fog_show_volumes | false | cheat |  |
| vphys2_friction_factor | 1 | cheat | Change global friction factor |
| vphys2_restitution_factor | 1 | cheat | Change global restitution factor |
| vprof_dump_counters | cmd |  | Dump vprof counters to the console |
| vprof_generate_report | cmd |  | Generate a report to the console. |
| vprof_generate_report_budget | cmd |  | Generate a report to the console based on budget group. |
| vprof_generate_report_hierarchy | cmd |  | Generate a report to the console. |
| vprof_off | cmd |  | Disable vprof |
| vprof_on | cmd |  | Enable vprof |
| vprof_remote_start | cmd |  | Request a VProf data stream from the remote server (requires authentication) |
| vprof_remote_stop | cmd |  | Stop an existing remote VProf data request |
| vprof_reset | cmd |  | Reset the stats in VProf profiler |
| vprof_reset_peaks | cmd |  | Reset just the peak time in VProf profiler |
| vprof_vtrace | cmd |  | Toggle whether vprof data is sent to VTrace |
| vtune | cmd |  | Controls VTune's sampling. |
| weapon_accuracy_forcespread | 0 | sv, cl, rep, release | Force spread to the specified value. |
| weapon_accuracy_nospread | false | sv, cl, rep, release | Disable weapon inaccuracy spread |
| weapon_accuracy_reset_on_deploy | false | sv, cl, rep, cheat, release | On deploy, forcibly reset weapon accuracy to zero. |
| weapon_accuracy_shotgun_spread_patterns | true | sv, cl, rep, release |  |
| weapon_air_spread_scale | 1 | sv, cl, rep, release | Scale factor for jumping inaccuracy, set to 0 to make jumping accuracy equal to standing |
| weapon_auto_cleanup_time | 0 | sv, cl, rep, release | If set to non-zero, weapons will delete themselves after the specified time (in seconds) if no players are near. |
| weapon_debug_spread_gap | 0.67 | cl, cheat, per_user |  |
| weapon_debug_spread_show | 0 | cl, cheat, per_user | Enables display of weapon accuracy; 1 |
| weapon_max_before_cleanup | 0 | sv, cl, rep, release | If set to non-zero, will remove the oldest dropped weapon to maintain the specified number of dropped weapons in the world. |
| weapon_near_empty_sound | true | sv, cl, rep, cheat |  |
| weapon_reticle_knife_show | true | sv, cl, rep, release | When enabled will show knife reticle on clients. Used for game modes requiring target id display when holding a knife. |
| weapon_sound_falloff_multiplier | 1 | sv, cl, rep, cheat, release | Scaling for falloff of weapon firing sounds |
| world_dump_loaded_worlds | cmd |  | Dump all of the worlds that we know about |
| world_layer_list | cmd |  | List all world layers |
| world_layer_set_visible | cmd |  | Show or hide the specified world layer |
| writeid | cmd |  | Writes a list of permanently-banned user IDs to file. |
| writeip | cmd |  | Save the ban list to file. |
| writekeybindings | cmd | release | Saves current key bindings to disk. |
| zoom_sensitivity_ratio | 1 | cl, a, per_user | Additional mouse sensitivity scale factor applied when FOV is zoomed in. |
