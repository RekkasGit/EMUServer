## [22.11.0] - 04/29/2023

### Code

* Add check for owner in quest::pausetimer() ([#3304](https://github.com/EQEmu/Server/pull/3304)) @Kinglykrab 2023-04-23
* Add check for owner in quest::resumetimer() ([#3305](https://github.com/EQEmu/Server/pull/3305)) @Kinglykrab 2023-04-23
* Add initiator/owner checks to various methods in questmgr.cpp ([#3306](https://github.com/EQEmu/Server/pull/3306)) @Kinglykrab 2023-04-23
* Fix possible nullptr in quest::addloot() ([#3303](https://github.com/EQEmu/Server/pull/3303)) @Kinglykrab 2023-04-23
* Remove GetClassHPFactor() from zone/client_mods.cpp and zone/client.h ([#3313](https://github.com/EQEmu/Server/pull/3313)) @Kinglykrab 2023-04-30
* Remove GetClassHPFactor() from zone/merc.h ([#3314](https://github.com/EQEmu/Server/pull/3314)) @Kinglykrab 2023-04-30
* Remove pDontCastBefore_casting_spell from zone/npc.h ([#3311](https://github.com/EQEmu/Server/pull/3311)) @Kinglykrab 2023-04-30
* Remove unused code in zone/pets.cpp ([#3310](https://github.com/EQEmu/Server/pull/3310)) @Kinglykrab 2023-04-30
* Remove unused methods in zone/bot.cpp and zone/bot.h ([#3315](https://github.com/EQEmu/Server/pull/3315)) @Kinglykrab 2023-04-30
* Remove unused methods in zone/client.cpp and zone/client.h ([#3312](https://github.com/EQEmu/Server/pull/3312)) @Kinglykrab 2023-04-30
* Remove unused variable in common/crash.cpp ([#3308](https://github.com/EQEmu/Server/pull/3308)) @Kinglykrab 2023-04-30
* Use default ctor/dtor in oriented_bounding_box.h ([#3307](https://github.com/EQEmu/Server/pull/3307)) @Kinglykrab 2023-04-30
* quest::createBot() unnecessary check against nullptr ([#3302](https://github.com/EQEmu/Server/pull/3302)) @Kinglykrab 2023-04-23
* quest::setallskill() had always true condition. ([#3301](https://github.com/EQEmu/Server/pull/3301)) @Kinglykrab 2023-04-30

### Crash

* Fix UCS crash that occurs during log reloading ([#3324](https://github.com/EQEmu/Server/pull/3324)) @Akkadius 2023-04-30
* Fix possible dereference of nullptr in Client::CalcHPRegen ([#3316](https://github.com/EQEmu/Server/pull/3316)) @Aeadoin 2023-04-23
* Fix possible nullptr in Client::GetCharMaxLevelFromQGlobal() ([#3317](https://github.com/EQEmu/Server/pull/3317)) @Kinglykrab 2023-04-23

### Discord

* Add Discord webhook callback processing to world ([#3322](https://github.com/EQEmu/Server/pull/3322)) @Akkadius 2023-04-30

### Fixes

* Fix issue with NPCs no longer using some armor. ([#3318](https://github.com/EQEmu/Server/pull/3318)) @noudess 2023-04-24
* Fix issue with spawning Mercs ([#3327](https://github.com/EQEmu/Server/pull/3327)) @Aeadoin 2023-04-29
* Possible issues with SummonItem in Client::QuestReward() methods ([#3325](https://github.com/EQEmu/Server/pull/3325)) @Kinglykrab 2023-04-27

### Maps

* Update download with faster releases link ([#3321](https://github.com/EQEmu/Server/pull/3321)) @Akkadius 2023-04-30

### Messages

* Remove duplicate you have lost a level message ([#3323](https://github.com/EQEmu/Server/pull/3323)) @noudess 2023-04-25

### Quest API

* Add GetDefaultRaceSize() overloads to Perl/Lua ([#3320](https://github.com/EQEmu/Server/pull/3320)) @Kinglykrab 2023-04-30
* Add HasSpellEffect() to Perl/Lua ([#3319](https://github.com/EQEmu/Server/pull/3319)) @Kinglykrab 2023-04-30

## [22.10.0] - 04/22/2023

### Backups

* Fix database dump error reporting ([#3175](https://github.com/EQEmu/Server/pull/3175)) @Akkadius 2023-04-04

### Bots

* Cleanup GetBotTables() ([#3270](https://github.com/EQEmu/Server/pull/3270)) @Aeadoin 2023-04-06

### Cleanuo

* Only define row if we have results in Database::GetCharacterID() ([#3199](https://github.com/EQEmu/Server/pull/3199)) @Kinglykrab 2023-04-05

### Code

* Add missing breaks and returns in bonuses.cpp ([#3231](https://github.com/EQEmu/Server/pull/3231)) @Kinglykrab 2023-04-05
* Breaks in wrong spot in cases in spell_effects.cpp ([#3297](https://github.com/EQEmu/Server/pull/3297)) @Kinglykrab 2023-04-22
* Cleanup always true/false statements in shareddb.cpp ([#3189](https://github.com/EQEmu/Server/pull/3189)) @Kinglykrab 2023-04-05
* Cleanup cheap-to-copy reference to use value instead in eq_stream_ident.cpp/eq_stream_ident.h ([#3209](https://github.com/EQEmu/Server/pull/3209)) @Kinglykrab 2023-04-05
* Cleanup discord.cpp and discord_manager.cpp ([#3205](https://github.com/EQEmu/Server/pull/3205)) @Kinglykrab 2023-04-05
* Cleanup duplicate conditions in negate bonuses in bonuses.cpp ([#3226](https://github.com/EQEmu/Server/pull/3226)) @Kinglykrab 2023-04-05
* Cleanup item_instance.cpp always true statements and reassigning of same values ([#3187](https://github.com/EQEmu/Server/pull/3187)) @Kinglykrab 2023-04-05
* Cleanup macros in features.h ([#3185](https://github.com/EQEmu/Server/pull/3185)) @Kinglykrab 2023-04-05
* Cleanup string -> char* -> string conversions in bot_command.cpp ([#3252](https://github.com/EQEmu/Server/pull/3252)) @Kinglykrab 2023-04-05
* Cleanup unnecessary condition in Client::SendAlternateCurrencyValue() ([#3266](https://github.com/EQEmu/Server/pull/3266)) @Kinglykrab 2023-04-05
* Cleanup zone/zoning.cpp ([#3289](https://github.com/EQEmu/Server/pull/3289)) @Kinglykrab 2023-04-14
* Combine similar cases in Client::InitInnates() ([#3260](https://github.com/EQEmu/Server/pull/3260)) @Kinglykrab 2023-04-05
* Convert equipable_slot_list to std::vector from std::list in bot_command.cpp ([#3253](https://github.com/EQEmu/Server/pull/3253)) @Kinglykrab 2023-04-05
* Delete embxs.cpp/embxs.h ([#3284](https://github.com/EQEmu/Server/pull/3284)) @Kinglykrab 2023-04-14
* Delete unused strings in bot_command.cpp ([#3251](https://github.com/EQEmu/Server/pull/3251)) @Kinglykrab 2023-04-05
* Fix GetLastName() length check in Client::SendWindow() ([#3263](https://github.com/EQEmu/Server/pull/3263)) @Kinglykrab 2023-04-05
* Fix always false conditions in Client::IncStats() ([#3256](https://github.com/EQEmu/Server/pull/3256)) @Kinglykrab 2023-04-05
* Fix check for !this in Client::SendHPUpdateMarquee() ([#3257](https://github.com/EQEmu/Server/pull/3257)) @Kinglykrab 2023-04-05
* Fix filter condition in attack.cpp ([#3218](https://github.com/EQEmu/Server/pull/3218)) @Kinglykrab 2023-04-05
* Fix ornamentation augment icons in inspect requests ([#3264](https://github.com/EQEmu/Server/pull/3264)) @Kinglykrab 2023-04-05
* Fix possible nullptr inst in GetSharedBank() ([#3190](https://github.com/EQEmu/Server/pull/3190)) @Kinglykrab 2023-04-08
* Fix possible overflows in Client::AddPlatinum() and Client::TakePlatinum() ([#3255](https://github.com/EQEmu/Server/pull/3255)) @Kinglykrab 2023-04-05
* Fix shared_tasks.cpp/shared_tasks.cpp variable named same as class member ([#3192](https://github.com/EQEmu/Server/pull/3192)) @Kinglykrab 2023-04-05
* Fix skill_used being used as boolean in Mob::CommonDamage() ([#3220](https://github.com/EQEmu/Server/pull/3220)) @Kinglykrab 2023-04-05
* Identical conditions right beside each other in aa.cpp ([#3213](https://github.com/EQEmu/Server/pull/3213)) @Kinglykrab 2023-04-05
* Move unreachable code in ApplySpellsBonuses() ([#3229](https://github.com/EQEmu/Server/pull/3229)) @Kinglykrab 2023-04-05
* Move variable definition to more relevant scope in DatabaseDumpService::Dump() ([#3200](https://github.com/EQEmu/Server/pull/3200)) @Kinglykrab 2023-04-05
* Multiple cases with same outcome in GetDiscordPayloadFromEvent() ([#3184](https://github.com/EQEmu/Server/pull/3184)) @Kinglykrab 2023-04-05
* Remove ExportVarComplex() from embparser.cpp/embparser.h ([#3282](https://github.com/EQEmu/Server/pull/3282)) @Kinglykrab 2023-04-14
* Remove GetQGlobal() from qglobals.cpp/qglobals.h ([#3285](https://github.com/EQEmu/Server/pull/3285)) @Kinglykrab 2023-04-14
* Remove IsFullHP from mob.cpp/mob.h ([#3277](https://github.com/EQEmu/Server/pull/3277)) @Kinglykrab 2023-04-14
* Remove IsMeleeDmg() from skills.cpp/skills.h ([#3279](https://github.com/EQEmu/Server/pull/3279)) @Kinglykrab 2023-04-14
* Remove _GetMovementSpeed() from mob.h ([#3276](https://github.com/EQEmu/Server/pull/3276)) @Kinglykrab 2023-04-14
* Remove always true condition in Strings::Commify() ([#3193](https://github.com/EQEmu/Server/pull/3193)) @Kinglykrab 2023-04-05
* Remove always true conditions and unreachable code in Client::SendMercPersonalInfo() ([#3258](https://github.com/EQEmu/Server/pull/3258)) @Kinglykrab 2023-04-05
* Remove always true statement in say_link.cpp ([#3188](https://github.com/EQEmu/Server/pull/3188)) @Kinglykrab 2023-04-05
* Remove always true statements in task_client_state.cpp ([#3292](https://github.com/EQEmu/Server/pull/3292)) @Kinglykrab 2023-04-14
* Remove always true/false conditions from bot.cpp ([#3237](https://github.com/EQEmu/Server/pull/3237)) @Kinglykrab 2023-04-05
* Remove bool return from GetSharedPlatinum() ([#3191](https://github.com/EQEmu/Server/pull/3191)) @Kinglykrab 2023-04-05
* Remove extra assignment of current_endurance in Client ctor ([#3261](https://github.com/EQEmu/Server/pull/3261)) @Kinglykrab 2023-04-05
* Remove extraneous check for NegateAttacks in SE_NegateAttacks ([#3228](https://github.com/EQEmu/Server/pull/3228)) @Kinglykrab 2023-04-05
* Remove extraneous parentheses around math in Mob::ApplySpellsBonuses() ([#3227](https://github.com/EQEmu/Server/pull/3227)) @Kinglykrab 2023-04-05
* Remove getd(), geti(), InUse(), lasterr(), my_get_sv(), and VarExists() in embperl.cpp/embperl.h ([#3283](https://github.com/EQEmu/Server/pull/3283)) @Kinglykrab 2023-04-15
* Remove item_timers from questmgr.cpp/questmgr.h ([#3286](https://github.com/EQEmu/Server/pull/3286)) @Kinglykrab 2023-04-14
* Remove pendinggroup from mob.h ([#3278](https://github.com/EQEmu/Server/pull/3278)) @Kinglykrab 2023-04-14
* Remove position_same_update_count from client.cpp/client.h ([#3280](https://github.com/EQEmu/Server/pull/3280)) @Kinglykrab 2023-04-14
* Remove unnecessary break in while loop in Mob::AddToHateList() ([#3219](https://github.com/EQEmu/Server/pull/3219)) @Kinglykrab 2023-04-05
* Remove unnecessary check for IsStackable() in DeleteItem() ([#3186](https://github.com/EQEmu/Server/pull/3186)) @Kinglykrab 2023-04-05
* Remove unnecessary condition and cleanup variable name in tasks.cpp ([#3293](https://github.com/EQEmu/Server/pull/3293)) @Kinglykrab 2023-04-14
* Remove unnecessary conditions in Client::Consume() ([#3265](https://github.com/EQEmu/Server/pull/3265)) @Kinglykrab 2023-04-05
* Remove unnecessary conditions in Client::FilteredMessageCheck() ([#3262](https://github.com/EQEmu/Server/pull/3262)) @Kinglykrab 2023-04-05
* Remove unnecessary conditions in Client::SendFactionMessage() ([#3267](https://github.com/EQEmu/Server/pull/3267)) @Kinglykrab 2023-04-05
* Remove unnecessary setting of reuse variable in Bot::DoClassAttacks() ([#3233](https://github.com/EQEmu/Server/pull/3233)) @Kinglykrab 2023-04-05
* Remove unused SetConfigFile in common/eqemu_config.h ([#3208](https://github.com/EQEmu/Server/pull/3208)) @Kinglykrab 2023-04-05
* Remove unused code in eq_packet.cpp/eq_packet.h ([#3183](https://github.com/EQEmu/Server/pull/3183)) @Kinglykrab 2023-04-05
* Remove unused ctor and use default dtor in xtargetautohaters.h ([#3290](https://github.com/EQEmu/Server/pull/3290)) @Kinglykrab 2023-04-14
* Remove unused macros in common/types.h ([#3194](https://github.com/EQEmu/Server/pull/3194)) @Kinglykrab 2023-04-05
* Remove unused variable in Database::CopyCharacter() ([#3197](https://github.com/EQEmu/Server/pull/3197)) @Kinglykrab 2023-04-05
* Remove unused variables and use reference in task_manager.cpp ([#3291](https://github.com/EQEmu/Server/pull/3291)) @Kinglykrab 2023-04-14
* SE_AttackSpeed3 effect_value is always less than 0 ([#3222](https://github.com/EQEmu/Server/pull/3222)) @Kinglykrab 2023-04-05
* SE_StrikeThrough and SE_StrikeThrough2 are the same in bonuses.cpp ([#3223](https://github.com/EQEmu/Server/pull/3223)) @Kinglykrab 2023-04-05
* Set bonuses to use spell ID instead of boolean ([#3230](https://github.com/EQEmu/Server/pull/3230)) @Kinglykrab 2023-04-05
* Use .clear() and .empty() instead of comparing to empty string or setting to empty string in CheckDatabaseConvertPPBlob() ([#3201](https://github.com/EQEmu/Server/pull/3201)) @Kinglykrab 2023-04-05
* Use .clear() instead of setting string to empty in eqemu_command_handler.cpp ([#3195](https://github.com/EQEmu/Server/pull/3195)) @Kinglykrab 2023-04-05
* Use .empty() in Client::ScribeSpells() and Client::LearnDisciplines() ([#3259](https://github.com/EQEmu/Server/pull/3259)) @Kinglykrab 2023-04-05
* Use constant reference and check for empty string properly in dbcore.cpp ([#3203](https://github.com/EQEmu/Server/pull/3203)) @Kinglykrab 2023-04-05
* Use default ctor instead of an empty ctor. ([#3206](https://github.com/EQEmu/Server/pull/3206)) @Kinglykrab 2023-04-05
* Use default dtor instead of empty dtor for EQTime in eqtime.cpp/eqtime.h ([#3210](https://github.com/EQEmu/Server/pull/3210)) @Kinglykrab 2023-04-05
* Use variable for c->GetTarget() instead of calling multiple times in bot_command.cpp ([#3254](https://github.com/EQEmu/Server/pull/3254)) @Kinglykrab 2023-04-05
* Use variable for character instead of a loop ([#3268](https://github.com/EQEmu/Server/pull/3268)) @Kinglykrab 2023-04-05
* Utilize .empty() instead of checking for an empty string in Database::ReserveName() ([#3198](https://github.com/EQEmu/Server/pull/3198)) @Kinglykrab 2023-04-05
* Utilize IsTaunting(), SetPetPower(), SetPetType(), and SetTaunting() ([#3275](https://github.com/EQEmu/Server/pull/3275)) @Kinglykrab 2023-04-15
* Validate for nullptrs in bot.cpp ([#3232](https://github.com/EQEmu/Server/pull/3232)) @Kinglykrab 2023-04-05
* other is always defined in these cases in attack.cpp ([#3217](https://github.com/EQEmu/Server/pull/3217)) @Kinglykrab 2023-04-05
* results variable is assigned but never used in SaveCharacterCreate() ([#3180](https://github.com/EQEmu/Server/pull/3180)) @Kinglykrab 2023-04-05

### Crash

* Add additional raid integrity checks on Bot Spawn. ([#3295](https://github.com/EQEmu/Server/pull/3295)) @Aeadoin 2023-04-16
* Fix crash with uninitialized item instance, and Bot timeout ([#3296](https://github.com/EQEmu/Server/pull/3296)) @Aeadoin 2023-04-15
* Resolve crash due to uninitialized pointer. ([#3271](https://github.com/EQEmu/Server/pull/3271)) @Aeadoin 2023-04-08

### Feature

* Make ornamentations work with any augment type ([#3281](https://github.com/EQEmu/Server/pull/3281)) @Kinglykrab 2023-04-16

### Fixes

* Camping was causing player to leave raid, causing unexpected behavior ([#3299](https://github.com/EQEmu/Server/pull/3299)) @Aeadoin 2023-04-22
* Resolve loading of inventory ([#3272](https://github.com/EQEmu/Server/pull/3272)) @Aeadoin 2023-04-08

### Quest API

* Add ApplySpellRaid() and SetSpellDurationRaid() to Bots in Perl/Lua ([#3274](https://github.com/EQEmu/Server/pull/3274)) @Kinglykrab 2023-04-09
* Add GetBuffSpellIDs() to Perl/Lua ([#3273](https://github.com/EQEmu/Server/pull/3273)) @Kinglykrab 2023-04-09
* Fix LDoN Methods in Perl/Lua ([#3287](https://github.com/EQEmu/Server/pull/3287)) @Kinglykrab 2023-04-10

### Rules

* Optional summoning when already in melee range ([#3204](https://github.com/EQEmu/Server/pull/3204)) @trentdm 2023-04-08

### Telnet

* Telnet encoding fix ([#3269](https://github.com/EQEmu/Server/pull/3269)) @Akkadius 2023-04-05

## [22.9.1] - 04/03/2023 

### Code

* Add client pointer validation to Zone::GetClosestZonePoint() ([#3173](https://github.com/EQEmu/Server/pull/3173)) @Kinglykrab 2023-04-01
* Change level to bot_level in Bot::DoClassAttacks() to not overlap member variable ([#3239](https://github.com/EQEmu/Server/pull/3239)) @Kinglykrab 2023-04-03
* Cleanup unnecessary string -> char* -> string conversions in eqemu_config.cpp ([#3207](https://github.com/EQEmu/Server/pull/3207)) @Kinglykrab 2023-04-03
* Cleanup uses of insert/push_back when a temp object is used. ([#3170](https://github.com/EQEmu/Server/pull/3170)) @Aeadoin 2023-04-03
* Cleanup variable names in Bot::AddSpellToBotList() ([#3248](https://github.com/EQEmu/Server/pull/3248)) @Kinglykrab 2023-04-03
* Explicitly cast to float for more precision in Bot::GenerateBastHitPoints() ([#3238](https://github.com/EQEmu/Server/pull/3238)) @Kinglykrab 2023-04-03
* Fix SEResist array settings duplicate code ([#3225](https://github.com/EQEmu/Server/pull/3225)) @Kinglykrab 2023-04-03
* Fix loop and code duplication for SE_ProcOnKillShot ([#3224](https://github.com/EQEmu/Server/pull/3224)) @Kinglykrab 2023-04-03
* Fix possible dereferencing of invalid iterator in constants ([#3181](https://github.com/EQEmu/Server/pull/3181)) @Kinglykrab 2023-04-03
* Fix typo where itembonuses should have been used instead of spellbonuses ([#3221](https://github.com/EQEmu/Server/pull/3221)) @Kinglykrab 2023-04-03
* Further bot.cpp nullptr checks ([#3240](https://github.com/EQEmu/Server/pull/3240)) @Kinglykrab 2023-04-03
* Move cases in Bot::AICastSpell() ([#3247](https://github.com/EQEmu/Server/pull/3247)) @Kinglykrab 2023-04-03
* Multiple cases same outcome and set skip variable to same value ([#3216](https://github.com/EQEmu/Server/pull/3216)) @Kinglykrab 2023-04-03
* Multiple cases with same outcome in GetGMSayColorFromCategory() ([#3182](https://github.com/EQEmu/Server/pull/3182)) @Kinglykrab 2023-04-03
* Remove extraneous loottable_id setting in WakeTheDead in aa.cpp ([#3215](https://github.com/EQEmu/Server/pull/3215)) @Kinglykrab 2023-04-03
* Remove possible dereferenced nullptrs in bot.cpp ([#3241](https://github.com/EQEmu/Server/pull/3241)) @Kinglykrab 2023-04-03
* Remove unnecessary >= 0 checks for procs in botspellsai.cpp ([#3242](https://github.com/EQEmu/Server/pull/3242)) @Kinglykrab 2023-04-03
* Remove unnecessary botCaster check in Bot::GetDebuffBotSpell() ([#3246](https://github.com/EQEmu/Server/pull/3246)) @Kinglykrab 2023-04-03
* Remove unnecessary group validation in Bot::Death() ([#3235](https://github.com/EQEmu/Server/pull/3235)) @Kinglykrab 2023-04-03
* Remove unnecessary hpr checks in Bot::BotCastHeal() ([#3245](https://github.com/EQEmu/Server/pull/3245)) @Kinglykrab 2023-04-03
* Remove unnecessary setting of spell_type_index in Bot::GetChanceToCastBySpellType() ([#3243](https://github.com/EQEmu/Server/pull/3243)) @Kinglykrab 2023-04-03
* Remove unnecessary skill_to_use check in Bot::DoClassAttacks() ([#3236](https://github.com/EQEmu/Server/pull/3236)) @Kinglykrab 2023-04-03
* Remove unnecessary spell_list validation check in botspellsai.cpp ([#3244](https://github.com/EQEmu/Server/pull/3244)) @Kinglykrab 2023-04-03
* Remove unnecessary validation check in Zone::ClearBlockedSpells() ([#3172](https://github.com/EQEmu/Server/pull/3172)) @Kinglykrab 2023-04-01
* Remove unused Includes under zone files ([#3162](https://github.com/EQEmu/Server/pull/3162)) @Aeadoin 2023-04-02
* Remove unused query variable in Database::DeleteInstance() ([#3202](https://github.com/EQEmu/Server/pull/3202)) @Kinglykrab 2023-04-03
* Unconditional return in for loop in GetRaidByCharID() ([#3179](https://github.com/EQEmu/Server/pull/3179)) @Kinglykrab 2023-04-03
* Use a constant reference for content_flags in SetContentFlags() ([#3196](https://github.com/EQEmu/Server/pull/3196)) @Kinglykrab 2023-04-03
* Wake The Dead argument was named the same as a member variable in Mob ([#3214](https://github.com/EQEmu/Server/pull/3214)) @Kinglykrab 2023-04-03
* gid is assigned 2 values simultaneously in bot.cpp ([#3234](https://github.com/EQEmu/Server/pull/3234)) @Kinglykrab 2023-04-03
* summon_count > MAX_SWARM_PETS  is always false in aa.cpp ([#3212](https://github.com/EQEmu/Server/pull/3212)) @Kinglykrab 2023-04-03

### Fixes

* Correct Forward Declaration compilation warning ([#3176](https://github.com/EQEmu/Server/pull/3176)) @Aeadoin 2023-04-02
* Fix issue with Bot Raid invites not working. ([#3249](https://github.com/EQEmu/Server/pull/3249)) @Aeadoin 2023-04-03

### Performance

* Change to use Pass by reference where valid. ([#3163](https://github.com/EQEmu/Server/pull/3163)) @Aeadoin 2023-04-02

## [22.9.0] - 04/01/2023 

### Bots

* Remove Bot Groups Functionality ([#3165](https://github.com/EQEmu/Server/pull/3165)) @Aeadoin 2023-04-01

### Code

* Cleanup excessive type casting: string -> char * -> string ([#3169](https://github.com/EQEmu/Server/pull/3169)) @Aeadoin 2023-04-01

### Crash

* Add Checks for valid pointers or fix existing. ([#3164](https://github.com/EQEmu/Server/pull/3164)) @Aeadoin 2023-04-01
* Fix out of bound arrays, other potential crashes ([#3166](https://github.com/EQEmu/Server/pull/3166)) @Aeadoin 2023-04-01

### Fixes

* Correct SE_SlayUndead & SE_HeadShotLevel limit Value when applied. ([#3171](https://github.com/EQEmu/Server/pull/3171)) @Aeadoin 2023-04-01
* Prevent VerifyGroup from setting OOZ membername to Null character. ([#3168](https://github.com/EQEmu/Server/pull/3168)) @Aeadoin 2023-04-01

### Quest API

* Add missing Luabind definitions to lua_general.cpp ([#3167](https://github.com/EQEmu/Server/pull/3167)) @Kinglykrab 2023-04-01

## [22.8.2] - 03/30/2023 

### Code

* "equipped" not "equiped", "dual" not "duel". ([#3149](https://github.com/EQEmu/Server/pull/3149)) @Kinglykrab 2023-03-27

### Crash

* Add Checks for out of bounds & dereferencing nullptrs ([#3151](https://github.com/EQEmu/Server/pull/3151)) @Aeadoin 2023-03-28

### Fixes

* Check Rule "Bots Enabled" to prevent bot database calls on connect ([#3154](https://github.com/EQEmu/Server/pull/3154)) @Aeadoin 2023-03-29
* Correct logic checks for Bot rule AllowOwnerOptionAltCombat ([#3158](https://github.com/EQEmu/Server/pull/3158)) @Aeadoin 2023-03-30
* Fix an issue with EVENT_DISCONNECT not firing on regular /camp ([#3153](https://github.com/EQEmu/Server/pull/3153)) @Kinglykrab 2023-03-28
* Fix bot_raid_members.sql for MYSQL. ([#3155](https://github.com/EQEmu/Server/pull/3155)) @Aeadoin 2023-03-28
* Fix for OOZ Group updates when removing/inviting Bots ([#3159](https://github.com/EQEmu/Server/pull/3159)) @Aeadoin 2023-03-30
* Fix issues with Lua tables not starting at index 1 ([#3160](https://github.com/EQEmu/Server/pull/3160)) @Kinglykrab 2023-03-30
* Fix strcpy-param-overlap ([#3157](https://github.com/EQEmu/Server/pull/3157)) @Aeadoin 2023-03-29

### Rules

* Remove Guild Bank Zone ID Rule ([#3156](https://github.com/EQEmu/Server/pull/3156)) @Kinglykrab 2023-03-29

## [22.8.1] - 03/27/2023 

### Fixes

* Fix for NPCs having spells interrupted. ([#3150](https://github.com/EQEmu/Server/pull/3150)) @Aeadoin 2023-03-27

## [22.8.0] - 03/25/2023 

### Code

* Cleanup Strings::ToInt uses. ([#3142](https://github.com/EQEmu/Server/pull/3142)) @Aeadoin 2023-03-26
* Remove extern bool Critical ([#3146](https://github.com/EQEmu/Server/pull/3146)) @Kinglykrab 2023-03-25

### Crash

* Fix for crash in Raid::QueuePacket ([#3145](https://github.com/EQEmu/Server/pull/3145)) @Aeadoin 2023-03-25

### Feature

* Add support for -1 extradmgskill to allow all skills to be scaled. ([#3136](https://github.com/EQEmu/Server/pull/3136)) @Kinglykrab 2023-03-26

### Fixes

* Fix for Items looted from corpses. ([#3147](https://github.com/EQEmu/Server/pull/3147)) @Aeadoin 2023-03-26
* Fix for SQL Query in npc_scale_global_base ([#3144](https://github.com/EQEmu/Server/pull/3144)) @Aeadoin 2023-03-26

## [22.7.0] - 03/24/2023 

### Bots

* Place BOT_COMMAND_CHAR inside messages ([#3027](https://github.com/EQEmu/Server/pull/3027)) @trentdm 2023-03-05
* Prevent interrupt spam when OOM ([#3011](https://github.com/EQEmu/Server/pull/3011)) @nytmyr 2023-03-07

### Code

* Cleaning up Raid.cpp ([#3125](https://github.com/EQEmu/Server/pull/3125)) @Aeadoin 2023-03-20
* Cleanup unused methods and variables in world/main.cpp and world/main.h ([#3105](https://github.com/EQEmu/Server/pull/3105)) @Kinglykrab 2023-03-17
* Cleanup uses of Strings::ToInt to match correct type. ([#3054](https://github.com/EQEmu/Server/pull/3054)) @Aeadoin 2023-03-22
* Delete deprecated/perlxs folder ([#3110](https://github.com/EQEmu/Server/pull/3110)) @Kinglykrab 2023-03-17
* Delete queues.h ([#3089](https://github.com/EQEmu/Server/pull/3089)) @Kinglykrab 2023-03-17
* Delete world/console.old.cpp ([#3099](https://github.com/EQEmu/Server/pull/3099)) @Kinglykrab 2023-03-17
* Delete zone_numbers.h ([#3129](https://github.com/EQEmu/Server/pull/3129)) @Kinglykrab 2023-03-20
* Remove AllConnected(), CanUpdate(), and SendInfo() from login_server_list.cpp and login_server_list.h ([#3104](https://github.com/EQEmu/Server/pull/3104)) @Kinglykrab 2023-03-17
* Remove CLIENT_TIMEOUT from world/client.h and zone/client.h ([#3071](https://github.com/EQEmu/Server/pull/3071)) @Kinglykrab 2023-03-17
* Remove ChangeHP() from mob.h ([#3128](https://github.com/EQEmu/Server/pull/3128)) @Kinglykrab 2023-03-19
* Remove CheckAuth(), SetOnline(), and pMD5Pass from cliententry.h ([#3095](https://github.com/EQEmu/Server/pull/3095)) @Kinglykrab 2023-03-17
* Remove CommandRequirement() from zonedb.h ([#3094](https://github.com/EQEmu/Server/pull/3094)) @Kinglykrab 2023-03-17
* Remove CountZones() from launcher_link.h ([#3100](https://github.com/EQEmu/Server/pull/3100)) @Kinglykrab 2023-03-17
* Remove DBInitVars() and HandleMysqlError() from queryserv/database.h ([#3114](https://github.com/EQEmu/Server/pull/3114)) @Kinglykrab 2023-03-17
* Remove DBInitVars(), HandleMysqlError(), and IsChatChannelInDB() in ucs/database.h ([#3113](https://github.com/EQEmu/Server/pull/3113)) @Kinglykrab 2023-03-17
* Remove DisableStats(), EnableStats(), DisableLoginserver(), and EnableLoginserver() from world_config.h ([#3107](https://github.com/EQEmu/Server/pull/3107)) @Kinglykrab 2023-03-17
* Remove DoBuffWearOffEffect() from mob.h ([#3062](https://github.com/EQEmu/Server/pull/3062)) @Kinglykrab 2023-03-17
* Remove FindByName(charname) from clientlist.h ([#3096](https://github.com/EQEmu/Server/pull/3096)) @Kinglykrab 2023-03-17
* Remove FindCLEByLSID(), GetCLE(), GetCLEIPCount(), and RemoveCLEByLSID() from clientlist.h ([#3098](https://github.com/EQEmu/Server/pull/3098)) @Kinglykrab 2023-03-17
* Remove FindPatch() from struct_category.cpp and struct_category.h ([#3130](https://github.com/EQEmu/Server/pull/3130)) @Kinglykrab 2023-03-20
* Remove FlushLootStats() from npc.h ([#3079](https://github.com/EQEmu/Server/pull/3079)) @Kinglykrab 2023-03-17
* Remove GetAILevel() from npc.h ([#3080](https://github.com/EQEmu/Server/pull/3080)) @Kinglykrab 2023-03-17
* Remove GetDestination() from doors.h ([#3078](https://github.com/EQEmu/Server/pull/3078)) @Kinglykrab 2023-03-17
* Remove GetServerByAddress() from server_manager.h ([#3119](https://github.com/EQEmu/Server/pull/3119)) @Kinglykrab 2023-03-17
* Remove GetStartCount() and InitStartTimer() from zone_launch.cpp and zone_launch.h ([#3121](https://github.com/EQEmu/Server/pull/3121)) @Kinglykrab 2023-03-17
* Remove GetTransformation() and GetInvertedTransformation() from oriented_bounding_box.h ([#3084](https://github.com/EQEmu/Server/pull/3084)) @Kinglykrab 2023-03-17
* Remove IsAffectedByBuff() ([#3068](https://github.com/EQEmu/Server/pull/3068)) @Kinglykrab 2023-03-17
* Remove IsConnected() from loginserver/database.h ([#3117](https://github.com/EQEmu/Server/pull/3117)) @Kinglykrab 2023-03-17
* Remove IsOrigin(glm::vec2) from position.h ([#3088](https://github.com/EQEmu/Server/pull/3088)) @Kinglykrab 2023-03-17
* Remove MakeGuildMembers() from wguild_mgr.h ([#3106](https://github.com/EQEmu/Server/pull/3106)) @Kinglykrab 2023-03-17
* Remove PlayerLogin_Struct from login_types.h ([#3118](https://github.com/EQEmu/Server/pull/3118)) @Kinglykrab 2023-03-17
* Remove RemoveSpawnGroup() from spawngroup.h ([#3090](https://github.com/EQEmu/Server/pull/3090)) @Kinglykrab 2023-03-17
* Remove SendGuildPacket() from clientlist.cpp, clientlist.h, and wguild_mgr.cpp ([#3097](https://github.com/EQEmu/Server/pull/3097)) @Kinglykrab 2023-03-17
* Remove SetConnection() from loginserver/world_server.h ([#3120](https://github.com/EQEmu/Server/pull/3120)) @Kinglykrab 2023-03-17
* Remove SetDBID() from object.h ([#3082](https://github.com/EQEmu/Server/pull/3082)) @Kinglykrab 2023-03-17
* Remove SetSentTime2 in petitions.h ([#3086](https://github.com/EQEmu/Server/pull/3086)) @Kinglykrab 2023-03-17
* Remove StoreCharacter() from worlddb.h ([#3108](https://github.com/EQEmu/Server/pull/3108)) @Kinglykrab 2023-03-17
* Remove UpdateLoginserverWorldAdminAccountPasswordById() from account_management.cpp ([#3115](https://github.com/EQEmu/Server/pull/3115)) @Kinglykrab 2023-03-17
* Remove _baseBotStance from bot.h ([#3076](https://github.com/EQEmu/Server/pull/3076)) @Kinglykrab 2023-03-17
* Remove _botRole from bot.h ([#3075](https://github.com/EQEmu/Server/pull/3075)) @Kinglykrab 2023-03-17
* Remove _previousTarget from bot.h ([#3074](https://github.com/EQEmu/Server/pull/3074)) @Kinglykrab 2023-03-17
* Remove authenticated from launcher_link.cpp and launcher_link.h ([#3101](https://github.com/EQEmu/Server/pull/3101)) @Kinglykrab 2023-03-17
* Remove can_corpse_be_rezzed from corpse.h ([#3077](https://github.com/EQEmu/Server/pull/3077)) @Kinglykrab 2023-03-17
* Remove casting_spell_type from mob.h ([#3064](https://github.com/EQEmu/Server/pull/3064)) @Kinglykrab 2023-03-17
* Remove class EQStream from client.h ([#3070](https://github.com/EQEmu/Server/pull/3070)) @Kinglykrab 2023-03-17
* Remove current_buff_count ([#3067](https://github.com/EQEmu/Server/pull/3067)) @Kinglykrab 2023-03-17
* Remove firstlogin and realfirstlogin from world/client.h ([#3072](https://github.com/EQEmu/Server/pull/3072)) @Kinglykrab 2023-03-17
* Remove fixedZ from mob.h ([#3065](https://github.com/EQEmu/Server/pull/3065)) @Kinglykrab 2023-03-17
* Remove inWater from mob.h ([#3069](https://github.com/EQEmu/Server/pull/3069)) @Kinglykrab 2023-03-17
* Remove is_authenticatd, LSShutDownUpdate(), and SetInstanceID() from zoneserver.h ([#3109](https://github.com/EQEmu/Server/pull/3109)) @Kinglykrab 2023-03-17
* Remove last_insert_id from petitions.h ([#3087](https://github.com/EQEmu/Server/pull/3087)) @Kinglykrab 2023-03-17
* Remove last_max_hp from mob.h ([#3063](https://github.com/EQEmu/Server/pull/3063)) @Kinglykrab 2023-03-17
* Remove m_inuse, m_z, and m_heading from object.h ([#3083](https://github.com/EQEmu/Server/pull/3083)) @Kinglykrab 2023-03-17
* Remove npc_ai.cpp/npc_ai.cpp ([#3081](https://github.com/EQEmu/Server/pull/3081)) @Kinglykrab 2023-03-17
* Remove ownHiddenTrigger from trap.cpp and trap.h ([#3092](https://github.com/EQEmu/Server/pull/3092)) @Kinglykrab 2023-03-17
* Remove perlparser.h ([#3085](https://github.com/EQEmu/Server/pull/3085)) @Kinglykrab 2023-03-17
* Remove unused AbilityTimer variable in client.h ([#3035](https://github.com/EQEmu/Server/pull/3035)) @Kinglykrab 2023-03-05
* Remove unused BotAA struct in bot_structs.h ([#3038](https://github.com/EQEmu/Server/pull/3038)) @Kinglykrab 2023-03-05
* Remove unused HandleUpdateTasksOnKill in client.h ([#3032](https://github.com/EQEmu/Server/pull/3032)) @Kinglykrab 2023-03-05
* Remove unused SaveBackup in client.h ([#3030](https://github.com/EQEmu/Server/pull/3030)) @Kinglykrab 2023-03-05
* Remove unused ^evacuate and ^succor subcommands from bot_command.h ([#3039](https://github.com/EQEmu/Server/pull/3039)) @Kinglykrab 2023-03-05
* Remove unused bot structs in bot_structs.h ([#3037](https://github.com/EQEmu/Server/pull/3037)) @Kinglykrab 2023-03-05
* Remove unused client queued work variable in client.cpp/client.h ([#3034](https://github.com/EQEmu/Server/pull/3034)) @Kinglykrab 2023-03-05
* Remove unused command variables in client.cpp ([#3031](https://github.com/EQEmu/Server/pull/3031)) @Kinglykrab 2023-03-05
* Remove unused lua_hate_entry.cpp ([#3057](https://github.com/EQEmu/Server/pull/3057)) @Kinglykrab 2023-03-12
* Remove unused methods in eql_config.cpp, eql_config.h, launcher_list.cpp, and launcher_list.h ([#3103](https://github.com/EQEmu/Server/pull/3103)) @Kinglykrab 2023-03-17
* Remove unused methods in loginserver/client.h ([#3116](https://github.com/EQEmu/Server/pull/3116)) @Kinglykrab 2023-03-17
* Remove unused player update variables in client.cpp/client.h ([#3033](https://github.com/EQEmu/Server/pull/3033)) @Kinglykrab 2023-03-05
* Utilize GetPlayerState() in mob methods ([#3066](https://github.com/EQEmu/Server/pull/3066)) @Kinglykrab 2023-03-17
* Utilize GetScheduler() in zone/worldserver.cpp ([#3093](https://github.com/EQEmu/Server/pull/3093)) @Kinglykrab 2023-03-17
* Utilize SetFilter in client.cpp ([#3036](https://github.com/EQEmu/Server/pull/3036)) @Kinglykrab 2023-03-05
* Utilize SetHiddenTrigger in trap.cpp ([#3091](https://github.com/EQEmu/Server/pull/3091)) @Kinglykrab 2023-03-17
* remove _botOrderAttack from bot.h ([#3073](https://github.com/EQEmu/Server/pull/3073)) @Kinglykrab 2023-03-17

### Commands

* Cleanup #haste Command ([#3042](https://github.com/EQEmu/Server/pull/3042)) @Kinglykrab 2023-03-06
* Cleanup #hideme Command ([#3043](https://github.com/EQEmu/Server/pull/3043)) @Kinglykrab 2023-03-06
* Cleanup #interrupt Command ([#3044](https://github.com/EQEmu/Server/pull/3044)) @Kinglykrab 2023-03-06
* Cleanup #level Command ([#3045](https://github.com/EQEmu/Server/pull/3045)) @Kinglykrab 2023-03-06
* Cleanup #picklock Command ([#3046](https://github.com/EQEmu/Server/pull/3046)) @Kinglykrab 2023-03-06
* Cleanup #resetaa and #resetaa_timer ([#3047](https://github.com/EQEmu/Server/pull/3047)) @Kinglykrab 2023-03-06
* Cleanup #wc Command ([#3049](https://github.com/EQEmu/Server/pull/3049)) @Kinglykrab 2023-03-06
* Remove #equipitem Command ([#3040](https://github.com/EQEmu/Server/pull/3040)) @Kinglykrab 2023-03-06

### Console

* Add IS_TTY to force terminal coloring output ([#3021](https://github.com/EQEmu/Server/pull/3021)) @Akkadius 2023-03-04

### Crash

* Fix dangling Group member pointers for Bots. ([#3134](https://github.com/EQEmu/Server/pull/3134)) @Aeadoin 2023-03-21
* Fixes Crash when Zoning with XTarget when Bots are in group. ([#3126](https://github.com/EQEmu/Server/pull/3126)) @Aeadoin 2023-03-19

### Feature

* Add Basic Bot Raiding Functionality ([#2782](https://github.com/EQEmu/Server/pull/2782)) @neckkola 2023-03-17
* Add Data Bucket support for scaling of Heroic Stats. ([#3058](https://github.com/EQEmu/Server/pull/3058)) @Aeadoin 2023-03-24
* Add Item Extra Skill Damage Percent Modifier ([#3127](https://github.com/EQEmu/Server/pull/3127)) @Kinglykrab 2023-03-19

### Fixes

* Add Avoidance and HP Regen Per Second too NPC Scaling. ([#3050](https://github.com/EQEmu/Server/pull/3050)) @Aeadoin 2023-03-09
* Add Heroic Strikethrough & HP Regen Per Second to GM Entity Info ([#3055](https://github.com/EQEmu/Server/pull/3055)) @Aeadoin 2023-03-12
* Add Heroic Strikethrough to NPC Scaling ([#3028](https://github.com/EQEmu/Server/pull/3028)) @Kinglykrab 2023-03-06
* Change SPA 193 Weapon Damage to allow values over 65,535 ([#3138](https://github.com/EQEmu/Server/pull/3138)) @Aeadoin 2023-03-23
* Checkmarks and X characters in popup messages ([#3041](https://github.com/EQEmu/Server/pull/3041)) @Kinglykrab 2023-03-06
* Cursor Coin Upon Death ([#3020](https://github.com/EQEmu/Server/pull/3020)) @cybernine186 2023-03-04
* Ensure synchronization of pet taunt state with UI ([#3025](https://github.com/EQEmu/Server/pull/3025)) @catapultam-habeo 2023-03-04
* Fix Bard Bot Casting ([#3122](https://github.com/EQEmu/Server/pull/3122)) @Aeadoin 2023-03-17
* Fix Discovered Items with Alternate Currency and LDoN Adventure Merchants ([#3026](https://github.com/EQEmu/Server/pull/3026)) @Kinglykrab 2023-03-04
* Fix Heal Scale and Spell Scale in NPC Scaling ([#3051](https://github.com/EQEmu/Server/pull/3051)) @Kinglykrab 2023-03-10
* Fix Raid Invites causing client desync issues ([#3053](https://github.com/EQEmu/Server/pull/3053)) @Aeadoin 2023-03-11
* Fix Raid methods that could cause crashes with Bots in raid ([#3111](https://github.com/EQEmu/Server/pull/3111)) @Aeadoin 2023-03-17
* Fix edge cases where camped bots would be left in a raid ([#3139](https://github.com/EQEmu/Server/pull/3139)) @Aeadoin 2023-03-23
* Fix for Raid Disband if leader not in same zone. ([#3135](https://github.com/EQEmu/Server/pull/3135)) @Aeadoin 2023-03-21
* Fix for incorrect bindpoint x,y,z,headings ([#3141](https://github.com/EQEmu/Server/pull/3141)) @Aeadoin 2023-03-23
* Fix for transferring Raid Leader ([#3140](https://github.com/EQEmu/Server/pull/3140)) @Aeadoin 2023-03-23
* Fix issue with overflow on min/max hit dmg in npc scaling calculations ([#3052](https://github.com/EQEmu/Server/pull/3052)) @Aeadoin 2023-03-10
* Fix typo for bot_id raid_members column in db_update_manifest.txt ([#3132](https://github.com/EQEmu/Server/pull/3132)) @Kinglykrab 2023-03-20
* Fixes for corpses not properly saving some item instance data correctly. ([#3123](https://github.com/EQEmu/Server/pull/3123)) @KimLS 2023-03-23

### Illusions

* Fix bug where spells like Ignite Bones left NPC size incorrect. ([#3061](https://github.com/EQEmu/Server/pull/3061)) @noudess 2023-03-16

### Quest API

* Add SendIllusion overloads/parameters to Perl/Lua ([#3059](https://github.com/EQEmu/Server/pull/3059)) @Kinglykrab 2023-03-16
* Add Spell GetActX methods to Perl/Lua ([#3056](https://github.com/EQEmu/Server/pull/3056)) @Kinglykrab 2023-03-12
* Add Timer related methods to Mobs in Perl/Lua ([#3133](https://github.com/EQEmu/Server/pull/3133)) @Kinglykrab 2023-03-20

### Rules

* Add Multiplier for Heroic Stats. ([#3014](https://github.com/EQEmu/Server/pull/3014)) @Aeadoin 2023-03-04
* Add ResurrectionEffectsBlock ([#2990](https://github.com/EQEmu/Server/pull/2990)) @nytmyr 2023-03-04
* Add Rule to allow ExtraDmgSkill/SPA 220 to effect Spell Skills ([#3124](https://github.com/EQEmu/Server/pull/3124)) @Aeadoin 2023-03-19
* Add Task System Rule ExpRewardsIgnoreLevelBasedEXPMods ([#3112](https://github.com/EQEmu/Server/pull/3112)) @Aeadoin 2023-03-17

### Scaling

* Add support for pipe-separated zone IDs and versions ([#3015](https://github.com/EQEmu/Server/pull/3015)) @Kinglykrab 2023-03-04

### Strings

* Add exception handling to converters themselves ([#3029](https://github.com/EQEmu/Server/pull/3029)) @Akkadius 2023-03-05
* Add more number formatters ([#2873](https://github.com/EQEmu/Server/pull/2873)) @Kinglykrab 2023-03-04

## [22.4.5] - 03/03/2023 

### Bots

* Add additional Heroic Sta/Wis/Int bonuses for Bots. ([#3013](https://github.com/EQEmu/Server/pull/3013)) @Aeadoin 2023-03-01
* Cleanup AI_IdleCastCheck Logic ([#3004](https://github.com/EQEmu/Server/pull/3004)) @Aeadoin 2023-02-26

### Code

* Delete unused zone/skills.h ([#3007](https://github.com/EQEmu/Server/pull/3007)) @Kinglykrab 2023-02-27
* Remove DumpPacketProfile() from client.h ([#3000](https://github.com/EQEmu/Server/pull/3000)) @Kinglykrab 2023-02-26
* Remove GetCombinedAC_TEST() from client.h ([#2999](https://github.com/EQEmu/Server/pull/2999)) @Kinglykrab 2023-02-26
* Remove GetDamageMultiplier() from client.h ([#3001](https://github.com/EQEmu/Server/pull/3001)) @Kinglykrab 2023-02-26
* Remove NumberOfAvailableTitles() from titles.h ([#3006](https://github.com/EQEmu/Server/pull/3006)) @Kinglykrab 2023-02-27
* Remove ReturnItemPacket from client.h/inventory.cpp ([#3002](https://github.com/EQEmu/Server/pull/3002)) @Kinglykrab 2023-02-26
* Remove class EGNode from mob.h ([#3003](https://github.com/EQEmu/Server/pull/3003)) @Kinglykrab 2023-02-26
* Remove unused ClientFactory in client.h ([#2998](https://github.com/EQEmu/Server/pull/2998)) @Kinglykrab 2023-02-26
* Remove unused iterator from LoadCharacterDisciplines ([#3012](https://github.com/EQEmu/Server/pull/3012)) @Aeadoin 2023-03-02

### Crash

* Fix crash in CheckTradeskillLoreConflict ([#3009](https://github.com/EQEmu/Server/pull/3009)) @Aeadoin 2023-02-28

### Fixes

* Account for bad data in Tradeskill Recipe Entries ([#2991](https://github.com/EQEmu/Server/pull/2991)) @Aeadoin 2023-02-25
* Fix DoAnim quest method default speed ([#3016](https://github.com/EQEmu/Server/pull/3016)) @Kinglykrab 2023-03-01
* Fix an issue where EVENT_TIMER timers would not be cleaned up after zone ([#3018](https://github.com/EQEmu/Server/pull/3018)) @noudess 2023-03-03
* Fix for Discipline Loading from Database causing issues with slot_ids ([#3008](https://github.com/EQEmu/Server/pull/3008)) @Aeadoin 2023-02-28
* Fix for Lore Components where component is returned. ([#3005](https://github.com/EQEmu/Server/pull/3005)) @Aeadoin 2023-02-27
* Fix issue where quest saylink responses would occur before the NPC's response ([#3010](https://github.com/EQEmu/Server/pull/3010)) @Akkadius 2023-03-01
* Fix log messages when players join channel ([#2992](https://github.com/EQEmu/Server/pull/2992)) @Valorith 2023-03-03
* Fix npcfeature and playerfeature ([#3017](https://github.com/EQEmu/Server/pull/3017)) @Kinglykrab 2023-03-02

### Quest API

* Add GetDefaultRaceSize() to Perl/Lua ([#2993](https://github.com/EQEmu/Server/pull/2993)) @Kinglykrab 2023-02-27
* Add HasSpecialAbilities() to Perl/Lua ([#2994](https://github.com/EQEmu/Server/pull/2994)) @Kinglykrab 2023-02-27
* Add IsBerserk() to Perl/Lua ([#2997](https://github.com/EQEmu/Server/pull/2997)) @Kinglykrab 2023-03-01
* Add IsFindable() and IsTrackable() to Perl/Lua ([#2996](https://github.com/EQEmu/Server/pull/2996)) @Kinglykrab 2023-03-01
* Add IsUnderwaterOnly() to Perl/Lua ([#2995](https://github.com/EQEmu/Server/pull/2995)) @Kinglykrab 2023-03-01

## [22.4.4] - 02/24/2023 

### Bots

* Add Caster Range Command, and IsValidSpellRange Checks ([#2942](https://github.com/EQEmu/Server/pull/2942)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-23
* Cleanup BotDatabase::LoadBuffs ([#2981](https://github.com/EQEmu/Server/pull/2981)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-24
* Verify Bots Group Integrity on join ([#2980](https://github.com/EQEmu/Server/pull/2980)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-23

### Commands

* Cleanup #peekinv Command ([#2969](https://github.com/EQEmu/Server/pull/2969)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-23

### Doors

* Fix doors triggering invalid zone fetches of dest_zone of "none" ([#2985](https://github.com/EQEmu/Server/pull/2985)) ([Akkadius](https://github.com/Akkadius)) 2023-02-24

### Fixes

* Adjust database manifest to include .sql extension  ([Akkadius](https://github.com/Akkadius)) 2023-02-25
* Correct Mend reuse time and add reduction support. ([#2972](https://github.com/EQEmu/Server/pull/2972)) ([nytmyr](https://github.com/nytmyr)) 2023-02-23
* Fix Beneficial Target of Target procs ([#2987](https://github.com/EQEmu/Server/pull/2987)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-24
* Fix for undefined MySQL library behavior. ([#2834](https://github.com/EQEmu/Server/pull/2834)) ([KimLS](https://github.com/KimLS)) 2023-02-25

### Pathing

* Improve roambox logic ([#2983](https://github.com/EQEmu/Server/pull/2983)) ([Akkadius](https://github.com/Akkadius)) 2023-02-24
* More z-clip improvements, Wurm and Spectral Iksar race adjustments ([#2988](https://github.com/EQEmu/Server/pull/2988)) ([Akkadius](https://github.com/Akkadius)) 2023-02-25
* Smoother pathing z-correction ([#2982](https://github.com/EQEmu/Server/pull/2982)) ([Akkadius](https://github.com/Akkadius)) 2023-02-24

### Player Events

* Add QS processing, mutex tweaks ([#2984](https://github.com/EQEmu/Server/pull/2984)) ([Akkadius](https://github.com/Akkadius)) 2023-02-25

### Quest API

* Add IsAutoAttackEnabled() to Perl/Lua ([#2979](https://github.com/EQEmu/Server/pull/2979)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-23
* Add IsAutoFireEnabled() to Perl/Lua ([#2978](https://github.com/EQEmu/Server/pull/2978)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-23
* Fix EVENT_TIMER crash when entity is no longer available ([#2986](https://github.com/EQEmu/Server/pull/2986)) ([Akkadius](https://github.com/Akkadius)) 2023-02-24

### Scaling

* Add support for zone ID and instance version to NPC Scaling ([#2968](https://github.com/EQEmu/Server/pull/2968)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-25

### Tradeskills

* Fix for Lore Conflict ([#2977](https://github.com/EQEmu/Server/pull/2977)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-24

## [22.4.3] - 02/21/2023 

### Bots

* Change HasBotItem(item_id) to return slot_id instead of bool. ([#2966](https://github.com/EQEmu/Server/pull/2966)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-19
* Change SaveTimers to Replace instead of Insert. ([#2951](https://github.com/EQEmu/Server/pull/2951)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-18
* Fix output of ^spells while ^Enforcespellsettings is enabled ([#2959](https://github.com/EQEmu/Server/pull/2959)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-18

### Crash

* Fix crash with EVENT_UNEQUIP_ITEM_BOT ([#2973](https://github.com/EQEmu/Server/pull/2973)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-20
* Fix world crash in player event processing ([#2960](https://github.com/EQEmu/Server/pull/2960)) ([Akkadius](https://github.com/Akkadius)) 2023-02-18

### Database

* Address deadlock in player events ([#2974](https://github.com/EQEmu/Server/pull/2974)) ([Akkadius](https://github.com/Akkadius)) 2023-02-21

### Fixes

* Fix MIR LDoN Theme Items on LDoN Merchants ([#2971](https://github.com/EQEmu/Server/pull/2971)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-20
* Fix OOCMute not functioning ([#2970](https://github.com/EQEmu/Server/pull/2970)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-20

### Pathing

* Improvements to z-clipping, z-recovery and z-calculations ([#2975](https://github.com/EQEmu/Server/pull/2975)) ([Akkadius](https://github.com/Akkadius)) 2023-02-21

### Pets

* Client Pet summoned by NPC should not change guard location. ([#2967](https://github.com/EQEmu/Server/pull/2967)) ([noudess](https://github.com/noudess)) 2023-02-19

### Player Events

* Create new event ITEM_CREATION ([#2944](https://github.com/EQEmu/Server/pull/2944)) ([Akkadius](https://github.com/Akkadius)) 2023-02-18

### Quest API

* Add client->SignalClient() overload to Perl ([#2963](https://github.com/EQEmu/Server/pull/2963)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-19
* Fix Perl SetSimpleRoamBox Overloads ([#2961](https://github.com/EQEmu/Server/pull/2961)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-19

### Reload API

* Add world handlers for certain opcodes ([#2958](https://github.com/EQEmu/Server/pull/2958)) ([Akkadius](https://github.com/Akkadius)) 2023-02-18

### SQL

* Add date to optional Drakkin Guktan Faction Update ([#2965](https://github.com/EQEmu/Server/pull/2965)) ([joligario](https://github.com/joligario)) 2023-02-19

## [22.4.2] - 02/18/2023 

### Content

* Added optional SQL 2023_02_17_fix_sseru_mischief_doors.sql to fix sseru/mischief doors ([#2955](https://github.com/EQEmu/Server/pull/2955)) ([Akkadius](https://github.com/Akkadius)) 2023-02-18

### Logging

* Remove noisy raid/group/forage errors ([#2952](https://github.com/EQEmu/Server/pull/2952)) ([Akkadius](https://github.com/Akkadius)) 2023-02-18

### MySQL

* Add keepalives to UCS and Loginserver ([#2953](https://github.com/EQEmu/Server/pull/2953)) ([Akkadius](https://github.com/Akkadius)) 2023-02-18

### Player Events

* Add logging category to hold processing batch logs ([#2954](https://github.com/EQEmu/Server/pull/2954)) ([Akkadius](https://github.com/Akkadius)) 2023-02-18

### Tradeskills

* Fix regression caused by #2932 ([#2956](https://github.com/EQEmu/Server/pull/2956)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-18

## [22.4.1] - 02/17/2023 

### Bots

* Set Taunt to enabled for SK/Paladin Bots by Default. ([#2941](https://github.com/EQEmu/Server/pull/2941)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-17

### DevTools

* Fix NPC targetting dev tools display window ([#2943](https://github.com/EQEmu/Server/pull/2943)) ([Akkadius](https://github.com/Akkadius)) 2023-02-17

### Fixes

* Issue with AssignRaidToInstance that was using the groups repository instead of raid ([#2947](https://github.com/EQEmu/Server/pull/2947)) ([Akkadius](https://github.com/Akkadius)) 2023-02-17
* Missing comma in schema list breaking dumps  ([Akkadius](https://github.com/Akkadius)) 2023-02-17

### Player Events

* Fix issue with item instances not being validated properly before accessing causing crashes on handin ([#2945](https://github.com/EQEmu/Server/pull/2945)) ([Akkadius](https://github.com/Akkadius)) 2023-02-17
* Fix rare out of bound issue when loading event types ([#2946](https://github.com/EQEmu/Server/pull/2946)) ([Akkadius](https://github.com/Akkadius)) 2023-02-17
* Turn off KILLED_NPC (trash) off by default ([#2948](https://github.com/EQEmu/Server/pull/2948)) ([Akkadius](https://github.com/Akkadius)) 2023-02-17

## [22.4.0] - 02/17/2023 

### Bots

* Add Additional HeroicAgi/Dex Modifiers. ([#2838](https://github.com/EQEmu/Server/pull/2838)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-07
* Add Additional HeroicStr modifiers. ([#2837](https://github.com/EQEmu/Server/pull/2837)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-07
* Add IsBot() to methods in attack.cpp where applicable. ([#2840](https://github.com/EQEmu/Server/pull/2840)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-09
* Add Lore Check for Augments. ([#2874](https://github.com/EQEmu/Server/pull/2874)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-12
* Add Pet Power Support for Temp Pets. ([#2853](https://github.com/EQEmu/Server/pull/2853)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-11
* Add Support for TryTriggerOnCastFocusEffect ([#2864](https://github.com/EQEmu/Server/pull/2864)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-13
* Add TotalDominationBonus modifiers. ([#2852](https://github.com/EQEmu/Server/pull/2852)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-09
* ST_AreaClientOnly spells to land on Bots ([#2849](https://github.com/EQEmu/Server/pull/2849)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-09
* Update ResistSpell to use temp_level_diff client formula ([#2851](https://github.com/EQEmu/Server/pull/2851)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-09

### Bots & Mercenaries

* Add 100% Hit chance if sitting while attacked. ([#2839](https://github.com/EQEmu/Server/pull/2839)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-07
* Add Support for TrySympatheticProc ([#2866](https://github.com/EQEmu/Server/pull/2866)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-13

### CI

* Fix Windows stderr not bubbling properly ([#2925](https://github.com/EQEmu/Server/pull/2925)) ([Akkadius](https://github.com/Akkadius)) 2023-02-14

### Code

* Add IsOfClientBot() virtual method. ([#2845](https://github.com/EQEmu/Server/pull/2845)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-07
* Doors EVENT_CLICK_DOOR syntax adjustment  ([Akkadius](https://github.com/Akkadius)) 2023-02-14
* Remove Unused Mod Hooks ([#2856](https://github.com/EQEmu/Server/pull/2856)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13

### Crash

* Crash fix where invalid input to #heromodel would crash zone ([#2937](https://github.com/EQEmu/Server/pull/2937)) ([Akkadius](https://github.com/Akkadius)) 2023-02-15
* Fix Bot Crash in Bot::Bot Constructor. ([#2868](https://github.com/EQEmu/Server/pull/2868)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-12
* Fix Crash in FindType ([#2867](https://github.com/EQEmu/Server/pull/2867)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-13
* Fix crash in Mob::CommonDamage when attacker was null ([#2872](https://github.com/EQEmu/Server/pull/2872)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-13
* Fix crash issue with dropping items and order of operations ([#2939](https://github.com/EQEmu/Server/pull/2939)) ([joligario](https://github.com/joligario)) 2023-02-16
* Fix issue where long short names overflow file_name  ([Akkadius](https://github.com/Akkadius)) 2023-02-09
* Fix potential crash in Mob::CommonDamage ([#2848](https://github.com/EQEmu/Server/pull/2848)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-09

### Doors

* Fix issue where NPC's wouldn't open doors because door param overflow ([#2934](https://github.com/EQEmu/Server/pull/2934)) ([Akkadius](https://github.com/Akkadius)) 2023-02-15

### Feature

* Add IsOfClientBotMerc() virtual method. ([#2843](https://github.com/EQEmu/Server/pull/2843)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-07

### Fixes

* Another doors fix  ([Akkadius](https://github.com/Akkadius)) 2023-02-14
* Fix CheckNumHitsRemaining() with 1H Blunt ([#2846](https://github.com/EQEmu/Server/pull/2846)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-07
* Fix Door opening regression caused by #2880  ([Akkadius](https://github.com/Akkadius)) 2023-02-14
* Fix EVENT_SPELL_EFFECT_TRANSLOCATE_COMPLETE regression caused by  #2897 ([#2928](https://github.com/EQEmu/Server/pull/2928)) ([Akkadius](https://github.com/Akkadius)) 2023-02-14
* Fix HP_EVENT regression ([#2927](https://github.com/EQEmu/Server/pull/2927)) ([Akkadius](https://github.com/Akkadius)) 2023-02-14
* Fix crash in EVENT_DISCOVER_ITEM ([#2933](https://github.com/EQEmu/Server/pull/2933)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-15
* Fix crash where dropped items crash Lua logic ([#2936](https://github.com/EQEmu/Server/pull/2936)) ([Akkadius](https://github.com/Akkadius)) 2023-02-15
* Fix for interrupting item casts to no longer lock the client if cast time of item greater than 0 ([#2921](https://github.com/EQEmu/Server/pull/2921)) ([Natedog2012](https://github.com/Natedog2012)) 2023-02-13
* Fix issue where Lore groundspawn pickups will desync ROF2+ ([#2929](https://github.com/EQEmu/Server/pull/2929)) ([Akkadius](https://github.com/Akkadius)) 2023-02-14
* Fix issue with EVENT_HP firing regression from #2904 ([#2924](https://github.com/EQEmu/Server/pull/2924)) ([Akkadius](https://github.com/Akkadius)) 2023-02-14
* Replace uses of SPELL_UNKNOWN with IsValidSpell() ([#2938](https://github.com/EQEmu/Server/pull/2938)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-16
* Self Only Spells will no longer check target level or buff restrictions ([#2931](https://github.com/EQEmu/Server/pull/2931)) ([noudess](https://github.com/noudess)) 2023-02-15

### Groundspawns

* Fix issue where groundspawns appear floating high off the ground ([#2930](https://github.com/EQEmu/Server/pull/2930)) ([Akkadius](https://github.com/Akkadius)) 2023-02-15

### Logging

* Add raw opcode when emu translated opcode is not found (OP_Unknown) via (C->S) ([#2847](https://github.com/EQEmu/Server/pull/2847)) ([Akkadius](https://github.com/Akkadius)) 2023-02-08
* Implement Player Event Logging system ([#2833](https://github.com/EQEmu/Server/pull/2833)) ([Akkadius](https://github.com/Akkadius)) 2023-02-13

### Quest API

* (Performance) Check equip or scale item events exist before export and execute ([#2898](https://github.com/EQEmu/Server/pull/2898)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_AA_BUY or EVENT_AA_GAIN exist before export and execute ([#2892](https://github.com/EQEmu/Server/pull/2892)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_AGGRO, EVENT_ATTACK, or EVENT_COMBAT exist before export and execute ([#2901](https://github.com/EQEmu/Server/pull/2901)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_COMBINE, EVENT_COMBINE_SUCCESS, EVENT_COMBINE_FAILURE, or EVENT_COMBINE_VALIDATE exist before export and execute ([#2896](https://github.com/EQEmu/Server/pull/2896)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_DEATH, EVENT_DEATH_COMPLETE, or EVENT_DEATH_ZONE exist before export and execute ([#2909](https://github.com/EQEmu/Server/pull/2909)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_ENVIRONMENTAL_DAMAGE exists before export and execute ([#2899](https://github.com/EQEmu/Server/pull/2899)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_FEIGN_DEATH exists before export and execute ([#2916](https://github.com/EQEmu/Server/pull/2916)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_ITEM_TICK or EVENT_WEAPON_PROC exist before export and execute ([#2914](https://github.com/EQEmu/Server/pull/2914)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_LANGUAGE_SKILL_UP, EVENT_SKILL_UP, or EVENT_USE_SKILL exist before export and execute ([#2894](https://github.com/EQEmu/Server/pull/2894)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_PAYLOAD or EVENT_SIGNAL exist before export and execute ([#2902](https://github.com/EQEmu/Server/pull/2902)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_SLAY exists before export and execute ([#2910](https://github.com/EQEmu/Server/pull/2910)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event EVENT_WAYPOINT_ARRIVE or EVENT_WAYPOINT_DEPART exist before export and execute ([#2905](https://github.com/EQEmu/Server/pull/2905)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_AGGRO_SAY, EVENT_SAY, and EVENT_PROXIMITY_SAY ([#2882](https://github.com/EQEmu/Server/pull/2882)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_BOT_CREATE ([#2886](https://github.com/EQEmu/Server/pull/2886)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_CLICK_DOOR and EVENT_CLICK_OBJECT ([#2880](https://github.com/EQEmu/Server/pull/2880)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_DESPAWN and EVENT_DESPAWN_ZONE ([#2887](https://github.com/EQEmu/Server/pull/2887)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_DISCOVER_ITEM ([#2912](https://github.com/EQEmu/Server/pull/2912)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_DUEL_LOSE and EVENT_DUEL_WIN ([#2915](https://github.com/EQEmu/Server/pull/2915)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_ENTER_ZONE and EVENT_ZONE ([#2900](https://github.com/EQEmu/Server/pull/2900)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_GM_COMMAND ([#2890](https://github.com/EQEmu/Server/pull/2890)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_GROUP_CHANGE ([#2884](https://github.com/EQEmu/Server/pull/2884)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_HP ([#2904](https://github.com/EQEmu/Server/pull/2904)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_KILLED_MERIT ([#2911](https://github.com/EQEmu/Server/pull/2911)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_LEVEL_UP and EVENT_LEVEL_DOWN ([#2889](https://github.com/EQEmu/Server/pull/2889)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_POPUP_RESPONSE ([#2881](https://github.com/EQEmu/Server/pull/2881)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_RESPAWN ([#2917](https://github.com/EQEmu/Server/pull/2917)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_TICK ([#2919](https://github.com/EQEmu/Server/pull/2919)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_TIMER ([#2903](https://github.com/EQEmu/Server/pull/2903)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_TRADE ([#2906](https://github.com/EQEmu/Server/pull/2906)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_UNHANDLED_OPCODE ([#2918](https://github.com/EQEmu/Server/pull/2918)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_WARP ([#2907](https://github.com/EQEmu/Server/pull/2907)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute area events ([#2888](https://github.com/EQEmu/Server/pull/2888)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check merchant events exist before export and execute ([#2893](https://github.com/EQEmu/Server/pull/2893)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check spell or cast events exist before export and execute ([#2897](https://github.com/EQEmu/Server/pull/2897)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check task events exist before export and execute ([#2883](https://github.com/EQEmu/Server/pull/2883)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_CONNECT and EVENT_DISCONNECT ([#2913](https://github.com/EQEmu/Server/pull/2913)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* (Performance) Check event exists before export and execute EVENT_TEST_BUFF ([#2920](https://github.com/EQEmu/Server/pull/2920)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Add $target export to EVENT_INSPECT in Perl ([#2891](https://github.com/EQEmu/Server/pull/2891)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Add Additional XP Events EVENT_AA_EXP_GAIN, EVENT_EXP_GAIN ([#2865](https://github.com/EQEmu/Server/pull/2865)) ([Valorith](https://github.com/Valorith)) 2023-02-13
* Add EVENT_DESTROY_ITEM_CLIENT to Perl/Lua. ([#2871](https://github.com/EQEmu/Server/pull/2871)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Add EVENT_DROP_ITEM_CLIENT to Perl/Lua ([#2869](https://github.com/EQEmu/Server/pull/2869)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Add Recipe-based methods to Perl/Lua. ([#2844](https://github.com/EQEmu/Server/pull/2844)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-08
* Export $door to EVENT_CLICKDOOR in Perl ([#2861](https://github.com/EQEmu/Server/pull/2861)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-11
* Export $hate_entity to EVENT_HATE_LIST in Perl ([#2885](https://github.com/EQEmu/Server/pull/2885)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export $item and $augment to augment events in Perl ([#2895](https://github.com/EQEmu/Server/pull/2895)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export $item and $corpse to EVENT_LOOT and EVENT_LOOT_ZONE in Perl ([#2878](https://github.com/EQEmu/Server/pull/2878)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export $item to Client/Bot Equip Events in Perl ([#2860](https://github.com/EQEmu/Server/pull/2860)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-11
* Export $item to EVENT_DISCOVER_ITEM in Perl ([#2863](https://github.com/EQEmu/Server/pull/2863)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-11
* Export $item to EVENT_PLAYER_PICKUP in Perl. ([#2875](https://github.com/EQEmu/Server/pull/2875)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export $item to Fishing and Forage Events in Perl ([#2876](https://github.com/EQEmu/Server/pull/2876)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export $killed_npc to EVENT_NPC_SLAY to Perl ([#2879](https://github.com/EQEmu/Server/pull/2879)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export $object to EVENT_CLICK_OBJECT in Perl ([#2862](https://github.com/EQEmu/Server/pull/2862)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-11
* Export $spawned to EVENT_SPAWN_ZONE in Perl ([#2877](https://github.com/EQEmu/Server/pull/2877)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export target to EVENT_TARGET_CHANGE in Perl/Lua. ([#2870](https://github.com/EQEmu/Server/pull/2870)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Export targets to EVENT_CONSIDER and EVENT_CONSIDER_CORPSE ([#2908](https://github.com/EQEmu/Server/pull/2908)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13
* Fix SetSimpleRoamBox in Perl to have optional params again ([#2935](https://github.com/EQEmu/Server/pull/2935)) ([Akkadius](https://github.com/Akkadius)) 2023-02-15

### Rules

* Add Group/Raid Experience Rules ([#2850](https://github.com/EQEmu/Server/pull/2850)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-13

### Tradeskills

* Check if combine would result in lore conflict ([#2932](https://github.com/EQEmu/Server/pull/2932)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-16

### Windows

* Fix MSVC compilation bug via workaround ([#2926](https://github.com/EQEmu/Server/pull/2926)) ([Akkadius](https://github.com/Akkadius)) 2023-02-14

## [22.3.0] - 02/06/2023

### Bots

* Add GetAugmentIDsBySlotID & AddItem with table ref Methods. ([#2805](https://github.com/EQEmu/Server/pull/2805)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-29

### Commands

* #list now searches without case sensitivity ([#2825](https://github.com/EQEmu/Server/pull/2825)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06
* Remove extraneous else from #weather ([#2819](https://github.com/EQEmu/Server/pull/2819)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-01

### Crash

* Fix IsUnderwaterOnly crash where npc data references can be stale ([#2830](https://github.com/EQEmu/Server/pull/2830)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06
* Fix command crash with #npcedit weapon when second weapon not passed ni ([#2829](https://github.com/EQEmu/Server/pull/2829)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06
* Fix crash in bot command botdyearmor ([#2832](https://github.com/EQEmu/Server/pull/2832)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06

### DB Updates

* Add Windows MySQL path auto detection for users where the path is not found ([#2836](https://github.com/EQEmu/Server/pull/2836)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06

### Doors

* Have NPCs trigger double doors ([#2821](https://github.com/EQEmu/Server/pull/2821)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06
* Remove door dev tools spam on client controlled doors ([#2824](https://github.com/EQEmu/Server/pull/2824)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06

### Feature

* Add Min/Max Status to Merchants ([#2806](https://github.com/EQEmu/Server/pull/2806)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-29

### Fixes

* #reload aa will now refresh the AA table properly for every client when changes are made ([#2814](https://github.com/EQEmu/Server/pull/2814)) ([Natedog2012](https://github.com/Natedog2012)) 2023-01-31
* #reload static should now properly fill the entity_lists for… ([#2815](https://github.com/EQEmu/Server/pull/2815)) ([Natedog2012](https://github.com/Natedog2012)) 2023-01-31
* BuffLevelRestrictions were restricting group buffs if mob targeted ([#2809](https://github.com/EQEmu/Server/pull/2809)) ([noudess](https://github.com/noudess)) 2023-01-29
* Fix does_augment_fit_slot method. ([#2817](https://github.com/EQEmu/Server/pull/2817)) ([Aeadoin](https://github.com/Aeadoin)) 2023-02-01
* Fix NPC ghosting at safe coordinates ([#2823](https://github.com/EQEmu/Server/pull/2823)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06
* Fixing % based mob see invis ([#2802](https://github.com/EQEmu/Server/pull/2802)) ([fryguy503](https://github.com/fryguy503)) 2023-01-29
* Resolve issue with max buff count being 25 in ROF2. ([#2800](https://github.com/EQEmu/Server/pull/2800)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-28

### Hotfix

* Post revert build fix for https://github.com/EQEmu/Server/commit/54050924d81d1f83268fe01f9c2b36fe10626601  ([Akkadius](https://github.com/Akkadius)) 2023-02-01

### Lua

* Resolve stoi Exception ([#2736](https://github.com/EQEmu/Server/pull/2736)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06

### Pathing

* Improvements to handling tight corridors pathing, clipping detection and recovery ([#2826](https://github.com/EQEmu/Server/pull/2826)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06

### Quest API

* Add Augment Slot support to does_augment_fit ([#2813](https://github.com/EQEmu/Server/pull/2813)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-31
* Add EVENT_DAMAGE_GIVEN and EVENT_DAMAGE_TAKEN to Perl/Lua. ([#2804](https://github.com/EQEmu/Server/pull/2804)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-29
* Add EVENT_ITEM_CLICK_CLIENT and EVENT_ITEM_CLICK_CAST_CLIENT to Perl/Lua. ([#2810](https://github.com/EQEmu/Server/pull/2810)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-30
* Add EVENT_TASKACCEPTED to Player scope ([#2822](https://github.com/EQEmu/Server/pull/2822)) ([Valorith](https://github.com/Valorith)) 2023-02-06
* Add GetItemCooldown to return the time remaining on items… ([#2811](https://github.com/EQEmu/Server/pull/2811)) ([Natedog2012](https://github.com/Natedog2012)) 2023-01-30
* Add LDoN Methods to Perl/Lua ([#2799](https://github.com/EQEmu/Server/pull/2799)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-29
* Add Override Parameters to ScaleNPC() in Perl/Lua. ([#2816](https://github.com/EQEmu/Server/pull/2816)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-01
* Add rule AlternateAugmentationSealer for using a different bagtype ([#2831](https://github.com/EQEmu/Server/pull/2831)) ([Natedog2012](https://github.com/Natedog2012)) 2023-02-06
* Default ScaleNPC to always scale. ([#2818](https://github.com/EQEmu/Server/pull/2818)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-02-06

### Readme

* Update build badges with Drone  ([Akkadius](https://github.com/Akkadius)) 2023-01-29

### Rules

* Add rule to ignore name filter on chat channel creation. ([#2820](https://github.com/EQEmu/Server/pull/2820)) ([Valorith](https://github.com/Valorith)) 2023-02-06
* Added rule to bypass level based haste caps ([#2835](https://github.com/EQEmu/Server/pull/2835)) ([jcr4990](https://github.com/jcr4990)) 2023-02-06
* Fix rule updates that affected bot booting checks ([#2841](https://github.com/EQEmu/Server/pull/2841)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06

### Tasks

* Implement alternate currency rewards ([#2827](https://github.com/EQEmu/Server/pull/2827)) ([Akkadius](https://github.com/Akkadius)) 2023-02-06

## [22.2.0] - 01/27/2023

### Bots

* Add EVENT_UNEQUIP_ITEM_BOT & EVENT_EQUIP_ITEM_BOT ([#2796](https://github.com/EQEmu/Server/pull/2796)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-27
* ^create and ^viewcombos popup messages fix. ([#2797](https://github.com/EQEmu/Server/pull/2797)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-26

### Code Cleanup

* Cleanup #door Command. ([#2783](https://github.com/EQEmu/Server/pull/2783)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-24

### Crash

* Fix crash issue with log formatting during character creation ([#2798](https://github.com/EQEmu/Server/pull/2798)) ([Akkadius](https://github.com/Akkadius)) 2023-01-27

### Feature

* ResetItemCooldown added to lua/perl and fix item re-cast times to show properly ([#2793](https://github.com/EQEmu/Server/pull/2793)) ([Natedog2012](https://github.com/Natedog2012)) 2023-01-26

### Git

* Add CMake Files to .gitignore ([#2792](https://github.com/EQEmu/Server/pull/2792)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-25

## [22.1.2] - 01/24/2023

### CI/CD

* Build / Release Pipeline Changes ([#2788](https://github.com/EQEmu/Server/pull/2788)) ([Akkadius](https://github.com/Akkadius)) 2023-01-24

### Code Cleanup

* Cleanup #door Command. ([#2783](https://github.com/EQEmu/Server/pull/2783)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-24

### Crash

* Fix rarer world crash issue where scheduler database was not available ([#2789](https://github.com/EQEmu/Server/pull/2789)) ([Akkadius](https://github.com/Akkadius)) 2023-01-24

### Fixes

* Fix nullptr spell in BCSpells::Load() ([#2790](https://github.com/EQEmu/Server/pull/2790)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-24
* Remove duplicate logic in GetActSpellHealing reducing HOT criticals ([#2786](https://github.com/EQEmu/Server/pull/2786)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-24

## [22.1.1] - 01/23/2023

### Fixes

* Fix botgrouplist to display unique entries. ([#2785](https://github.com/EQEmu/Server/pull/2785)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-23
* Fix scenario where dereferenced object could be null. ([#2784](https://github.com/EQEmu/Server/pull/2784)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-23

## [22.1.0] - 01/22/2023

This is a first release using the new build system. Changelog entry representative of last year. Subsequent releases will consist of incremental changes since the last release.

### AA

* Fix AA tables dump ([#2769](https://github.com/EQEmu/Server/pull/2769)) ([Akkadius](https://github.com/Akkadius)) 2023-01-22

### Appveyor

* Remove bots preprocessor  ([Akkadius](https://github.com/Akkadius)) 2023-01-20

### Bot/Merc

* Cleanup methods, and virtual overrides. ([#2734](https://github.com/EQEmu/Server/pull/2734)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-15

### Bots

* Add Bot Command Reloading ([#2773](https://github.com/EQEmu/Server/pull/2773)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-22
* Add Bot-specific Spell Settings. ([#2553](https://github.com/EQEmu/Server/pull/2553)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-27
* Add Buff support for Bards under AI_IdleCastChecks ([#2590](https://github.com/EQEmu/Server/pull/2590)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-28
* Add Data Bucket support to Bot Spell Entries. ([#2505](https://github.com/EQEmu/Server/pull/2505)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-06
* Add EVENT_TRADE Support to Bots. ([#2560](https://github.com/EQEmu/Server/pull/2560)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-25
* Add Event_Trade Support for ^inventorygive Command ([#2628](https://github.com/EQEmu/Server/pull/2628)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-11
* Add Expansion Bitmask Quest APIs. ([#2523](https://github.com/EQEmu/Server/pull/2523)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-16
* Add GetBotOwnerByBotID Method ([#2715](https://github.com/EQEmu/Server/pull/2715)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-11
* Add Melee Support for Casting, Cleanup Bot Casting Logic ([#2571](https://github.com/EQEmu/Server/pull/2571)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-25
* Add Quest API Methods ([#2631](https://github.com/EQEmu/Server/pull/2631)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-12
* Add Quest API Support for Limits. ([#2522](https://github.com/EQEmu/Server/pull/2522)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-17
* Add Rule Allowing Bots to Equip Any Race Items ([#2578](https://github.com/EQEmu/Server/pull/2578)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-26
* Add Support for AA bonuses that were missing. ([#2764](https://github.com/EQEmu/Server/pull/2764)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-20
* Add Support for Bots to receive Auras, and other AoE Buffs. ([#2586](https://github.com/EQEmu/Server/pull/2586)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-27
* Add Virtual Override for Bot::Attack ([#2771](https://github.com/EQEmu/Server/pull/2771)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-20
* Add give/remove saylinks to ^itemuse. ([#2503](https://github.com/EQEmu/Server/pull/2503)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-30
* Add support for Bot scripting. ([#2515](https://github.com/EQEmu/Server/pull/2515)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-17
* Apply Spells:IgnoreSpellDmgLvlRestriction to bots ([#2024](https://github.com/EQEmu/Server/pull/2024)) ([catapultam-habeo](https://github.com/catapultam-habeo)) 2022-03-07
* Bot::PerformTradeWithClient Cleanup. ([#2084](https://github.com/EQEmu/Server/pull/2084)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-01
* Cleanup Bot Spell Functions, reduce reliance on NPC Functions/Attributes ([#2495](https://github.com/EQEmu/Server/pull/2495)) ([Aeadoin](https://github.com/Aeadoin)) 2022-10-29
* Cleanup Fast Rest Regen ([#2626](https://github.com/EQEmu/Server/pull/2626)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-07
* Cleanup Say Event Parse. ([#2557](https://github.com/EQEmu/Server/pull/2557)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-20
* Cleanup Spell Settings Commands ([#2607](https://github.com/EQEmu/Server/pull/2607)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-04
* Cleanup ^inventoryremove, ^inventorylist, and ^list Commands and bot groups. ([#2273](https://github.com/EQEmu/Server/pull/2273)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-03
* Cleanup and remove preprocessors. ([#2757](https://github.com/EQEmu/Server/pull/2757)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-20
* Cleanup various Bot Spell Focus methods ([#2649](https://github.com/EQEmu/Server/pull/2649)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-16
* Convert Load, Save, SaveNew, and Delete to Repositories. ([#2614](https://github.com/EQEmu/Server/pull/2614)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-04
* Expanded Bot Spell Settings List. ([#2606](https://github.com/EQEmu/Server/pull/2606)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-03
* Fix Bot Spell Type "In Combat Buffs" ([#2711](https://github.com/EQEmu/Server/pull/2711)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-08
* Fix Gender not saving as GetBaseGender on BotSave ([#2639](https://github.com/EQEmu/Server/pull/2639)) ([nytmyr](https://github.com/nytmyr)) 2022-12-13
* Fix Slow Query in QueryNameAvailablity ([#2781](https://github.com/EQEmu/Server/pull/2781)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-22
* Fix ^dyearmor command math. ([#2081](https://github.com/EQEmu/Server/pull/2081)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-04-30
* Fix bot spawn when bot id = char_id ([#1984](https://github.com/EQEmu/Server/pull/1984)) ([neckkola](https://github.com/neckkola)) 2022-03-07
* Hotfix for possible crash. ([#2539](https://github.com/EQEmu/Server/pull/2539)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Melee Bot Support for Spell Settings Commands ([#2599](https://github.com/EQEmu/Server/pull/2599)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-01
* Move Bot Spell Loading process to constructor from calcbotstats() ([#2583](https://github.com/EQEmu/Server/pull/2583)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-27
* Optimize inventory loading. ([#2588](https://github.com/EQEmu/Server/pull/2588)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-28
* Post pre-processor fixes ([#2770](https://github.com/EQEmu/Server/pull/2770)) ([Akkadius](https://github.com/Akkadius)) 2023-01-20
* Resolve incorrect values on Bot Creation ([#2644](https://github.com/EQEmu/Server/pull/2644)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-14
* Restrict Bot Groups from spawning while Feigned. ([#2761](https://github.com/EQEmu/Server/pull/2761)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-19
* Save Bot Toggle Archer Setting between Loads. ([#2612](https://github.com/EQEmu/Server/pull/2612)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-04
* Update Bot Heal & Damage methods to more closely match Clients + Bugfixes ([#2045](https://github.com/EQEmu/Server/pull/2045)) ([catapultam-habeo](https://github.com/catapultam-habeo)) 2022-03-11
* Update Bot Logic to ignore ST_TargetsTarget when buffing ([#2584](https://github.com/EQEmu/Server/pull/2584)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-27

### C++20

* Arithmetic on different enums is deprecated ([#2752](https://github.com/EQEmu/Server/pull/2752)) ([mackal](https://github.com/mackal)) 2023-01-17
* Enable C++20 + Fixes + FMT 9.1 ([#2664](https://github.com/EQEmu/Server/pull/2664)) ([Akkadius](https://github.com/Akkadius)) 2022-12-21

### Code

* Removed vscode setting ([#2753](https://github.com/EQEmu/Server/pull/2753)) ([xackery](https://github.com/xackery)) 2023-01-17

### Code Cleanup

* Add Validation to varchar number item fields. ([#2241](https://github.com/EQEmu/Server/pull/2241)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-04
* Cleanup #kick message. ([#2164](https://github.com/EQEmu/Server/pull/2164)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-10
* Cleanup Haste references and Lua API calls for unsigned to signed. ([#2240](https://github.com/EQEmu/Server/pull/2240)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-04
* Cleanup code smells and compiler warnings in common/shareddb ([#2270](https://github.com/EQEmu/Server/pull/2270)) ([Quintinon](https://github.com/Quintinon)) 2022-07-03
* Cleanup magic numbers ([#2662](https://github.com/EQEmu/Server/pull/2662)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-20
* Cleanup spell and max level bucket logic. ([#2181](https://github.com/EQEmu/Server/pull/2181)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-28
* Extra Space in NPC::AISpellsList(). ([#2555](https://github.com/EQEmu/Server/pull/2555)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-20
* Fix unintended copies in zone/zonedb.cpp by changing auto to auto& ([#2271](https://github.com/EQEmu/Server/pull/2271)) ([Quintinon](https://github.com/Quintinon)) 2022-07-03
* Make use of std::abs where possible. ([#2739](https://github.com/EQEmu/Server/pull/2739)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-15
* Merge Client::Attack and Bot::Attack into Mob::Attack ([#2756](https://github.com/EQEmu/Server/pull/2756)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-20
* Move Client::Undye() to client.cpp from #path Command. ([#2188](https://github.com/EQEmu/Server/pull/2188)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-21
* Possible issues with variable/parameter name equality. ([#2161](https://github.com/EQEmu/Server/pull/2161)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-10
* Quest API push methods using invalid types. ([#2172](https://github.com/EQEmu/Server/pull/2172)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-16
* Remove Unused EQEMU_DEPOP_INVALIDATES_CACHE ([#2292](https://github.com/EQEmu/Server/pull/2292)) ([Akkadius](https://github.com/Akkadius)) 2022-07-14
* Remove this-> in code where its implied ([#2088](https://github.com/EQEmu/Server/pull/2088)) ([Akkadius](https://github.com/Akkadius)) 2022-05-01
* Remove unused basic_functions.h ([#2729](https://github.com/EQEmu/Server/pull/2729)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-13
* Remove unused maxskill.h. ([#2728](https://github.com/EQEmu/Server/pull/2728)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-13
* Remove unused methods. ([#2171](https://github.com/EQEmu/Server/pull/2171)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-15
* Remove unusued Max Item ID Constant ([#2528](https://github.com/EQEmu/Server/pull/2528)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-08
* Remove use of bzero since it is deprecated for memset ([#2295](https://github.com/EQEmu/Server/pull/2295)) ([Akkadius](https://github.com/Akkadius)) 2022-07-14
* Resharper Warnings ([#2235](https://github.com/EQEmu/Server/pull/2235)) ([Quintinon](https://github.com/Quintinon)) 2022-06-01
* Resolve some warnings in loginserver/world_server.cpp ([#2347](https://github.com/EQEmu/Server/pull/2347)) ([mackal](https://github.com/mackal)) 2022-07-31
* Rework Lua QuestReward to not use try/catch blocks ([#2417](https://github.com/EQEmu/Server/pull/2417)) ([mackal](https://github.com/mackal)) 2022-09-03
* Send eqstr message in AddAAPoints ([#2507](https://github.com/EQEmu/Server/pull/2507)) ([hgtw](https://github.com/hgtw)) 2022-10-29
* Update to EQEmu #2253 to clean up message strings ([#2279](https://github.com/EQEmu/Server/pull/2279)) ([fryguy503](https://github.com/fryguy503)) 2022-07-03
* Zone Data Loading Refactor ([#2388](https://github.com/EQEmu/Server/pull/2388)) ([Akkadius](https://github.com/Akkadius)) 2022-09-01

### Commands

* #bind Typo. ([#2196](https://github.com/EQEmu/Server/pull/2196)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-23
* #ginfo Cleanup. ([#1955](https://github.com/EQEmu/Server/pull/1955)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-03
* #reload Command Overhaul. ([#2162](https://github.com/EQEmu/Server/pull/2162)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-10
* #reload level_mods could cause Non-Booted zones to crash. ([#2670](https://github.com/EQEmu/Server/pull/2670)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-24
* Add #bugs Command. ([#2559](https://github.com/EQEmu/Server/pull/2559)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Add #feature Command. ([#2142](https://github.com/EQEmu/Server/pull/2142)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Add #findcharacter Command. ([#2692](https://github.com/EQEmu/Server/pull/2692)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-03
* Add #findrecipe and #viewrecipe Commands. ([#2401](https://github.com/EQEmu/Server/pull/2401)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-31
* Add #setanon Command ([#2690](https://github.com/EQEmu/Server/pull/2690)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-03
* Add #suspendmulti Command. ([#2619](https://github.com/EQEmu/Server/pull/2619)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-11
* Add BestZ and Region Data to #loc ([#2245](https://github.com/EQEmu/Server/pull/2245)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-05
* Add additional #peqzone functionality. ([#2085](https://github.com/EQEmu/Server/pull/2085)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-01
* Add max_hp back to #modifynpcstat command. ([#2638](https://github.com/EQEmu/Server/pull/2638)) ([nytmyr](https://github.com/nytmyr)) 2022-12-13
* Adding movespeed to #showstats output ([#2596](https://github.com/EQEmu/Server/pull/2596)) ([fryguy503](https://github.com/fryguy503)) 2022-11-30
* Bug fix for #logs command. ([#2008](https://github.com/EQEmu/Server/pull/2008)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-17
* Cleanup #ai Command. ([#1980](https://github.com/EQEmu/Server/pull/1980)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-11
* Cleanup #appearanceeffects Command. ([#2777](https://github.com/EQEmu/Server/pull/2777)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-22
* Cleanup #attack Command. ([#2103](https://github.com/EQEmu/Server/pull/2103)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-04
* Cleanup #ban, #ipban, #flag, #kick, #setlsinfo, and #setpass Commands. ([#2104](https://github.com/EQEmu/Server/pull/2104)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-08
* Cleanup #chat Command. ([#2581](https://github.com/EQEmu/Server/pull/2581)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-27
* Cleanup #corpsefix Command. ([#2197](https://github.com/EQEmu/Server/pull/2197)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Cleanup #cvs Command. ([#2153](https://github.com/EQEmu/Server/pull/2153)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-08
* Cleanup #date Command. ([#2228](https://github.com/EQEmu/Server/pull/2228)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-01
* Cleanup #dbspawn2 Command. ([#2493](https://github.com/EQEmu/Server/pull/2493)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-30
* Cleanup #delacct Command. ([#2567](https://github.com/EQEmu/Server/pull/2567)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Cleanup #depop Command. ([#2536](https://github.com/EQEmu/Server/pull/2536)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Cleanup #depopzone Command. ([#2537](https://github.com/EQEmu/Server/pull/2537)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Cleanup #devtools Command. ([#2538](https://github.com/EQEmu/Server/pull/2538)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Cleanup #doanim Command. ([#2540](https://github.com/EQEmu/Server/pull/2540)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Cleanup #emote Command. ([#2535](https://github.com/EQEmu/Server/pull/2535)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Cleanup #emotesearch and #emoteview Command. ([#2494](https://github.com/EQEmu/Server/pull/2494)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-30
* Cleanup #emptyinventory Command. ([#2219](https://github.com/EQEmu/Server/pull/2219)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-29
* Cleanup #findaliases and #help Commands. ([#2204](https://github.com/EQEmu/Server/pull/2204)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Cleanup #findclass and #findrace Commands. ([#2211](https://github.com/EQEmu/Server/pull/2211)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Cleanup #flagedit Command. ([#1968](https://github.com/EQEmu/Server/pull/1968)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Cleanup #freeze and #unfreeze Commands. ([#2102](https://github.com/EQEmu/Server/pull/2102)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-04
* Cleanup #gassign Command. ([#2101](https://github.com/EQEmu/Server/pull/2101)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #gearup Command. ([#2589](https://github.com/EQEmu/Server/pull/2589)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-27
* Cleanup #getvariable Command. ([#2100](https://github.com/EQEmu/Server/pull/2100)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-04
* Cleanup #guild Command ([#2693](https://github.com/EQEmu/Server/pull/2693)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-04
* Cleanup #hatelist Command. ([#1976](https://github.com/EQEmu/Server/pull/1976)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Cleanup #heromodel Command. ([#2566](https://github.com/EQEmu/Server/pull/2566)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Cleanup #kill Command. ([#2195](https://github.com/EQEmu/Server/pull/2195)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-23
* Cleanup #level Command. ([#2203](https://github.com/EQEmu/Server/pull/2203)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Cleanup #logs Command. ([#1969](https://github.com/EQEmu/Server/pull/1969)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Cleanup #makepet Command. ([#2105](https://github.com/EQEmu/Server/pull/2105)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #modifynpcstat Command. ([#2499](https://github.com/EQEmu/Server/pull/2499)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-30
* Cleanup #motd Command. ([#2190](https://github.com/EQEmu/Server/pull/2190)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-23
* Cleanup #name Command. ([#1977](https://github.com/EQEmu/Server/pull/1977)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Cleanup #netstats Command. ([#1970](https://github.com/EQEmu/Server/pull/1970)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Cleanup #npcedit Command. ([#2582](https://github.com/EQEmu/Server/pull/2582)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-27
* Cleanup #npcedit, #lastname, #title, and #titlesuffix Commands. ([#2215](https://github.com/EQEmu/Server/pull/2215)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-28
* Cleanup #npceditmass command. ([#1957](https://github.com/EQEmu/Server/pull/1957)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-03
* Cleanup #npcemote Command. ([#2106](https://github.com/EQEmu/Server/pull/2106)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #npcloot Command. ([#1974](https://github.com/EQEmu/Server/pull/1974)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-11
* Cleanup #npcsay and #npcshout Commands. ([#2107](https://github.com/EQEmu/Server/pull/2107)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #npcspecialattk Command. ([#2108](https://github.com/EQEmu/Server/pull/2108)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #npctype_cache Command. ([#2109](https://github.com/EQEmu/Server/pull/2109)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #npctypespawn Command. ([#2110](https://github.com/EQEmu/Server/pull/2110)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #nudge Command. ([#2220](https://github.com/EQEmu/Server/pull/2220)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-29
* Cleanup #oocmute Command. ([#2191](https://github.com/EQEmu/Server/pull/2191)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Cleanup #opcode Command. ([#2547](https://github.com/EQEmu/Server/pull/2547)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-16
* Cleanup #profanity Command. ([#2113](https://github.com/EQEmu/Server/pull/2113)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #push Command. ([#2114](https://github.com/EQEmu/Server/pull/2114)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #qglobal Command. ([#2115](https://github.com/EQEmu/Server/pull/2115)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #randomizefeatures Command. ([#2118](https://github.com/EQEmu/Server/pull/2118)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #refreshgroup Command. ([#2119](https://github.com/EQEmu/Server/pull/2119)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadaa Command. ([#2120](https://github.com/EQEmu/Server/pull/2120)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadallrules Command. ([#2121](https://github.com/EQEmu/Server/pull/2121)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadlevelmods Command. ([#2122](https://github.com/EQEmu/Server/pull/2122)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadmerchants Command. ([#2123](https://github.com/EQEmu/Server/pull/2123)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadperlexportsettings Command. ([#2124](https://github.com/EQEmu/Server/pull/2124)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadrulesworld Command. ([#2128](https://github.com/EQEmu/Server/pull/2128)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadstatic Command. ([#2130](https://github.com/EQEmu/Server/pull/2130)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadtitles Command. ([#2125](https://github.com/EQEmu/Server/pull/2125)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadtraps Command. ([#2126](https://github.com/EQEmu/Server/pull/2126)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadworld and #repop Command. ([#2127](https://github.com/EQEmu/Server/pull/2127)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #reloadzps Command. ([#2129](https://github.com/EQEmu/Server/pull/2129)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #resetaa Command. ([#2132](https://github.com/EQEmu/Server/pull/2132)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #resetaa_timer Command. ([#2131](https://github.com/EQEmu/Server/pull/2131)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #resetdisc_timer Command. ([#2133](https://github.com/EQEmu/Server/pull/2133)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #revoke Command. ([#2134](https://github.com/EQEmu/Server/pull/2134)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #roambox Command. ([#2135](https://github.com/EQEmu/Server/pull/2135)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #rules Command. ([#2593](https://github.com/EQEmu/Server/pull/2593)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-10
* Cleanup #save Command. ([#2136](https://github.com/EQEmu/Server/pull/2136)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #scale Command. ([#2591](https://github.com/EQEmu/Server/pull/2591)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-05
* Cleanup #scribespell and #scribespells Commands. ([#2534](https://github.com/EQEmu/Server/pull/2534)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Cleanup #sensetrap Command. ([#2137](https://github.com/EQEmu/Server/pull/2137)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #serverinfo Command. ([#2568](https://github.com/EQEmu/Server/pull/2568)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Cleanup #serverrules Command. ([#2139](https://github.com/EQEmu/Server/pull/2139)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #setlanguage Command. ([#2464](https://github.com/EQEmu/Server/pull/2464)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-13
* Cleanup #setskillall Command. ([#1992](https://github.com/EQEmu/Server/pull/1992)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-15
* Cleanup #shownpcgloballoot and #showzonegloballoot Command. ([#2141](https://github.com/EQEmu/Server/pull/2141)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #showskills Command. ([#1994](https://github.com/EQEmu/Server/pull/1994)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-15
* Cleanup #spawneditmass Command. ([#2229](https://github.com/EQEmu/Server/pull/2229)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-04
* Cleanup #spawnfix Command. ([#2143](https://github.com/EQEmu/Server/pull/2143)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #spawnstatus Command. ([#2144](https://github.com/EQEmu/Server/pull/2144)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #summon Command. ([#2145](https://github.com/EQEmu/Server/pull/2145)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-06
* Cleanup #summonburiedplayercorpse Command. ([#2146](https://github.com/EQEmu/Server/pull/2146)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #suspend Command. ([#2564](https://github.com/EQEmu/Server/pull/2564)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Cleanup #task Command. ([#2071](https://github.com/EQEmu/Server/pull/2071)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-04-14
* Cleanup #time and #timezone Command. ([#2147](https://github.com/EQEmu/Server/pull/2147)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #timers Command. ([#2562](https://github.com/EQEmu/Server/pull/2562)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Cleanup #trapinfo Command. ([#2148](https://github.com/EQEmu/Server/pull/2148)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #ucs Command. ([#2149](https://github.com/EQEmu/Server/pull/2149)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Cleanup #undye and #undyeme Commands. ([#1966](https://github.com/EQEmu/Server/pull/1966)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Cleanup #unscribespell Command. ([#1998](https://github.com/EQEmu/Server/pull/1998)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-16
* Cleanup #untraindisc Command. ([#1996](https://github.com/EQEmu/Server/pull/1996)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-16
* Cleanup #version Command. ([#1967](https://github.com/EQEmu/Server/pull/1967)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Cleanup #worldwide command. ([#2021](https://github.com/EQEmu/Server/pull/2021)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-01
* Cleanup #xtargets Command. ([#2545](https://github.com/EQEmu/Server/pull/2545)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-17
* Cleanup #zone and #zoneinstance Commands. ([#2202](https://github.com/EQEmu/Server/pull/2202)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Command Status Reload and Helper Method ([#2377](https://github.com/EQEmu/Server/pull/2377)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-20
* Consolidate #lock and #unlock Commands into #serverlock. ([#2193](https://github.com/EQEmu/Server/pull/2193)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-23
* Fix #copycharacter command crash ([#2446](https://github.com/EQEmu/Server/pull/2446)) ([Akkadius](https://github.com/Akkadius)) 2022-09-25
* Fix #killallnpcs from crashing ([#2037](https://github.com/EQEmu/Server/pull/2037)) ([Akkadius](https://github.com/Akkadius)) 2022-03-07
* Fix Flymode Command Help Prompt ([#2669](https://github.com/EQEmu/Server/pull/2669)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-23
* Fix typos in #ban and #ipban Commands. ([#2209](https://github.com/EQEmu/Server/pull/2209)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-26
* Make #damage require a target ([#2426](https://github.com/EQEmu/Server/pull/2426)) ([hgtw](https://github.com/hgtw)) 2022-09-05
* Nested Command Aliases ([#2636](https://github.com/EQEmu/Server/pull/2636)) ([Akkadius](https://github.com/Akkadius)) 2022-12-15
* Remove #guildapprove, #guildcreate, and #guildlist Commands ([#2775](https://github.com/EQEmu/Server/pull/2775)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-22
* Remove #iteminfo Command. ([#2565](https://github.com/EQEmu/Server/pull/2565)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Remove #profiledump and #profilereset Commands. ([#2546](https://github.com/EQEmu/Server/pull/2546)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-16
* Remove #undyeme Command. ([#2776](https://github.com/EQEmu/Server/pull/2776)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-22
* Remove unused #bestz and #pf Commands. ([#2112](https://github.com/EQEmu/Server/pull/2112)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Remove unused/broken #deletegraveyard and #setgraveyard Commands. ([#2198](https://github.com/EQEmu/Server/pull/2198)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-23

### Diawind

* Plus sign markdown fix ([#2727](https://github.com/EQEmu/Server/pull/2727)) ([Akkadius](https://github.com/Akkadius)) 2023-01-12

### Feature

* AA Cap Limit ([#2423](https://github.com/EQEmu/Server/pull/2423)) ([fryguy503](https://github.com/fryguy503)) 2022-10-13
* Add "Keeps Sold Items" Flag to NPCs ([#2671](https://github.com/EQEmu/Server/pull/2671)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-25
* Add Experience Gain Toggle. ([#2676](https://github.com/EQEmu/Server/pull/2676)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-30
* Add Guild Chat to Console. ([#2387](https://github.com/EQEmu/Server/pull/2387)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-22
* Add Hate Override for Heals ([#2485](https://github.com/EQEmu/Server/pull/2485)) ([Aeadoin](https://github.com/Aeadoin)) 2022-10-14
* Add Rule to Disable Group EXP Modifier. ([#2741](https://github.com/EQEmu/Server/pull/2741)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-15
* Add Support for "Show Mine Only" Filters ([#2484](https://github.com/EQEmu/Server/pull/2484)) ([Aeadoin](https://github.com/Aeadoin)) 2022-10-13
* Add Type 49545 to Spell Resistrictions ([#2436](https://github.com/EQEmu/Server/pull/2436)) ([Aeadoin](https://github.com/Aeadoin)) 2022-09-20
* Add humanoid and non-wielded restrictions to pick pocket ([#2276](https://github.com/EQEmu/Server/pull/2276)) ([noudess](https://github.com/noudess)) 2022-07-03
* Add player /inspect quest event ([#2508](https://github.com/EQEmu/Server/pull/2508)) ([hgtw](https://github.com/hgtw)) 2022-10-29
* Add special ability to block /open ([#2506](https://github.com/EQEmu/Server/pull/2506)) ([hgtw](https://github.com/hgtw)) 2022-10-29
* Allow Focus Effects to be Filtered out. ([#2447](https://github.com/EQEmu/Server/pull/2447)) ([Aeadoin](https://github.com/Aeadoin)) 2022-09-25
* Allow pets to zone with permanent (buffdurationformula 50) buffs to maintain them through zone transitions ([#2035](https://github.com/EQEmu/Server/pull/2035)) ([catapultam-habeo](https://github.com/catapultam-habeo)) 2022-03-07
* Bind Wound and Forage while mounted. ([#2257](https://github.com/EQEmu/Server/pull/2257)) ([fryguy503](https://github.com/fryguy503)) 2022-07-03
* Change #scribespells to be aware of spellgroups & ranks ([#2501](https://github.com/EQEmu/Server/pull/2501)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-06
* Change GetSkillDmgAmt to int32 ([#2364](https://github.com/EQEmu/Server/pull/2364)) ([Aeadoin](https://github.com/Aeadoin)) 2022-08-10
* Change Lifetap Emotes to be filterable. ([#2454](https://github.com/EQEmu/Server/pull/2454)) ([Aeadoin](https://github.com/Aeadoin)) 2022-09-29
* Change Mana Costs to use Signed Int ([#2384](https://github.com/EQEmu/Server/pull/2384)) ([Aeadoin](https://github.com/Aeadoin)) 2022-08-21
* Change mana_used to int32 ([#2321](https://github.com/EQEmu/Server/pull/2321)) ([Aeadoin](https://github.com/Aeadoin)) 2022-07-30
* Client Checksum Verification (Resubmit old 1678) ([#1922](https://github.com/EQEmu/Server/pull/1922)) ([noudess](https://github.com/noudess)) 2022-03-07
* EQ2-style implied targeting for spells. ([#2032](https://github.com/EQEmu/Server/pull/2032)) ([catapultam-habeo](https://github.com/catapultam-habeo)) 2022-03-07
* Faction Association ([#2408](https://github.com/EQEmu/Server/pull/2408)) ([mackal](https://github.com/mackal)) 2022-09-03
* GM State Change Persistance ([#2328](https://github.com/EQEmu/Server/pull/2328)) ([fryguy503](https://github.com/fryguy503)) 2022-07-31
* Implement Heroic Strikethrough to NPCs ([#2395](https://github.com/EQEmu/Server/pull/2395)) ([Aeadoin](https://github.com/Aeadoin)) 2022-08-31
* Implement OP_CashReward ([#2307](https://github.com/EQEmu/Server/pull/2307)) ([mackal](https://github.com/mackal)) 2022-07-15
* Instance Version Specific Experience Modifiers ([#2376](https://github.com/EQEmu/Server/pull/2376)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-20
* NPCs with bows and arrows do ranged attacks ([#2322](https://github.com/EQEmu/Server/pull/2322)) ([mackal](https://github.com/mackal)) 2022-07-30
* Soft Delete Bots on Character Soft Delete ([#2467](https://github.com/EQEmu/Server/pull/2467)) ([Aeadoin](https://github.com/Aeadoin)) 2022-10-13
* Spell Ranks will now work with AllowSpellMemorizeFromItem Rule ([#2475](https://github.com/EQEmu/Server/pull/2475)) ([Aeadoin](https://github.com/Aeadoin)) 2022-10-13
* Update HateMod used by SPA 114 to Int32. ([#2428](https://github.com/EQEmu/Server/pull/2428)) ([Aeadoin](https://github.com/Aeadoin)) 2022-09-08

### Fixes

* #npcstats command displaying incorrect faction ([#2710](https://github.com/EQEmu/Server/pull/2710)) ([noudess](https://github.com/noudess)) 2023-01-08
* #peqzone no longer bypass Handle_OP_ZoneChange ([#2063](https://github.com/EQEmu/Server/pull/2063)) ([Natedog2012](https://github.com/Natedog2012)) 2022-03-19
* #scribespells triggered error on mysql keyword rank ([#2779](https://github.com/EQEmu/Server/pull/2779)) ([noudess](https://github.com/noudess)) 2023-01-21
* #tune command various fixes ([#2046](https://github.com/EQEmu/Server/pull/2046)) ([KayenEQ](https://github.com/KayenEQ)) 2022-03-11
* Add Complete Heal Spell back to IsCompleteHealSpell Method ([#2722](https://github.com/EQEmu/Server/pull/2722)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-11
* Add SE_MakeDrunk to avoid error message. ([#2601](https://github.com/EQEmu/Server/pull/2601)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-01
* Add omitted function call in UCS ([#2768](https://github.com/EQEmu/Server/pull/2768)) ([Valorith](https://github.com/Valorith)) 2023-01-20
* Add required distance to CoTH before aggro wipe ([#2253](https://github.com/EQEmu/Server/pull/2253)) ([fryguy503](https://github.com/fryguy503)) 2022-07-03
* Adjustment for nullptr crash ([#2232](https://github.com/EQEmu/Server/pull/2232)) ([Akkadius](https://github.com/Akkadius)) 2022-06-01
* Alleviate some lag with crosszone/worldwide spell casting. ([#2016](https://github.com/EQEmu/Server/pull/2016)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-21
* Allow High Level Spells to be Unmemorized. ([#2641](https://github.com/EQEmu/Server/pull/2641)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-14
* Allow Songs to be scribed from scrolls ([#2460](https://github.com/EQEmu/Server/pull/2460)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-12
* AltCurrencySelectItemReply_Struct was not handled correctly. ([#2702](https://github.com/EQEmu/Server/pull/2702)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-04
* Any use of TempName left old clean_name. ([#1946](https://github.com/EQEmu/Server/pull/1946)) ([noudess](https://github.com/noudess)) 2022-01-26
* Avoid erase in discord queue range loop ([#2411](https://github.com/EQEmu/Server/pull/2411)) ([hgtw](https://github.com/hgtw)) 2022-09-03
* Bandolier didn't recognize source weapon on cursor ([#2026](https://github.com/EQEmu/Server/pull/2026)) ([noudess](https://github.com/noudess)) 2022-03-07
* Bard Invisible causing display issues. ([#2067](https://github.com/EQEmu/Server/pull/2067)) ([KayenEQ](https://github.com/KayenEQ)) 2022-04-01
* Bard update fixes 1 ([#1982](https://github.com/EQEmu/Server/pull/1982)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-09
* Bazaar Search MYSQL Error ([#2252](https://github.com/EQEmu/Server/pull/2252)) ([fryguy503](https://github.com/fryguy503)) 2022-06-08
* Blocked spells max spell id increased ([#2207](https://github.com/EQEmu/Server/pull/2207)) ([Isaaru](https://github.com/Isaaru)) 2022-05-25
* Boats should never get FixZ'd ([#2246](https://github.com/EQEmu/Server/pull/2246)) ([noudess](https://github.com/noudess)) 2022-07-02
* Clamp Item Ldon Sell Back Rates. ([#2592](https://github.com/EQEmu/Server/pull/2592)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-30
* Clear title/suffix bug fix. ([#2068](https://github.com/EQEmu/Server/pull/2068)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-04-02
* Correct (probably) unintended bitwise AND instead of logical AND ([#2239](https://github.com/EQEmu/Server/pull/2239)) ([Quintinon](https://github.com/Quintinon)) 2022-06-02
* Correct type signed/unsigned int when reading item from database in shareddb ([#2269](https://github.com/EQEmu/Server/pull/2269)) ([Quintinon](https://github.com/Quintinon)) 2022-06-15
* Data Bucket Permanent Duration String ([#2624](https://github.com/EQEmu/Server/pull/2624)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-06
* Delete NpcType Struct returned by Bot::CreateDefaultNPCTypeStructForBot() when unused ([#2267](https://github.com/EQEmu/Server/pull/2267)) ([Quintinon](https://github.com/Quintinon)) 2022-06-18
* Do not allow /open to be used on traps or auras, causes crash ([#1951](https://github.com/EQEmu/Server/pull/1951)) ([KayenEQ](https://github.com/KayenEQ)) 2022-01-30
* Doors::GetSize() Perl Croak Typo. ([#2027](https://github.com/EQEmu/Server/pull/2027)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-04
* EVENT_ENTER_AREA/EVENT_LEAVE_AREA. ([#2698](https://github.com/EQEmu/Server/pull/2698)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-02
* Edge case AA reset timer issue fixes ([#1995](https://github.com/EQEmu/Server/pull/1995)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-14
* Fix #door Save ([#2699](https://github.com/EQEmu/Server/pull/2699)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-02
* Fix #findaa and GetAAName(). ([#2774](https://github.com/EQEmu/Server/pull/2774)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-22
* Fix #zone 0. ([#2691](https://github.com/EQEmu/Server/pull/2691)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-01
* Fix Aug Clicks where item has no click effect. ([#2725](https://github.com/EQEmu/Server/pull/2725)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-12
* Fix Bot "Failed to Load" Messages. ([#2719](https://github.com/EQEmu/Server/pull/2719)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-11
* Fix Bot Group Loading ([#2780](https://github.com/EQEmu/Server/pull/2780)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-22
* Fix Bot ^spellsettingsadd command ([#2603](https://github.com/EQEmu/Server/pull/2603)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-01
* Fix Duplicate Silent Saylink Messages ([#2386](https://github.com/EQEmu/Server/pull/2386)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-22
* Fix EntityList::GetBotListByCharacterID() ([#2569](https://github.com/EQEmu/Server/pull/2569)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Fix Flag Updating with SetGMStatus() in Lua. ([#2554](https://github.com/EQEmu/Server/pull/2554)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-20
* Fix Group XP not working. ([#2748](https://github.com/EQEmu/Server/pull/2748)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-17
* Fix HP Regen Per Second. ([#2206](https://github.com/EQEmu/Server/pull/2206)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-25
* Fix IDFile Crash with spaces or invalid data. ([#2597](https://github.com/EQEmu/Server/pull/2597)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-01
* Fix IP Exemptions. ([#2189](https://github.com/EQEmu/Server/pull/2189)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-28
* Fix Instance Repository ([#2598](https://github.com/EQEmu/Server/pull/2598)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-01
* Fix Legacy Combat Lua Script ([#2226](https://github.com/EQEmu/Server/pull/2226)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-31
* Fix MovePC in #zone and #zoneinstance Commands. ([#2236](https://github.com/EQEmu/Server/pull/2236)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-01
* Fix NPC Reference in EVENT_SPAWN ([#2712](https://github.com/EQEmu/Server/pull/2712)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-08
* Fix ST_TargetsTarget Spells with Restrictions ([#2746](https://github.com/EQEmu/Server/pull/2746)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-15
* Fix Silent Saylinks Sending Message to Others. ([#2389](https://github.com/EQEmu/Server/pull/2389)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-22
* Fix Spell Bucket and Spell Global Logic Checks. ([#2285](https://github.com/EQEmu/Server/pull/2285)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-05
* Fix Spellinfo Command to work with SpellIDs above int16 ([#2437](https://github.com/EQEmu/Server/pull/2437)) ([Aeadoin](https://github.com/Aeadoin)) 2022-09-20
* Fix Strings::Money Missing Conditions. ([#2383](https://github.com/EQEmu/Server/pull/2383)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-21
* Fix Swarm Pet Flurry/Rampages Messages ([#2444](https://github.com/EQEmu/Server/pull/2444)) ([Aeadoin](https://github.com/Aeadoin)) 2022-09-25
* Fix bot compile locking client on server enter. ([#2210](https://github.com/EQEmu/Server/pull/2210)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-26
* Fix bot guild removal. ([#2194](https://github.com/EQEmu/Server/pull/2194)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-23
* Fix botgrouplist to display unique entries. ([#2785](https://github.com/EQEmu/Server/pull/2785)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-23
* Fix bots equipping augments. ([#2772](https://github.com/EQEmu/Server/pull/2772)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-22
* Fix case-sensitivity in #suspend Command. ([#2613](https://github.com/EQEmu/Server/pull/2613)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-05
* Fix duplicate and missing messages due to innate in spells ([#2170](https://github.com/EQEmu/Server/pull/2170)) ([noudess](https://github.com/noudess)) 2022-05-20
* Fix empty spawned merchants ([#2275](https://github.com/EQEmu/Server/pull/2275)) ([hgtw](https://github.com/hgtw)) 2022-06-28
* Fix for Bot command casting ([#1990](https://github.com/EQEmu/Server/pull/1990)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-12
* Fix for PR1954 target restriction with npcpc_only_flag from groupbuffs ([#1986](https://github.com/EQEmu/Server/pull/1986)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-10
* Fix for being able to skill up on corspe. ([#2058](https://github.com/EQEmu/Server/pull/2058)) ([noudess](https://github.com/noudess)) 2022-03-19
* Fix for castspell command ([#2010](https://github.com/EQEmu/Server/pull/2010)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-18
* Fix issue where #advnpcspawn addspawn does not add spawn sometimes. ([#2247](https://github.com/EQEmu/Server/pull/2247)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-07
* Fix issue where you can set your title to titles you don't have. ([#1917](https://github.com/EQEmu/Server/pull/1917)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-01-30
* Fix issue with Bot::LoadAndSpawnAllZonedBots. ([#2733](https://github.com/EQEmu/Server/pull/2733)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-15
* Fix issue with mobs summoning PCs into ceilings ([#1921](https://github.com/EQEmu/Server/pull/1921)) ([noudess](https://github.com/noudess)) 2022-01-30
* Fix loading world shared task state ([#2398](https://github.com/EQEmu/Server/pull/2398)) ([hgtw](https://github.com/hgtw)) 2022-08-28
* Fix luamod GetExperienceForKill return value  ([Cole-SoD](https://github.com/Cole-SoD)) 2023-01-12
* Fix memory leak in ucs ([#2409](https://github.com/EQEmu/Server/pull/2409)) ([hgtw](https://github.com/hgtw)) 2022-09-03
* Fix miscellaneous memory leaks related to EQApplicationPacket and it's pBuffer ([#2262](https://github.com/EQEmu/Server/pull/2262)) ([Quintinon](https://github.com/Quintinon)) 2022-07-03
* Fix null pointer crash on zones that have not booted a zone yet with #reload commands or anything that calls GetZoneDescription ([#2231](https://github.com/EQEmu/Server/pull/2231)) ([Akkadius](https://github.com/Akkadius)) 2022-06-01
* Fix possible crash in ProcessSpecialAbilities. ([#2630](https://github.com/EQEmu/Server/pull/2630)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-11
* Fix possible crash with zone name methods. ([#2055](https://github.com/EQEmu/Server/pull/2055)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-13
* Fix possible issue where variables have the same name. ([#2156](https://github.com/EQEmu/Server/pull/2156)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-08
* Fix quest::updatespawntimer() Perl croak. ([#1947](https://github.com/EQEmu/Server/pull/1947)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-01-26
* Fix recipient sound (vtell) on non-player races ([#2066](https://github.com/EQEmu/Server/pull/2066)) ([noudess](https://github.com/noudess)) 2022-04-02
* Fix scenario where dereferenced object could be null. ([#2784](https://github.com/EQEmu/Server/pull/2784)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-23
* Fix stack leaks in Lua events #2254  ([hgtw](https://github.com/hgtw)) 2022-06-09
* Fix trading with bots when in an illusion. ([#2645](https://github.com/EQEmu/Server/pull/2645)) ([nytmyr](https://github.com/nytmyr)) 2022-12-15
* Fix two invalid data accesses in zone/client.cpp ([#2238](https://github.com/EQEmu/Server/pull/2238)) ([Quintinon](https://github.com/Quintinon)) 2022-06-07
* Fixed Spell Logic for Bot Nukes ([#2481](https://github.com/EQEmu/Server/pull/2481)) ([Aeadoin](https://github.com/Aeadoin)) 2022-10-13
* Fixed message on promote/demote permissions check. ([#2700](https://github.com/EQEmu/Server/pull/2700)) ([Valorith](https://github.com/Valorith)) 2023-01-02
* Fixed several instances of incorrect comparision - & executes after == ([#2025](https://github.com/EQEmu/Server/pull/2025)) ([noudess](https://github.com/noudess)) 2022-03-07
* Force NPCs to respect special ability 24 and 50 when set on player pets ([#2059](https://github.com/EQEmu/Server/pull/2059)) ([Natedog2012](https://github.com/Natedog2012)) 2022-03-16
* Free return value of ZoneDatabase::LoadTraderItemWithCharges() ([#2264](https://github.com/EQEmu/Server/pull/2264)) ([Quintinon](https://github.com/Quintinon)) 2022-06-18
* Hacker_Str was causing sql errors - Non Escaped ([#2251](https://github.com/EQEmu/Server/pull/2251)) ([fryguy503](https://github.com/fryguy503)) 2022-06-08
* Handle memory leaks from return value of Client::GetTraderItems() ([#2266](https://github.com/EQEmu/Server/pull/2266)) ([Quintinon](https://github.com/Quintinon)) 2022-07-03
* Handle_OP_AugmentItem could cause Zone crash ([#2750](https://github.com/EQEmu/Server/pull/2750)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-17
* HasPet() Zone Crashes ([#2744](https://github.com/EQEmu/Server/pull/2744)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-15
* Illusions will now properly display armor to other clients when they zone in. ([#1958](https://github.com/EQEmu/Server/pull/1958)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-04
* Instrument Mods should not affect spells that change model size. ([#2072](https://github.com/EQEmu/Server/pull/2072)) ([KayenEQ](https://github.com/KayenEQ)) 2022-04-13
* Invisible will display as dropped now on air pets when they attack. ([#2042](https://github.com/EQEmu/Server/pull/2042)) ([KayenEQ](https://github.com/KayenEQ)) 2022-03-07
* IsDamage test for lifetap was not complete. ([#2213](https://github.com/EQEmu/Server/pull/2213)) ([noudess](https://github.com/noudess)) 2022-05-27
* Limit merchant temp item list to zone and instance ([#2346](https://github.com/EQEmu/Server/pull/2346)) ([mackal](https://github.com/mackal)) 2022-07-31
* Lua GetBlockNextSpell() no return. ([#2151](https://github.com/EQEmu/Server/pull/2151)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Make Perl TakeMoneyFromPP int64 ([#2158](https://github.com/EQEmu/Server/pull/2158)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-08
* Missing break ([#2031](https://github.com/EQEmu/Server/pull/2031)) ([KayenEQ](https://github.com/KayenEQ)) 2022-03-04
* Move EVENT_SPAWN for adding NPCs back to original spot, also add NPCs… ([#2749](https://github.com/EQEmu/Server/pull/2749)) ([Natedog2012](https://github.com/Natedog2012)) 2023-01-17
* NPC Constructor was passing hp_regen_per_second out of order to Mob(). ([#2681](https://github.com/EQEmu/Server/pull/2681)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-29
* NPC::CountItem and Corpse::CountItem 0 Charge Item Fix. ([#1959](https://github.com/EQEmu/Server/pull/1959)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-04
* NPC::GetNPCStat has no default return. ([#2150](https://github.com/EQEmu/Server/pull/2150)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* NPCs were getting weapon proc added twice ([#2277](https://github.com/EQEmu/Server/pull/2277)) ([noudess](https://github.com/noudess)) 2022-07-07
* Objects::GetTiltX() and Objects::GetTiltY() Perl Croak Typos. ([#2028](https://github.com/EQEmu/Server/pull/2028)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-04
* PR 1982 ([#1985](https://github.com/EQEmu/Server/pull/1985)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-10
* PR 2032 would lock client on casting fail as written ([#2038](https://github.com/EQEmu/Server/pull/2038)) ([KayenEQ](https://github.com/KayenEQ)) 2022-03-07
* Remove StringUtilTest::EscapeStringMemoryTest ([#2310](https://github.com/EQEmu/Server/pull/2310)) ([mackal](https://github.com/mackal)) 2022-07-15
* Remove Unnecessary Attack Log ([#2643](https://github.com/EQEmu/Server/pull/2643)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-14
* Remove unnecessary log messages. ([#2642](https://github.com/EQEmu/Server/pull/2642)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-14
* Removed Lua Event Argument Dispatch.  ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-01
* Resolve Warning due to Virtual Mob Method GetInv() ([#2650](https://github.com/EQEmu/Server/pull/2650)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-19
* Resolve XP Calculation Bug introduced w/ recent Rule addition ([#2703](https://github.com/EQEmu/Server/pull/2703)) ([Valorith](https://github.com/Valorith)) 2023-01-07
* Resolve logic error in Raid::QueueClients ([#2404](https://github.com/EQEmu/Server/pull/2404)) ([mackal](https://github.com/mackal)) 2022-09-01
* Resolve subroutine redefinition due to bot methods. ([#2117](https://github.com/EQEmu/Server/pull/2117)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Restore missing messages for lifetap and dmg spells. ([#2057](https://github.com/EQEmu/Server/pull/2057)) ([noudess](https://github.com/noudess)) 2022-04-14
* Shared Memory Faction Association Typo ([#2419](https://github.com/EQEmu/Server/pull/2419)) ([mackal](https://github.com/mackal)) 2022-09-03
* Spell Buckets/Globals SQL Escape. ([#2019](https://github.com/EQEmu/Server/pull/2019)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-26
* Spell Buckets/Globals did not allow string-based values. ([#2043](https://github.com/EQEmu/Server/pull/2043)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-09
* Stop skill ups on Charmed NPCs. ([#2249](https://github.com/EQEmu/Server/pull/2249)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-10
* Summon Companion causing pets to warps away. ([#1972](https://github.com/EQEmu/Server/pull/1972)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-08
* Touch Of Vinitras was ignoring pet DT rule ([#2469](https://github.com/EQEmu/Server/pull/2469)) ([Aeadoin](https://github.com/Aeadoin)) 2022-10-03
* Tradeskill Autocombine MinSkill ([#2260](https://github.com/EQEmu/Server/pull/2260)) ([fryguy503](https://github.com/fryguy503)) 2022-06-10
* Tradeskill Item 0 Error ([#2256](https://github.com/EQEmu/Server/pull/2256)) ([fryguy503](https://github.com/fryguy503)) 2022-06-10
* Zone Flags Regression ([#2760](https://github.com/EQEmu/Server/pull/2760)) ([Akkadius](https://github.com/Akkadius)) 2023-01-19
* checking casting_spell_slot before its defined is bad ([#2013](https://github.com/EQEmu/Server/pull/2013)) ([KayenEQ](https://github.com/KayenEQ)) 2022-02-20
* manifest for db version 9176 had incorrect field name ([#2062](https://github.com/EQEmu/Server/pull/2062)) ([noudess](https://github.com/noudess)) 2022-03-19
* quest::MovePCInstance() Arguments Fix. ([#2020](https://github.com/EQEmu/Server/pull/2020)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-27

### Hotfix

* Add Bazaar portal discs to SQL  ([Akkadius](https://github.com/Akkadius)) 2022-09-05
* Add discord_webhooks to server tables  ([Akkadius](https://github.com/Akkadius)) 2022-07-03
* Blocks are nested too deeply. ([#2689](https://github.com/EQEmu/Server/pull/2689)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-01
* Cleanup #questerrors Command. ([#2116](https://github.com/EQEmu/Server/pull/2116)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-07
* Compiling fails on FMT 9.1 with Bots ([#2665](https://github.com/EQEmu/Server/pull/2665)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-21
* Correct database call to point to the content_db connection  ([Akkadius](https://github.com/Akkadius)) 2022-06-12
* Corrected misnamed Database Query file for Experience Toggle ([#2683](https://github.com/EQEmu/Server/pull/2683)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-31
* Faction associations file naming / lock consistency  ([Akkadius](https://github.com/Akkadius)) 2022-09-05
* Fix DB version merge  ([Akkadius](https://github.com/Akkadius)) 2022-05-08
* Fix door click crash issue if destination zone doesn't exist  ([Akkadius](https://github.com/Akkadius)) 2023-01-20
* Fix issue with Bot Loading with 0 Health causing buffs to be lost. ([#2552](https://github.com/EQEmu/Server/pull/2552)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-18
* Fix lua mod load path  ([Akkadius](https://github.com/Akkadius)) 2022-09-29
* Fix merge issue  ([Akkadius](https://github.com/Akkadius)) 2022-07-14
* Fix path load ordering for CLI commands  ([Akkadius](https://github.com/Akkadius)) 2022-10-16
* Fix potential race for crash dumps (Linux)  ([Akkadius](https://github.com/Akkadius)) 2022-07-31
* Fix regression caused by #2129  ([Akkadius](https://github.com/Akkadius)) 2022-05-09
* Flipped positive / negative values for legacy_combat.lua  ([Akkadius](https://github.com/Akkadius)) 2022-06-09
* Force collation on conversion script  ([Akkadius](https://github.com/Akkadius)) 2022-09-28
* Instances Repository Fix ([#2576](https://github.com/EQEmu/Server/pull/2576)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-26
* Login Server failing to compile on Windows. ([#2758](https://github.com/EQEmu/Server/pull/2758)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-19
* Lua Parser Needs Lua_ItemInst ([#2696](https://github.com/EQEmu/Server/pull/2696)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-01
* Make sure we have a proper split size before assuming we can split it  ([Akkadius](https://github.com/Akkadius)) 2023-01-20
* Move discord_webhooks to state tables because we don't want webhooks being exported  ([Akkadius](https://github.com/Akkadius)) 2022-07-03
* Possible windows compile fix  ([Akkadius](https://github.com/Akkadius)) 2022-07-07
* Possible windows compile fix take 2  ([Akkadius](https://github.com/Akkadius)) 2022-07-07
* Remove appveyor fetch bots  ([Akkadius](https://github.com/Akkadius)) 2023-01-21
* Remove expansion field from account for those who have it ([#2357](https://github.com/EQEmu/Server/pull/2357)) ([Akkadius](https://github.com/Akkadius)) 2022-08-01
* Resolve Zone Crashing when grouped with Bots. ([#2747](https://github.com/EQEmu/Server/pull/2747)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-16
* Resolve issue with Bot Casting after zoning. ([#2617](https://github.com/EQEmu/Server/pull/2617)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-04
* Return weather_type_map  ([Akkadius](https://github.com/Akkadius)) 2022-10-14
* SQL Update  ([Akkadius](https://github.com/Akkadius)) 2022-07-31
* Shared Memory Protection Fixes  ([Akkadius](https://github.com/Akkadius)) 2022-07-27
* Windows compile fix take 3 (final)  ([Akkadius](https://github.com/Akkadius)) 2022-07-07
* fix manifest  ([Akkadius](https://github.com/Akkadius)) 2022-07-16

### Logging

* Add stack trace in code paths that shouldn't occur ([#2453](https://github.com/EQEmu/Server/pull/2453)) ([Akkadius](https://github.com/Akkadius)) 2022-09-28
* Cleanup AI Logging Events ([#2615](https://github.com/EQEmu/Server/pull/2615)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-04
* Fix log messages to final damage values ([#2056](https://github.com/EQEmu/Server/pull/2056)) ([noudess](https://github.com/noudess)) 2022-03-14
* Fix zoning log typo ([#2478](https://github.com/EQEmu/Server/pull/2478)) ([Akkadius](https://github.com/Akkadius)) 2022-10-11
* Force crash logs to always be on regardless of setting ([#2762](https://github.com/EQEmu/Server/pull/2762)) ([Akkadius](https://github.com/Akkadius)) 2023-01-20
* Improvements to GM Say Logging ([#2765](https://github.com/EQEmu/Server/pull/2765)) ([Akkadius](https://github.com/Akkadius)) 2023-01-20
* Logging Improvements ([#2755](https://github.com/EQEmu/Server/pull/2755)) ([Akkadius](https://github.com/Akkadius)) 2023-01-18
* More AI Logging Cleanup ([#2616](https://github.com/EQEmu/Server/pull/2616)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-10
* Netcode Logging Unify ([#2443](https://github.com/EQEmu/Server/pull/2443)) ([Akkadius](https://github.com/Akkadius)) 2022-09-28
* Remove function prefixes ([#2766](https://github.com/EQEmu/Server/pull/2766)) ([Akkadius](https://github.com/Akkadius)) 2023-01-20
* Remove loginserver unhandled error ([#2458](https://github.com/EQEmu/Server/pull/2458)) ([Akkadius](https://github.com/Akkadius)) 2022-09-29
* Reset stream so we don't bold the whole line  ([Akkadius](https://github.com/Akkadius)) 2023-01-18
* Table Injection - Member Variable Cleanup ([#2281](https://github.com/EQEmu/Server/pull/2281)) ([Akkadius](https://github.com/Akkadius)) 2022-07-07
* Update BUILD_LOGGING=false Blank Aliases ([#2083](https://github.com/EQEmu/Server/pull/2083)) ([Akkadius](https://github.com/Akkadius)) 2022-05-01

### Luamod

* Add CalcSpellEffectValue_formula to luamods ([#2721](https://github.com/EQEmu/Server/pull/2721)) ([Natedog2012](https://github.com/Natedog2012)) 2023-01-11

### Mercs

* Add Mercenary Support ([#2745](https://github.com/EQEmu/Server/pull/2745)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-17

### Optimization

* Handle channel name filter checks in memory ([#2767](https://github.com/EQEmu/Server/pull/2767)) ([Valorith](https://github.com/Valorith)) 2023-01-20

### QS

* Database class name change ([#2743](https://github.com/EQEmu/Server/pull/2743)) ([Akkadius](https://github.com/Akkadius)) 2023-01-15

### Quest API

* Add AddAISpellEffect(spell_effect_id, base_value, limit_value, max_value) and RemoveAISpellEffect(spell_effect_id) to Lua. ([#1981](https://github.com/EQEmu/Server/pull/1981)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-09
* Add AddItem() to Perl/Lua. ([#2054](https://github.com/EQEmu/Server/pull/2054)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-13
* Add AddPlatinum(), GetCarriedPlatinum() and TakePlatinum() to Perl/Lua. ([#2079](https://github.com/EQEmu/Server/pull/2079)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-04-30
* Add Area Damage Methods to Perl/Lua. ([#2549](https://github.com/EQEmu/Server/pull/2549)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-17
* Add Augment Slot Type/Visible to GetItemStat ([#2686](https://github.com/EQEmu/Server/pull/2686)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-01
* Add Bot Methods to Lua. ([#2731](https://github.com/EQEmu/Server/pull/2731)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-14
* Add Bot::Camp() to Perl/Lua. ([#2718](https://github.com/EQEmu/Server/pull/2718)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-11
* Add BuffCount() Overloads to Perl/Lua. ([#2679](https://github.com/EQEmu/Server/pull/2679)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-29
* Add CampAllBots() to Perl/Lua. ([#2732](https://github.com/EQEmu/Server/pull/2732)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-14
* Add Charges/Augment/Attuned Support to Varlink. ([#2685](https://github.com/EQEmu/Server/pull/2685)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-01
* Add CheckNameFilter to Perl/Lua. ([#2175](https://github.com/EQEmu/Server/pull/2175)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-20
* Add Client Augment Events to Perl/Lua. ([#2735](https://github.com/EQEmu/Server/pull/2735)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-15
* Add Client Spell Methods to Perl/Lua. ([#2550](https://github.com/EQEmu/Server/pull/2550)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Add CloneAppearance() to Perl/Lua. ([#2531](https://github.com/EQEmu/Server/pull/2531)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add CopyHateList() to Perl/Lua. ([#2623](https://github.com/EQEmu/Server/pull/2623)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-06
* Add Corpse::AddItem overloads for Lua ([#2509](https://github.com/EQEmu/Server/pull/2509)) ([hgtw](https://github.com/hgtw)) 2022-10-29
* Add Despawn Events to Perl/Lua. ([#2707](https://github.com/EQEmu/Server/pull/2707)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-07
* Add DoAnim Overloads to Perl/Lua. ([#2627](https://github.com/EQEmu/Server/pull/2627)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-10
* Add DoAugmentSlotsMatch() to Perl/Lua. ([#2687](https://github.com/EQEmu/Server/pull/2687)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-01
* Add DoesAugmentFit() to Perl/Lua. ([#2688](https://github.com/EQEmu/Server/pull/2688)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-01
* Add Door Methods to Perl/Lua. ([#2724](https://github.com/EQEmu/Server/pull/2724)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-12
* Add EVENT_AA_BUY and EVENT_AA_GAIN to Perl/Lua. ([#2504](https://github.com/EQEmu/Server/pull/2504)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-05
* Add EVENT_BOT_CREATE to Perl/Lua ([#2713](https://github.com/EQEmu/Server/pull/2713)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-09
* Add EVENT_CAST_ON exports to EVENT_CAST and EVENT_CAST_BEGIN. ([#2051](https://github.com/EQEmu/Server/pull/2051)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-12
* Add EVENT_EQUIP_ITEM_CLIENT and EVENT_UNEQUIP_ITEM_CLIENT to Perl/Lua. ([#2015](https://github.com/EQEmu/Server/pull/2015)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-23
* Add EVENT_GM_COMMAND to Perl/Lua. ([#2634](https://github.com/EQEmu/Server/pull/2634)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-11
* Add EVENT_LEVEL_DOWN to Perl/Lua. ([#2620](https://github.com/EQEmu/Server/pull/2620)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-11
* Add EVENT_PAYLOAD to Perl/Lua. ([#2611](https://github.com/EQEmu/Server/pull/2611)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-04
* Add EVENT_SKILL_UP & EVENT_LANGUAGE_SKILL_UP to Perl/Lua ([#2076](https://github.com/EQEmu/Server/pull/2076)) ([nytmyr](https://github.com/nytmyr)) 2022-04-25
* Add Entity Variable Methods to Perl/Lua. ([#2609](https://github.com/EQEmu/Server/pull/2609)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-04
* Add Fling Overloads to Perl/Lua. ([#2622](https://github.com/EQEmu/Server/pull/2622)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-06
* Add GetAugmentIDsBySlotID() to Perl/Lua. ([#2673](https://github.com/EQEmu/Server/pull/2673)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-25
* Add GetAverageLevel() to Perl/Lua. ([#2524](https://github.com/EQEmu/Server/pull/2524)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add GetBotItem() and GetBotItemIDBySlot() to Perl/Lua. ([#2350](https://github.com/EQEmu/Server/pull/2350)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-31
* Add GetBotListByCharacterID() to Perl/Lua. ([#2069](https://github.com/EQEmu/Server/pull/2069)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-04-02
* Add GetBotListByClientName() Class Overload to Perl/Lua. ([#2577](https://github.com/EQEmu/Server/pull/2577)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-26
* Add GetBotListByClientName(client_name) to Perl/Lua. ([#2064](https://github.com/EQEmu/Server/pull/2064)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-23
* Add GetEnvironmentalDamageName() to Perl/Lua. ([#1964](https://github.com/EQEmu/Server/pull/1964)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-10
* Add GetGMStatus() to Perl/Lua. ([#2448](https://github.com/EQEmu/Server/pull/2448)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-09-28
* Add GetGuildPublicNote() to Perl/Lua. ([#2608](https://github.com/EQEmu/Server/pull/2608)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-04
* Add GetHealAmount() and GetSpellDamage() to Perl/Lua. ([#2165](https://github.com/EQEmu/Server/pull/2165)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-11
* Add GetLeader() and GetLeaderName() to Perl/Lua. ([#2701](https://github.com/EQEmu/Server/pull/2701)) ([Valorith](https://github.com/Valorith)) 2023-01-04
* Add GetLowestLevel() to Perl. ([#2517](https://github.com/EQEmu/Server/pull/2517)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-05
* Add GetRandomBot() to Perl/Lua ([#2543](https://github.com/EQEmu/Server/pull/2543)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-16
* Add GetRandomClient(), GetRandomMob() and GetRandomNPC() overloads to Perl/Lua. ([#2541](https://github.com/EQEmu/Server/pull/2541)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add GetRandomMob() and GetRandomNPC() to Perl/Lua. ([#2006](https://github.com/EQEmu/Server/pull/2006)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-17
* Add GetSkillDmgAmt() to Perl. ([#2365](https://github.com/EQEmu/Server/pull/2365)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-10
* Add GetUltimateOwner() to Perl/Lua. ([#2516](https://github.com/EQEmu/Server/pull/2516)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-05
* Add Goto Player Teleport Methods. ([#2379](https://github.com/EQEmu/Server/pull/2379)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-20
* Add Group/Raid Overloads to Perl/Lua. ([#2587](https://github.com/EQEmu/Server/pull/2587)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-27
* Add Group/Raid overloads to Perl/Lua. ([#2526](https://github.com/EQEmu/Server/pull/2526)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add HasBotSpellEntry() to Perl/Lua. ([#2563](https://github.com/EQEmu/Server/pull/2563)) ([Aeadoin](https://github.com/Aeadoin)) 2022-11-25
* Add Hotzone Methods to Perl/Lua. ([#2558](https://github.com/EQEmu/Server/pull/2558)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Add Instance ID/Version exports to EVENT_ZONE. ([#2502](https://github.com/EQEmu/Server/pull/2502)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-05
* Add Instance Methods to Perl/Lua. ([#2573](https://github.com/EQEmu/Server/pull/2573)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-26
* Add IsAttackAllowed() to Perl/Lua. ([#2672](https://github.com/EQEmu/Server/pull/2672)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-25
* Add IsRaining() and IsSnowing() to Perl/Lua. ([#2477](https://github.com/EQEmu/Server/pull/2477)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-14
* Add IsRareSpawn() to Perl/Lua. ([#2338](https://github.com/EQEmu/Server/pull/2338)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-30
* Add Lua handlers for zone controller events ([#2514](https://github.com/EQEmu/Server/pull/2514)) ([hgtw](https://github.com/hgtw)) 2022-11-05
* Add Marquee methods to Perl/Lua. ([#2544](https://github.com/EQEmu/Server/pull/2544)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-16
* Add MaxSkills() to Perl/Lua. ([#2621](https://github.com/EQEmu/Server/pull/2621)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-06
* Add Merchant Events to Perl/Lua. ([#2452](https://github.com/EQEmu/Server/pull/2452)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-09-28
* Add Mob Hate Methods to Perl/Lua. ([#2548](https://github.com/EQEmu/Server/pull/2548)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-16
* Add Overloads to MoveZone Methods in Perl/Lua. ([#2551](https://github.com/EQEmu/Server/pull/2551)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-22
* Add Owner methods to Perl/Lua. ([#2542](https://github.com/EQEmu/Server/pull/2542)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add Popup methods to Perl/Lua. ([#2533](https://github.com/EQEmu/Server/pull/2533)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add Proximity Range Methods to Perl/Lua. ([#2572](https://github.com/EQEmu/Server/pull/2572)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-26
* Add RandomizeFeature() overloads to Perl/Lua. ([#2532](https://github.com/EQEmu/Server/pull/2532)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add Recipe Methods ([#2393](https://github.com/EQEmu/Server/pull/2393)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-23
* Add ResetAlternateAdvancementRank() to Perl/Lua. ([#2510](https://github.com/EQEmu/Server/pull/2510)) ([hgtw](https://github.com/hgtw)) 2022-10-29
* Add ResetDecayTimer() to Perl/Lua. ([#2520](https://github.com/EQEmu/Server/pull/2520)) ([hgtw](https://github.com/hgtw)) 2022-11-06
* Add SendGMCommand() to Perl/Lua. ([#2527](https://github.com/EQEmu/Server/pull/2527)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add SendPath() to Perl/Lua. ([#2740](https://github.com/EQEmu/Server/pull/2740)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-15
* Add SignalAllBotsByOwnerName() to Perl/Lua. ([#2730](https://github.com/EQEmu/Server/pull/2730)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-13
* Add SplitMoney() with Client splitter to Perl. ([#2525](https://github.com/EQEmu/Server/pull/2525)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-14
* Add TaskSelector to Perl/Lua. ([#2177](https://github.com/EQEmu/Server/pull/2177)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-15
* Add Time String to Seconds Method to Perl/Lua. ([#2580](https://github.com/EQEmu/Server/pull/2580)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-27
* Add TrackNPC to Perl/Lua. ([#2272](https://github.com/EQEmu/Server/pull/2272)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-29
* Add WearChange Overloads to Perl/Lua. ([#2600](https://github.com/EQEmu/Server/pull/2600)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-01
* Add Zone Flag Methods to Perl/Lua. ([#2574](https://github.com/EQEmu/Server/pull/2574)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-26
* Add apis to end shared tasks ([#2521](https://github.com/EQEmu/Server/pull/2521)) ([hgtw](https://github.com/hgtw)) 2022-11-06
* Add caster_id and caster_level export to EVENT_CAST_ON in Perl/Lua. ([#2049](https://github.com/EQEmu/Server/pull/2049)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-11
* Add commify to Perl/Lua. ([#2099](https://github.com/EQEmu/Server/pull/2099)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-03
* Add inventory->CountItemEquippedByID(item_id) and inventory->HasItemEquippedByID(item_id) to Perl/Lua. ([#1963](https://github.com/EQEmu/Server/pull/1963)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-02-06
* Add missing methods/package.adds to Perl API. ([#2287](https://github.com/EQEmu/Server/pull/2287)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-05
* Add multiple inventory method short hands to client. ([#2078](https://github.com/EQEmu/Server/pull/2078)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-04-30
* Add option to Ignore Mods to CalcEXP ([#2704](https://github.com/EQEmu/Server/pull/2704)) ([Aeadoin](https://github.com/Aeadoin)) 2023-01-06
* Adjustment to depop_all function. ([#2595](https://github.com/EQEmu/Server/pull/2595)) ([fryguy503](https://github.com/fryguy503)) 2022-11-30
* Allow CreateInstance to be used without a Client initiator. ([#2399](https://github.com/EQEmu/Server/pull/2399)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-28
* Allow EVENT_ZONE to be parsed as non-zero to prevent zoning. ([#2052](https://github.com/EQEmu/Server/pull/2052)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-12
* Allow scripts to prevent door click ([#2327](https://github.com/EQEmu/Server/pull/2327)) ([hgtw](https://github.com/hgtw)) 2022-07-27
* Cleanup Proximity Events ([#2697](https://github.com/EQEmu/Server/pull/2697)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-02
* Cleanup Signal Methods in Perl/Lua. ([#2604](https://github.com/EQEmu/Server/pull/2604)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-04
* Expand Bot quest API functionality. ([#2096](https://github.com/EQEmu/Server/pull/2096)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-04
* Expand SaveGuardSpot ([#2258](https://github.com/EQEmu/Server/pull/2258)) ([fryguy503](https://github.com/fryguy503)) 2022-06-10
* Export corpse in EVENT_DEATH_COMPLETE ([#2519](https://github.com/EQEmu/Server/pull/2519)) ([hgtw](https://github.com/hgtw)) 2022-11-06
* Export killed XYZH to EVENT_DEATH_ZONE in Perl. ([#2050](https://github.com/EQEmu/Server/pull/2050)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-03-12
* Fix Lua Door/Object Create Methods. ([#2633](https://github.com/EQEmu/Server/pull/2633)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-12-11
* Fix Perl EVENT_HP double parsing in Spire. ([#2585](https://github.com/EQEmu/Server/pull/2585)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-11-27
* Fix lua task selector count when over max ([#2353](https://github.com/EQEmu/Server/pull/2353)) ([hgtw](https://github.com/hgtw)) 2022-07-31
* Fix missing arg in perl set_proximity ([#2291](https://github.com/EQEmu/Server/pull/2291)) ([hgtw](https://github.com/hgtw)) 2022-07-09
* Fix parameters in some Perl worldwide methods. ([#2224](https://github.com/EQEmu/Server/pull/2224)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-31
* Let HasQuestSub check encounters ([#2435](https://github.com/EQEmu/Server/pull/2435)) ([hgtw](https://github.com/hgtw)) 2022-09-20
* Perl Doors Fix. ([#2288](https://github.com/EQEmu/Server/pull/2288)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-05
* Perl Money Fixes. ([#2098](https://github.com/EQEmu/Server/pull/2098)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-04
* Send delivered task items in trade events ([#2518](https://github.com/EQEmu/Server/pull/2518)) ([hgtw](https://github.com/hgtw)) 2022-11-06
* Use Floating Point for CameraEffect Intensity ([#2337](https://github.com/EQEmu/Server/pull/2337)) ([hgtw](https://github.com/hgtw)) 2022-07-31
* Use binding library for perl apis ([#2216](https://github.com/EQEmu/Server/pull/2216)) ([hgtw](https://github.com/hgtw)) 2022-07-04

### Rules

* Add Backstab Rules ([#2666](https://github.com/EQEmu/Server/pull/2666)) ([Valorith](https://github.com/Valorith)) 2022-12-21
* Add Frontal Stun Immunity Rules. ([#2217](https://github.com/EQEmu/Server/pull/2217)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-07
* Add Keep Level on Death ([#2319](https://github.com/EQEmu/Server/pull/2319)) ([trentdm](https://github.com/trentdm)) 2022-07-30
* Add LDoN Loot Count Modifier Rule ([#2694](https://github.com/EQEmu/Server/pull/2694)) ([Kinglykrab](https://github.com/Kinglykrab)) 2023-01-03
* Add ManaOnDeath and EndurOnDeath ([#2661](https://github.com/EQEmu/Server/pull/2661)) ([fryguy503](https://github.com/fryguy503)) 2022-12-20
* Add Rule to Disable NPC Last Names. ([#2227](https://github.com/EQEmu/Server/pull/2227)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-04
* Add Rule to Enable Tells with #hideme ([#2358](https://github.com/EQEmu/Server/pull/2358)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-08-04
* Add Rule to allow Assassinate on non-Humanoid body types. ([#2331](https://github.com/EQEmu/Server/pull/2331)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-29
* Add Rule to allow Headshots on non-Humanoid body types. ([#2329](https://github.com/EQEmu/Server/pull/2329)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-07-29
* Add Rules to disable various item functionalities and cleanup data types. ([#2225](https://github.com/EQEmu/Server/pull/2225)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-06-01
* Add Spells:BuffsFadeOnDeath. ([#2200](https://github.com/EQEmu/Server/pull/2200)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Add Spells:IllusionsAlwaysPersist. ([#2199](https://github.com/EQEmu/Server/pull/2199)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-27
* Add Toggle for Warrior Shielding ([#2496](https://github.com/EQEmu/Server/pull/2496)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-10-22
* Add adjustment for zone forage. ([#2330](https://github.com/EQEmu/Server/pull/2330)) ([fryguy503](https://github.com/fryguy503)) 2022-07-30
* Add rule for NPC Level Based Buff Restrictions. ([#2708](https://github.com/EQEmu/Server/pull/2708)) ([noudess](https://github.com/noudess)) 2023-01-15
* Add rule to allow players to permanently save chat channels to database, up to a limit. ([#2706](https://github.com/EQEmu/Server/pull/2706)) ([Valorith](https://github.com/Valorith)) 2023-01-19
* Change TradeskillUp Rules to be Floats ([#2674](https://github.com/EQEmu/Server/pull/2674)) ([Aeadoin](https://github.com/Aeadoin)) 2022-12-25
* Cleanup all unused rules. ([#2184](https://github.com/EQEmu/Server/pull/2184)) ([Kinglykrab](https://github.com/Kinglykrab)) 2022-05-23
* Rule Gate Pet Zoning ([#2625](https://github.com/EQEmu/Server/pull/2625)) ([fryguy503](https://github.com/fryguy503)) 2022-12-07
* Rule to allow cap on % XP gain per kill ([#2667](https://github.com/EQEmu/Server/pull/2667)) ([Valorith](https://github.com/Valorith)) 2022-12-25
* Update logic checks everywhere for FVNoDropFlag. ([#2179](https://github.com/EQEmu/Server/pull/2179)) ([Quintinon](https://github.com/Quintinon)) 2022-07-30

### SQL

* Bugs Table Migration  (#2602) ([#2559](https://github.com/EQEmu/Server/pull/2559)) ([joligario](https://github.com/joligario)) 2022-12-01
* Update 2023_01_15_merc_data.sql ([#2763](https://github.com/EQEmu/Server/pull/2763)) ([joligario](https://github.com/joligario)) 2023-01-20

### UCS

* Auto Client Reconnection ([#2154](https://github.com/EQEmu/Server/pull/2154)) ([Akkadius](https://github.com/Akkadius)) 2022-05-08

### Websocket

* Fix cpp20/gcc11 compile failure ([#2737](https://github.com/EQEmu/Server/pull/2737)) ([Akkadius](https://github.com/Akkadius)) 2023-01-15

### Zone Flags

* Use database connection, not content connection ([#2759](https://github.com/EQEmu/Server/pull/2759)) ([Akkadius](https://github.com/Akkadius)) 2023-01-19
