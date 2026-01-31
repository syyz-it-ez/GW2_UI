# Triaged Issues Report

Issues are sorted from **most to least impactful** for performance.

## Summary by Category

| Priority | Category | Count | Impact |
|:--------:|----------|------:|--------|
| 10 | `string_concat_in_loop` | 26 | 🔥 Critical (GC churn) |
| 8 | `debug_statement` | 16 | ⚠️ High (wasted cycles) |
| 5 | `global_write` | 141 | ⚡ Medium (lookup + bugs) |
| 3 | `unused_local_function` | 6 | 📝 Low (dead code) |
| 2 | `unused_local_variable` | 67 | 📝 Low (dead code) |
| 1 | `unnecessary_else` | 98 | 💅 Style only |

---

## All Issues (Ordered by Impact)

### Priority 10: `string_concat_in_loop`

**[1]** 🟡 `Classic\Immersive\Skins\colorPicker.lua` L13
- String concat in loop: str = str .. x
- Variable: `str`
- Suggestion: Use table.insert() + table.concat()
- Loop: L12-L14
- [ ] Status: Pending

**[2]** 🟡 `Libs\Core\UTF8\utf8.lua` L234
- String concat in loop: newstr = newstr .. x
- Variable: `newstr`
- Suggestion: Use table.insert() + table.concat()
- Loop: L230-L237
- [ ] Status: Pending

**[3]** 🟡 `Libs\Core\UTF8\utf8.lua` L284
- String concat in loop: newstr = newstr .. x
- Variable: `newstr`
- Suggestion: Use table.insert() + table.concat()
- Loop: L275-L287
- [ ] Status: Pending

**[4]** 🟡 `Libs\Core\oUF\ouf.lua` L270
- String concat in loop: objectUnit = objectUnit .. x
- Variable: `objectUnit`
- Suggestion: Use table.insert() + table.concat()
- Loop: L262-L356
- [ ] Status: Pending

**[5]** 🟡 `Libs\Core\oUF\ouf.lua` L478
- String concat in loop: cond = cond .. x
- Variable: `cond`
- Suggestion: Use table.insert() + table.concat()
- Loop: L473-L480
- [ ] Status: Pending

**[6]** 🟡 `Mainline\Immersive\Skins\colorPicker.lua` L15
- String concat in loop: str = str .. x
- Variable: `str`
- Suggestion: Use table.insert() + table.concat()
- Loop: L14-L16
- [ ] Status: Pending

**[7]** 🟡 `Mainline\Immersive\eventTracker.lua` L1338
- String concat in loop: netsText = netsText .. x
- Variable: `netsText`
- Suggestion: Use table.insert() + table.concat()
- Loop: L1337-L1342
- [ ] Status: Pending

**[8]** 🟡 `Mainline\Immersive\eventTracker.lua` L1374
- String concat in loop: netsText = netsText .. x
- Variable: `netsText`
- Suggestion: Use table.insert() + table.concat()
- Loop: L1373-L1378
- [ ] Status: Pending

**[9]** 🟡 `Mainline\Objectives\bonusObjective.lua` L210
- String concat in loop: simpleDesc = simpleDesc .. x
- Variable: `simpleDesc`
- Suggestion: Use table.insert() + table.concat()
- Loop: L203-L219
- [ ] Status: Pending

**[10]** 🟡 `Mists\Immersive\Skins\colorPicker.lua` L13
- String concat in loop: str = str .. x
- Variable: `str`
- Suggestion: Use table.insert() + table.concat()
- Loop: L12-L14
- [ ] Status: Pending

**[11]** 🟡 `TBC\Immersive\Skins\colorPicker.lua` L13
- String concat in loop: str = str .. x
- Variable: `str`
- Suggestion: Use table.insert() + table.concat()
- Loop: L12-L14
- [ ] Status: Pending

**[12]** 🟡 `core\API\utils.lua` L621
- String concat in loop: msg = msg .. x
- Variable: `msg`
- Suggestion: Use table.insert() + table.concat()
- Loop: L619-L622
- [ ] Status: Pending

**[13]** 🟡 `core\API\utils.lua` L991
- String concat in loop: msg = msg .. x
- Variable: `msg`
- Suggestion: Use table.insert() + table.concat()
- Loop: L988-L1004
- [ ] Status: Pending

**[14]** 🟡 `core\API\utils.lua` L1119
- String concat in loop: s = s .. x
- Variable: `s`
- Suggestion: Use table.insert() + table.concat()
- Loop: L1117-L1121
- [ ] Status: Pending

**[15]** 🟡 `core\DataInfo\guild.lua` L249
- String concat in loop: name = name .. x
- Variable: `name`
- Suggestion: Use table.insert() + table.concat()
- Loop: L242-L260
- [ ] Status: Pending

**[16]** 🟡 `core\DataInfo\money.lua` L128
- String concat in loop: label = label .. x
- Variable: `label`
- Suggestion: Use table.insert() + table.concat()
- Loop: L123-L131
- [ ] Status: Pending

**[17]** 🟡 `core\Immersive\chatframe.lua` L317
- String concat in loop: text = text .. x
- Variable: `text`
- Suggestion: Use table.insert() + table.concat()
- Loop: L316-L318
- [ ] Status: Pending

**[18]** 🟡 `core\Immersive\chatframe.lua` L836
- String concat in loop: rebuiltString = rebuiltString .. x
- Variable: `rebuiltString`
- Suggestion: Use table.insert() + table.concat()
- Loop: L799-L838
- [ ] Status: Pending

**[19]** 🟡 `core\Immersive\chatframe.lua` L873
- String concat in loop: outstr = outstr .. x
- Variable: `outstr`
- Suggestion: Use table.insert() + table.concat()
- Loop: L870-L883
- [ ] Status: Pending

**[20]** 🟡 `core\Immersive\chatframe.lua` L1266
- String concat in loop: groupList = groupList .. x
- Variable: `groupList`
- Suggestion: Use table.insert() + table.concat()
- Loop: L1259-L1268
- [ ] Status: Pending

**[21]** 🟡 `core\Immersive\chatframe.lua` L1270
- String concat in loop: groupList = groupList .. x
- Variable: `groupList`
- Suggestion: Use table.insert() + table.concat()
- Loop: L1250-L1275
- [ ] Status: Pending

**[22]** 🟡 `core\Objectives\notifications.lua` L113
- String concat in loop: finalText = finalText .. x
- Variable: `finalText`
- Suggestion: Use table.insert() + table.concat()
- Loop: L104-L116
- [ ] Status: Pending

**[23]** 🟡 `core\debug.lua` L33
- String concat in loop: msg = msg .. x
- Variable: `msg`
- Suggestion: Use table.insert() + table.concat()
- Loop: L31-L34
- [ ] Status: Pending

**[24]** 🟡 `settings\panels\panel_auras.lua` L82
- String concat in loop: name = name .. x
- Variable: `name`
- Suggestion: Use table.insert() + table.concat()
- Loop: L73-L88
- [ ] Status: Pending

**[25]** 🟡 `settings\panels\panel_auras.lua` L101
- String concat in loop: name = name .. x
- Variable: `name`
- Suggestion: Use table.insert() + table.concat()
- Loop: L92-L107
- [ ] Status: Pending

**[26]** 🟡 `settings\settingsWindowProfilesTab.lua` L386
- String concat in loop: name = name .. x
- Variable: `name`
- Suggestion: Use table.insert() + table.concat()
- Loop: L383-L394
- [ ] Status: Pending

### Priority 8: `debug_statement`

**[27]** 🐛 `Libs\Core\LibDeflate\LibDeflate.lua` L3391
- Debug call: print()
- [ ] Status: Pending

**[28]** 🐛 `Libs\Core\LibDeflate\LibDeflate.lua` L3406
- Debug call: print()
- [ ] Status: Pending

**[29]** 🐛 `Libs\Core\LibRealmInfo\LibRealmInfo.lua` L23
- Debug call: print()
- [ ] Status: Pending

**[30]** 🐛 `Libs\Core\oUF\private.lua` L19
- Debug call: print()
- [ ] Status: Pending

**[31]** 🐛 `Mainline\Actionbar\Actionbars.lua` L73
- Debug call: print()
- [ ] Status: Pending

**[32]** 🐛 `Mainline\Immersive\eventTracker.lua` L1800
- Debug call: print()
- [ ] Status: Pending

**[33]** 🐛 `Mainline\Immersive\eventTracker.lua` L1801
- Debug call: print()
- [ ] Status: Pending

**[34]** 🐛 `Mainline\Immersive\eventTracker.lua` L1802
- Debug call: print()
- [ ] Status: Pending

**[35]** 🐛 `Mainline\Immersive\eventTracker.lua` L1803
- Debug call: print()
- [ ] Status: Pending

**[36]** 🐛 `Mainline\Immersive\eventTracker.lua` L1804
- Debug call: print()
- [ ] Status: Pending

**[37]** 🐛 `Mainline\Immersive\eventTracker.lua` L1805
- Debug call: print()
- [ ] Status: Pending

**[38]** 🐛 `Mainline\Immersive\eventTracker.lua` L1806
- Debug call: print()
- [ ] Status: Pending

**[39]** 🐛 `core\debug.lua` L35
- Debug call: DebugLog()
- [ ] Status: Pending

**[40]** 🐛 `core\debug.lua` L39
- Debug call: DebugLog()
- [ ] Status: Pending

**[41]** 🐛 `core\debug.lua` L42
- Debug call: DebugLog()
- [ ] Status: Pending

**[42]** 🐛 `core\debug.lua` L45
- Debug call: DebugLog()
- [ ] Status: Pending

### Priority 5: `global_write`

**[43]** 🔴 `Classic\Character\character.lua` L1012
- Global write: arg1
- Variable: `arg1`
- [ ] Status: Pending

**[44]** 🔴 `Classic\Immersive\minimap.lua` L371
- Global write: GetMinimapShape
- Variable: `GetMinimapShape`
- [ ] Status: Pending

**[45]** 🔴 `Classic\Immersive\minimap.lua` L381
- Global write: GwMapGradient
- Variable: `GwMapGradient`
- [ ] Status: Pending

**[46]** 🔴 `Classic\Immersive\minimap.lua` L402
- Global write: GwMiniMapTrackingFrame
- Variable: `GwMiniMapTrackingFrame`
- [ ] Status: Pending

**[47]** 🔴 `Classic\Immersive\minimap.lua` L430
- Global write: GwMapTime
- Variable: `GwMapTime`
- [ ] Status: Pending

**[48]** 🔴 `Classic\Immersive\minimap.lua` L446
- Global write: GwMapCoords
- Variable: `GwMapCoords`
- [ ] Status: Pending

**[49]** 🔴 `Classic\Immersive\minimap.lua` L454
- Global write: GwMapFPS
- Variable: `GwMapFPS`
- [ ] Status: Pending

**[50]** 🔴 `Classic\Mixin\ObjectivesItemButtonMixin.lua` L1
- Global write: GwObjectivesItemButtonMixin
- Variable: `GwObjectivesItemButtonMixin`
- [ ] Status: Pending

**[51]** 🔴 `Classic\Objectives\objectives.lua` L174
- Global write: GwQuestLogBlockMixin
- Variable: `GwQuestLogBlockMixin`
- [ ] Status: Pending

**[52]** 🔴 `Classic\Objectives\objectives.lua` L196
- Global write: GwQuestLogMixin
- Variable: `GwQuestLogMixin`
- [ ] Status: Pending

**[53]** 🔴 `Classic\Objectives\objectives.lua` L442
- Global write: GwObjectivesQuestContainerMixin
- Variable: `GwObjectivesQuestContainerMixin`
- [ ] Status: Pending

**[54]** 🔴 `Classic\Objectives\objectives.lua` L535
- Global write: IsQuestWatched
- Variable: `IsQuestWatched`
- [ ] Status: Pending

**[55]** 🔴 `Classic\Objectives\objectives.lua` L549
- Global write: GetNumQuestWatches
- Variable: `GetNumQuestWatches`
- [ ] Status: Pending

**[56]** 🔴 `Classic\Objectives\objectives.lua` L554
- Global write: QuestLogTitleButton_OnClick
- Variable: `QuestLogTitleButton_OnClick`
- [ ] Status: Pending

**[57]** 🔴 `Libs\Core\CallbackHandler-1.0\CallbackHandler-1.0.lua` L97
- Global write: method
- Variable: `method`
- [ ] Status: Pending

**[58]** 🔴 `Libs\Core\LibRealmInfo\LibRealmInfo.lua` L1899
- Global write: LRI_RealmData
- Variable: `LRI_RealmData`
- [ ] Status: Pending

**[59]** 🔴 `Libs\Core\LibRealmInfo\LibRealmInfo.lua` L1900
- Global write: LRI_ConnectionData
- Variable: `LRI_ConnectionData`
- [ ] Status: Pending

**[60]** 🔴 `Libs\Core\oUF\colors.lua` L11
- Global write: r
- Variable: `r`
- [ ] Status: Pending

**[61]** 🔴 `Libs\Core\oUF\colors.lua` L11
- Global write: g
- Variable: `g`
- [ ] Status: Pending

**[62]** 🔴 `Libs\Core\oUF\colors.lua` L11
- Global write: b
- Variable: `b`
- [ ] Status: Pending

**[63]** 🔴 `Libs\Core\oUF\elements\tags.lua` L468
- Global write: val
- Variable: `val`
- [ ] Status: Pending

**[64]** 🔴 `Libs\Core\oUF\elements\tags.lua` L495
- Global write: val
- Variable: `val`
- [ ] Status: Pending

**[65]** 🔴 `Libs\Core\oUF\elements\tags.lua` L912
- Global write: tag
- Variable: `tag`
- [ ] Status: Pending

**[66]** 🔴 `Libs\Core\oUF\elements\tags.lua` L941
- Global write: tag
- Variable: `tag`
- [ ] Status: Pending

**[67]** 🔴 `Mainline\Character\paperdoll_equipment.lua` L671
- Global write: step
- Variable: `step`
- [ ] Status: Pending

**[68]** 🔴 `Mainline\Character\paperdoll_equipment.lua` L674
- Global write: step
- Variable: `step`
- [ ] Status: Pending

**[69]** 🔴 `Mainline\Immersive\Skins\achievements.lua` L210
- Global write: AchievementFrameAchievements_UpdateDataProvider
- Variable: `AchievementFrameAchievements_UpdateDataProvider`
- [ ] Status: Pending

**[70]** 🔴 `Mainline\Immersive\Skins\achievements.lua` L1105
- Global write: AchivementFrameLeftPanel
- Variable: `AchivementFrameLeftPanel`
- [ ] Status: Pending

**[71]** 🔴 `Mainline\Immersive\Skins\addons\WorldQuestTracker.lua` L4
- Global write: GwWorldQuestTrackerContainerMixin
- Variable: `GwWorldQuestTrackerContainerMixin`
- [ ] Status: Pending

**[72]** 🔴 `Mainline\Immersive\Skins\addons\petTracker.lua` L6
- Global write: GwPetTrackerContainerMixin
- Variable: `GwPetTrackerContainerMixin`
- [ ] Status: Pending

**[73]** 🔴 `Mainline\Immersive\Skins\addons\todoloo.lua` L4
- Global write: GwTodolooContainerMixin
- Variable: `GwTodolooContainerMixin`
- [ ] Status: Pending

**[74]** 🔴 `Mainline\Immersive\Skins\addons\todoloo.lua` L5
- Global write: GwTodolooBlockMixin
- Variable: `GwTodolooBlockMixin`
- [ ] Status: Pending

**[75]** 🔴 `Mainline\Immersive\minimap.lua` L618
- Global write: GwMapTime
- Variable: `GwMapTime`
- [ ] Status: Pending

**[76]** 🔴 `Mainline\Immersive\minimap.lua` L633
- Global write: GwMapCoords
- Variable: `GwMapCoords`
- [ ] Status: Pending

**[77]** 🔴 `Mainline\Immersive\minimap.lua` L641
- Global write: GwMapFPS
- Variable: `GwMapFPS`
- [ ] Status: Pending

**[78]** 🔴 `Mainline\Objectives\bonusObjective.lua` L17
- Global write: GwBonusObjectivesTrackerBlockMixin
- Variable: `GwBonusObjectivesTrackerBlockMixin`
- [ ] Status: Pending

**[79]** 🔴 `Mainline\Objectives\bonusObjective.lua` L95
- Global write: GwBonusObjectivesTrackerContainerMixin
- Variable: `GwBonusObjectivesTrackerContainerMixin`
- [ ] Status: Pending

**[80]** 🔴 `Mainline\Objectives\collectionTracking.lua` L11
- Global write: GwObjectivesCollectionBlockMixin
- Variable: `GwObjectivesCollectionBlockMixin`
- [ ] Status: Pending

**[81]** 🔴 `Mainline\Objectives\collectionTracking.lua` L81
- Global write: GwObjectivesCollectionContainerMixin
- Variable: `GwObjectivesCollectionContainerMixin`
- [ ] Status: Pending

**[82]** 🔴 `Mainline\Objectives\housingInitiative.lua` L7
- Global write: GwObjectivesHousingInitiativeBlockMixin
- Variable: `GwObjectivesHousingInitiativeBlockMixin`
- [ ] Status: Pending

**[83]** 🔴 `Mainline\Objectives\housingInitiative.lua` L29
- Global write: GwObjectivesHousingInitiativeContainerMixin
- Variable: `GwObjectivesHousingInitiativeContainerMixin`
- [ ] Status: Pending

**[84]** 🔴 `Mainline\Objectives\monthlyActivitiesTracking.lua` L7
- Global write: GwObjectivesMonthlyActivitiesBlockMixin
- Variable: `GwObjectivesMonthlyActivitiesBlockMixin`
- [ ] Status: Pending

**[85]** 🔴 `Mainline\Objectives\monthlyActivitiesTracking.lua` L29
- Global write: GwObjectivesMonthlyActivitiesContainerMixin
- Variable: `GwObjectivesMonthlyActivitiesContainerMixin`
- [ ] Status: Pending

**[86]** 🔴 `Mainline\Objectives\objectives.lua` L115
- Global write: GwQuestLogBlockMixin
- Variable: `GwQuestLogBlockMixin`
- [ ] Status: Pending

**[87]** 🔴 `Mainline\Objectives\objectives.lua` L136
- Global write: GwQuestLogMixin
- Variable: `GwQuestLogMixin`
- [ ] Status: Pending

**[88]** 🔴 `Mainline\Objectives\objectives.lua` L440
- Global write: GwObjectivesQuestContainerMixin
- Variable: `GwObjectivesQuestContainerMixin`
- [ ] Status: Pending

**[89]** 🔴 `Mainline\Objectives\recipeTracking.lua` L16
- Global write: GwObjectivesRecipeBlockMixin
- Variable: `GwObjectivesRecipeBlockMixin`
- [ ] Status: Pending

**[90]** 🔴 `Mainline\Objectives\recipeTracking.lua` L50
- Global write: GwObjectivesRecipeContainerMixin
- Variable: `GwObjectivesRecipeContainerMixin`
- [ ] Status: Pending

**[91]** 🔴 `Mainline\Units\healthglobe.lua` L5
- Global write: GwHealthglobeMixin
- Variable: `GwHealthglobeMixin`
- [ ] Status: Pending

**[92]** 🔴 `Mainline\Units\healthglobe.lua` L138
- Global write: GwHealthglobeRepairMixin
- Variable: `GwHealthglobeRepairMixin`
- [ ] Status: Pending

**[93]** 🔴 `Mists\Character\paperdoll_equipment.lua` L147
- Global write: step
- Variable: `step`
- [ ] Status: Pending

**[94]** 🔴 `Mists\Character\paperdoll_equipment.lua` L150
- Global write: step
- Variable: `step`
- [ ] Status: Pending

**[95]** 🔴 `Mists\Immersive\minimap.lua` L329
- Global write: GetMinimapShape
- Variable: `GetMinimapShape`
- [ ] Status: Pending

**[96]** 🔴 `Mists\Immersive\minimap.lua` L365
- Global write: GwMapGradient
- Variable: `GwMapGradient`
- [ ] Status: Pending

**[97]** 🔴 `Mists\Immersive\minimap.lua` L370
- Global write: GwMiniMapTrackingFrame
- Variable: `GwMiniMapTrackingFrame`
- [ ] Status: Pending

**[98]** 🔴 `Mists\Immersive\minimap.lua` L394
- Global write: GwMapTime
- Variable: `GwMapTime`
- [ ] Status: Pending

**[99]** 🔴 `Mists\Immersive\minimap.lua` L408
- Global write: GwMapCoords
- Variable: `GwMapCoords`
- [ ] Status: Pending

**[100]** 🔴 `Mists\Immersive\minimap.lua` L416
- Global write: GwMapFPS
- Variable: `GwMapFPS`
- [ ] Status: Pending

**[101]** 🔴 `Mists\Mixin\ObjectivesItemButtonMixin.lua` L1
- Global write: GwObjectivesItemButtonMixin
- Variable: `GwObjectivesItemButtonMixin`
- [ ] Status: Pending

**[102]** 🔴 `Mists\Objectives\objectives.lua` L150
- Global write: GwQuestLogBlockMixin
- Variable: `GwQuestLogBlockMixin`
- [ ] Status: Pending

**[103]** 🔴 `Mists\Objectives\objectives.lua` L170
- Global write: GwQuestLogMixin
- Variable: `GwQuestLogMixin`
- [ ] Status: Pending

**[104]** 🔴 `Mists\Objectives\objectives.lua` L451
- Global write: GwObjectivesQuestContainerMixin
- Variable: `GwObjectivesQuestContainerMixin`
- [ ] Status: Pending

**[105]** 🔴 `TBC\Character\character.lua` L846
- Global write: arg1
- Variable: `arg1`
- [ ] Status: Pending

**[106]** 🔴 `TBC\Immersive\minimap.lua` L376
- Global write: GetMinimapShape
- Variable: `GetMinimapShape`
- [ ] Status: Pending

**[107]** 🔴 `TBC\Immersive\minimap.lua` L388
- Global write: GwMapGradient
- Variable: `GwMapGradient`
- [ ] Status: Pending

**[108]** 🔴 `TBC\Immersive\minimap.lua` L410
- Global write: GwMapTime
- Variable: `GwMapTime`
- [ ] Status: Pending

**[109]** 🔴 `TBC\Immersive\minimap.lua` L426
- Global write: GwMapCoords
- Variable: `GwMapCoords`
- [ ] Status: Pending

**[110]** 🔴 `TBC\Immersive\minimap.lua` L434
- Global write: GwMapFPS
- Variable: `GwMapFPS`
- [ ] Status: Pending

**[111]** 🔴 `TBC\Mixin\ObjectivesItemButtonMixin.lua` L1
- Global write: GwObjectivesItemButtonMixin
- Variable: `GwObjectivesItemButtonMixin`
- [ ] Status: Pending

**[112]** 🔴 `TBC\Objectives\objectives.lua` L174
- Global write: GwQuestLogBlockMixin
- Variable: `GwQuestLogBlockMixin`
- [ ] Status: Pending

**[113]** 🔴 `TBC\Objectives\objectives.lua` L196
- Global write: GwQuestLogMixin
- Variable: `GwQuestLogMixin`
- [ ] Status: Pending

**[114]** 🔴 `TBC\Objectives\objectives.lua` L442
- Global write: GwObjectivesQuestContainerMixin
- Variable: `GwObjectivesQuestContainerMixin`
- [ ] Status: Pending

**[115]** 🔴 `TBC\Objectives\objectives.lua` L535
- Global write: IsQuestWatched
- Variable: `IsQuestWatched`
- [ ] Status: Pending

**[116]** 🔴 `TBC\Objectives\objectives.lua` L549
- Global write: GetNumQuestWatches
- Variable: `GetNumQuestWatches`
- [ ] Status: Pending

**[117]** 🔴 `TBC\Objectives\objectives.lua` L554
- Global write: QuestLogTitleButton_OnClick
- Variable: `QuestLogTitleButton_OnClick`
- [ ] Status: Pending

**[118]** 🔴 `core\Castingbar\castingbar.lua` L25
- Global write: GwCastingBarMixin
- Variable: `GwCastingBarMixin`
- [ ] Status: Pending

**[119]** 🔴 `core\Castingbar\castingbar.lua` L425
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[120]** 🔴 `core\Immersive\QuestReqItems.lua` L3
- Global write: GwQuestReqItemsFrameMixin
- Variable: `GwQuestReqItemsFrameMixin`
- [ ] Status: Pending

**[121]** 🔴 `core\Immersive\QuestView.lua` L223
- Global write: GwQuestViewFrameMixin
- Variable: `GwQuestViewFrameMixin`
- [ ] Status: Pending

**[122]** 🔴 `core\Immersive\Skins\gossip.lua` L246
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[123]** 🔴 `core\Immersive\Skins\gossip.lua` L401
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[124]** 🔴 `core\Immersive\Skins\menu.lua` L32
- Global write: level
- Variable: `level`
- [ ] Status: Pending

**[125]** 🔴 `core\Immersive\chatframe.lua` L354
- Global write: x
- Variable: `x`
- [ ] Status: Pending

**[126]** 🔴 `core\Immersive\chatframe.lua` L372
- Global write: text
- Variable: `text`
- [ ] Status: Pending

**[127]** 🔴 `core\Immersive\chatframe.lua` L373
- Global write: text
- Variable: `text`
- [ ] Status: Pending

**[128]** 🔴 `core\Immersive\chatframe.lua` L374
- Global write: text
- Variable: `text`
- [ ] Status: Pending

**[129]** 🔴 `core\Immersive\chatframe.lua` L375
- Global write: text
- Variable: `text`
- [ ] Status: Pending

**[130]** 🔴 `core\Mixin\GwObjectivesAnimationMixin.lua` L3
- Global write: GwObjectivesAnimationMixin
- Variable: `GwObjectivesAnimationMixin`
- [ ] Status: Pending

**[131]** 🔴 `core\Mixin\GwObjectivesBlockMixin.lua` L3
- Global write: GwObjectivesBlockTemplateMixin
- Variable: `GwObjectivesBlockTemplateMixin`
- [ ] Status: Pending

**[132]** 🔴 `core\Mixin\GwObjectivesContainerMixin.lua` L3
- Global write: GwObjectivesContainerMixin
- Variable: `GwObjectivesContainerMixin`
- [ ] Status: Pending

**[133]** 🔴 `core\Mixin\GwObjectivesGroupfinderButtonMixin.lua` L1
- Global write: GwObjectivesGroupfinderButtonMixin
- Variable: `GwObjectivesGroupfinderButtonMixin`
- [ ] Status: Pending

**[134]** 🔴 `core\Mixin\GwObjectivesUnitFrameMixin.lua` L3
- Global write: GwObjectivesUnitFrameMixin
- Variable: `GwObjectivesUnitFrameMixin`
- [ ] Status: Pending

**[135]** 🔴 `core\Mixin\GwQuestTrackerObjectiveMixin.lua` L3
- Global write: GwQuestTrackerObjectiveMixin
- Variable: `GwQuestTrackerObjectiveMixin`
- [ ] Status: Pending

**[136]** 🔴 `core\Mixin\healthBarMixin.lua` L3
- Global write: GwUnitHealthbarMixin
- Variable: `GwUnitHealthbarMixin`
- [ ] Status: Pending

**[137]** 🔴 `core\Mixin\powerBarMixin.lua` L4
- Global write: GwUnitPowerbarMixin
- Variable: `GwUnitPowerbarMixin`
- [ ] Status: Pending

**[138]** 🔴 `core\Objectives\ObjectivesTracker.lua` L94
- Global write: GwObjectivesTrackerMixin
- Variable: `GwObjectivesTrackerMixin`
- [ ] Status: Pending

**[139]** 🔴 `core\Objectives\ObjectivesTracker.lua` L187
- Global write: delta
- Variable: `delta`
- [ ] Status: Pending

**[140]** 🔴 `core\Objectives\achievement.lua` L8
- Global write: GwAchievementTrackerBlockMixin
- Variable: `GwAchievementTrackerBlockMixin`
- [ ] Status: Pending

**[141]** 🔴 `core\Objectives\achievement.lua` L78
- Global write: GwAchievementTrackerContainerMixin
- Variable: `GwAchievementTrackerContainerMixin`
- [ ] Status: Pending

**[142]** 🔴 `core\Objectives\arenaFrames.lua` L20
- Global write: GwArenaFrameMixin
- Variable: `GwArenaFrameMixin`
- [ ] Status: Pending

**[143]** 🔴 `core\Objectives\arenaFrames.lua` L113
- Global write: GwArenaPrepFrameMixin
- Variable: `GwArenaPrepFrameMixin`
- [ ] Status: Pending

**[144]** 🔴 `core\Objectives\arenaFrames.lua` L120
- Global write: GwObjectivesArenaContainerMixin
- Variable: `GwObjectivesArenaContainerMixin`
- [ ] Status: Pending

**[145]** 🔴 `core\Objectives\bossFrames.lua` L5
- Global write: GwBossFrameMixin
- Variable: `GwBossFrameMixin`
- [ ] Status: Pending

**[146]** 🔴 `core\Objectives\bossFrames.lua` L91
- Global write: GwObjectivesBossContainerMixin
- Variable: `GwObjectivesBossContainerMixin`
- [ ] Status: Pending

**[147]** 🔴 `core\Objectives\notifications.lua` L408
- Global write: GwObjectivesTrackerNotificationMixin
- Variable: `GwObjectivesTrackerNotificationMixin`
- [ ] Status: Pending

**[148]** 🔴 `core\Objectives\notifications.lua` L446
- Global write: step
- Variable: `step`
- [ ] Status: Pending

**[149]** 🔴 `core\Objectives\scenario.lua` L30
- Global write: GwObjectivesScenarioContainerMixin
- Variable: `GwObjectivesScenarioContainerMixin`
- [ ] Status: Pending

**[150]** 🔴 `core\Objectives\scenario.lua` L31
- Global write: GwQuesttrackerScenarioBlockMixin
- Variable: `GwQuesttrackerScenarioBlockMixin`
- [ ] Status: Pending

**[151]** 🔴 `core\Social\friends.lua` L620
- Global write: msg
- Variable: `msg`
- [ ] Status: Pending

**[152]** 🔴 `core\Social\raid.lua` L214
- Global write: ClaimRaidFrame
- Variable: `ClaimRaidFrame`
- [ ] Status: Pending

**[153]** 🔴 `core\Social\who.lua` L247
- Global write: msg
- Variable: `msg`
- [ ] Status: Pending

**[154]** 🔴 `core\Stancebar\stancebar.lua` L7
- Global write: GwStanceBarMixin
- Variable: `GwStanceBarMixin`
- [ ] Status: Pending

**[155]** 🔴 `core\Statusbar\statusbar.lua` L31
- Global write: GwAnimatedStatusBarMixin
- Variable: `GwAnimatedStatusBarMixin`
- [ ] Status: Pending

**[156]** 🔴 `core\Units\Grid\configEnvironment.lua` L47
- Global write: r
- Variable: `r`
- [ ] Status: Pending

**[157]** 🔴 `core\Units\Grid\configEnvironment.lua` L47
- Global write: g
- Variable: `g`
- [ ] Status: Pending

**[158]** 🔴 `core\Units\Grid\configEnvironment.lua` L47
- Global write: b
- Variable: `b`
- [ ] Status: Pending

**[159]** 🔴 `core\Units\Grid\configEnvironment.lua` L47
- Global write: r
- Variable: `r`
- [ ] Status: Pending

**[160]** 🔴 `core\Units\Grid\configEnvironment.lua` L47
- Global write: g
- Variable: `g`
- [ ] Status: Pending

**[161]** 🔴 `core\Units\Grid\configEnvironment.lua` L47
- Global write: b
- Variable: `b`
- [ ] Status: Pending

**[162]** 🔴 `core\Units\classpowers.lua` L284
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[163]** 🔴 `core\Units\classpowers.lua` L306
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[164]** 🔴 `core\Units\classpowers.lua` L516
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[165]** 🔴 `core\Units\classpowers.lua` L1535
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[166]** 🔴 `core\Units\comboBarTarget.lua` L63
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[167]** 🔴 `core\Units\dodgebar.lua` L58
- Global write: GwDodgeBarMixin
- Variable: `GwDodgeBarMixin`
- [ ] Status: Pending

**[168]** 🔴 `core\Units\healthglobe.lua` L7
- Global write: GwHealthglobeMixin
- Variable: `GwHealthglobeMixin`
- [ ] Status: Pending

**[169]** 🔴 `core\Units\healthglobe.lua` L137
- Global write: GwHealthglobeRepairMixin
- Variable: `GwHealthglobeRepairMixin`
- [ ] Status: Pending

**[170]** 🔴 `core\Units\party.lua` L79
- Global write: GwPartyFrameMixin
- Variable: `GwPartyFrameMixin`
- [ ] Status: Pending

**[171]** 🔴 `core\Units\petbar.lua` L13
- Global write: GwPlayerPetFrameMixin
- Variable: `GwPlayerPetFrameMixin`
- [ ] Status: Pending

**[172]** 🔴 `core\Units\playerFrame.lua` L5
- Global write: GwPlayerUnitFrameMixin
- Variable: `GwPlayerUnitFrameMixin`
- [ ] Status: Pending

**[173]** 🔴 `core\Units\powerbar.lua` L4
- Global write: GwPlayerPowerBarMixin
- Variable: `GwPlayerPowerBarMixin`
- [ ] Status: Pending

**[174]** 🔴 `core\Units\unitframes.lua` L314
- Global write: GwUnitFrameMixin
- Variable: `GwUnitFrameMixin`
- [ ] Status: Pending

**[175]** 🔴 `core\Units\unitframes.lua` L723
- Global write: p
- Variable: `p`
- [ ] Status: Pending

**[176]** 🔴 `core\Units\unitframes.lua` L1051
- Global write: GwTargetUnitFrameMixin
- Variable: `GwTargetUnitFrameMixin`
- [ ] Status: Pending

**[177]** 🔴 `core\disableBlizzard.lua` L122
- Global write: Arena_LoadUI
- Variable: `Arena_LoadUI`
- [ ] Status: Pending

**[178]** 🔴 `core\errorHandler.lua` L5
- Global write: Gw2ErrorHandlerMixin
- Variable: `Gw2ErrorHandlerMixin`
- [ ] Status: Pending

**[179]** 🔴 `core\errorHandler.lua` L166
- Global write: lvl
- Variable: `lvl`
- [ ] Status: Pending

**[180]** 🔴 `settings\profileSpecSwitch.lua` L32
- Global write: GetSpecializationInfoForClassID
- Variable: `GetSpecializationInfoForClassID`
- [ ] Status: Pending

**[181]** 🔴 `settings\settingsUtils.lua` L179
- Global write: GwSettingsPanelMixin
- Variable: `GwSettingsPanelMixin`
- [ ] Status: Pending

**[182]** 🔴 `settings\settingsWindow.lua` L4
- Global write: GwSettingsWindowMixin
- Variable: `GwSettingsWindowMixin`
- [ ] Status: Pending

**[183]** 🔴 `settings\settingsWindowSettingsTab.lua` L37
- Global write: GwSettingsWindowSettingsTabMixin
- Variable: `GwSettingsWindowSettingsTabMixin`
- [ ] Status: Pending

### Priority 3: `unused_local_function`

**[184]** 🟡 `Classic\Actionbar\actionbars.lua` L1151
- Local function 'changeFlyoutStyle' appears to be unused in <global>
- [ ] Status: Pending

**[185]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L534
- Local function 'band64' appears to be unused in <global>
- [ ] Status: Pending

**[186]** 🟡 `Libs\Core\oUF\blizzard.lua` L20
- Local function 'insecureHide' appears to be unused in <global>
- [ ] Status: Pending

**[187]** 🟡 `Mainline\Units\healthglobe.lua` L26
- Local function 'formatShieldValue' appears to be unused in <global>
- [ ] Status: Pending

**[188]** 🟡 `core\Immersive\hudart.lua` L391
- Local function 'loadFXModelDebug' appears to be unused in <global>
- [ ] Status: Pending

**[189]** 🟡 `core\Units\classpowers.lua` L1020
- Local function 'setHunter' appears to be unused in <global>
- [ ] Status: Pending

### Priority 2: `unused_local_variable`

**[190]** 🟡 `Classic\Character\character.lua` L580
- Local variable 'numTempPoints' is assigned but never used in <fornum>
- [ ] Status: Pending

**[191]** 🟡 `Classic\Character\character.lua` L580
- Local variable 'skillModifier' is assigned but never used in <fornum>
- [ ] Status: Pending

**[192]** 🟡 `Classic\Character\character.lua` L580
- Local variable 'stepCost' is assigned but never used in <fornum>
- [ ] Status: Pending

**[193]** 🟡 `Classic\Character\character.lua` L580
- Local variable 'rankCost' is assigned but never used in <fornum>
- [ ] Status: Pending

**[194]** 🟡 `Classic\Character\character.lua` L580
- Local variable 'minLevel' is assigned but never used in <fornum>
- [ ] Status: Pending

**[195]** 🟡 `Classic\Character\character.lua` L580
- Local variable 'skillCostType' is assigned but never used in <fornum>
- [ ] Status: Pending

**[196]** 🟡 `Classic\Character\stats.lua` L215
- Local variable 'damageText' is assigned but never used in getDamage
- [ ] Status: Pending

**[197]** 🟡 `Classic\Character\stats.lua` L216
- Local variable 'damageFrame' is assigned but never used in getDamage
- [ ] Status: Pending

**[198]** 🟡 `Classic\Objectives\objectives.lua` L358
- Local variable 'submenuObjectives' is assigned but never used in BlockOnClick
- [ ] Status: Pending

**[199]** 🟡 `Libs\Core\AceLocale-3.0\AceLocale-3.0.lua` L7
- Local variable 'oldminor' is assigned but never used in <global>
- [ ] Status: Pending

**[200]** 🟡 `Libs\Core\AceSerializer-3.0\AceSerializer-3.0.lua` L15
- Local variable 'oldminor' is assigned but never used in <global>
- [ ] Status: Pending

**[201]** 🟡 `Libs\Core\AceSerializer-3.0\AceSerializer-3.0.lua` L29
- Local variable 'serNaN' is assigned but never used in <global>
- [ ] Status: Pending

**[202]** 🟡 `Libs\Core\AceSerializer-3.0\AceSerializer-3.0.lua` L251
- Local variable 'data' is assigned but never used in Deserialize
- [ ] Status: Pending

**[203]** 🟡 `Libs\Core\CallbackHandler-1.0\CallbackHandler-1.0.lua` L10
- Local variable 'tconcat' is assigned but never used in <global>
- [ ] Status: Pending

**[204]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L34
- Local variable 'table_insert' is assigned but never used in <global>
- [ ] Status: Pending

**[205]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L39
- Local variable 'string_len' is assigned but never used in <global>
- [ ] Status: Pending

**[206]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L43
- Local variable 'math_modf' is assigned but never used in <global>
- [ ] Status: Pending

**[207]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L465
- Local variable 'success' is assigned but never used in CompressHuffman
- [ ] Status: Pending

**[208]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L465
- Local variable 'msg' is assigned but never used in CompressHuffman
- [ ] Status: Pending

**[209]** 🟡 `Libs\Core\LibCustomGlow\LibCustomGlow-1.0.lua` L11
- Local variable 'oldversion' is assigned but never used in <global>
- [ ] Status: Pending

**[210]** 🟡 `Libs\Core\LibCustomGlow\LibCustomGlow-1.0.lua` L527
- Local variable 'frameWidth' is assigned but never used in AnimIn_OnStop
- [ ] Status: Pending

**[211]** 🟡 `Libs\Core\LibCustomGlow\LibCustomGlow-1.0.lua` L527
- Local variable 'frameHeight' is assigned but never used in AnimIn_OnStop
- [ ] Status: Pending

**[212]** 🟡 `Libs\Core\LibDeflate\LibDeflate.lua` L2675
- Local variable 'FLEVEL' is assigned but never used in DecompressZlibInternal
- [ ] Status: Pending

**[213]** 🟡 `Libs\Core\LibGW2\LibGW2.lua` L14
- Local variable 'isTBC' is assigned but never used in <global>
- [ ] Status: Pending

**[214]** 🟡 `Libs\Core\LibGW2\LibGW2.lua` L15
- Local variable 'isCata' is assigned but never used in <global>
- [ ] Status: Pending

**[215]** 🟡 `Libs\Core\LibGW2\LibGW2.lua` L16
- Local variable 'isWrath' is assigned but never used in <global>
- [ ] Status: Pending

**[216]** 🟡 `Libs\Core\LibGW2\LibGW2.lua` L18
- Local variable 'isClassic' is assigned but never used in <global>
- [ ] Status: Pending

**[217]** 🟡 `Libs\Core\LibRealmInfo\LibRealmInfo.lua` L13
- Local variable 'oldminor' is assigned but never used in <global>
- [ ] Status: Pending

**[218]** 🟡 `Libs\Core\oUF\elements\healthprediction.lua` L126
- Local variable 'playerHeal' is assigned but never used in Update
- [ ] Status: Pending

**[219]** 🟡 `Mainline\Character\spellbook.lua` L7
- Local variable 'maxTalentRows' is assigned but never used in <global>
- [ ] Status: Pending

**[220]** 🟡 `Mainline\Character\spellbook.lua` L8
- Local variable 'talentsPerRow' is assigned but never used in <global>
- [ ] Status: Pending

**[221]** 🟡 `Mainline\Immersive\Skins\achievements.lua` L183
- Local variable 'numCompleted' is assigned but never used in UpdateCategoriesDataProvider
- [ ] Status: Pending

**[222]** 🟡 `Mainline\Immersive\Skins\achievements.lua` L219
- Local variable 'numIncomplete' is assigned but never used in AchievementFrameCategories_OnLoad
- [ ] Status: Pending

**[223]** 🟡 `Mists\Character\glyphs.lua` L46
- Local variable 'glyphType' is assigned but never used in <fornum>
- [ ] Status: Pending

**[224]** 🟡 `Mists\Character\glyphs.lua` L46
- Local variable 'icon' is assigned but never used in <fornum>
- [ ] Status: Pending

**[225]** 🟡 `Mists\Character\glyphs.lua` L46
- Local variable 'glyphID' is assigned but never used in <fornum>
- [ ] Status: Pending

**[226]** 🟡 `Mists\Mixin\ObjectivesItemButtonMixin.lua` L20
- Local variable 'link' is assigned but never used in OnUpdate
- [ ] Status: Pending

**[227]** 🟡 `Mists\Mixin\ObjectivesItemButtonMixin.lua` L20
- Local variable 'item' is assigned but never used in OnUpdate
- [ ] Status: Pending

**[228]** 🟡 `Mists\Mixin\ObjectivesItemButtonMixin.lua` L20
- Local variable 'showItemWhenComplete' is assigned but never used in OnUpdate
- [ ] Status: Pending

**[229]** 🟡 `Mists\Objectives\objectives.lua` L353
- Local variable 'submenuObjectives' is assigned but never used in BlockOnClick
- [ ] Status: Pending

**[230]** 🟡 `TBC\Character\character.lua` L580
- Local variable 'numTempPoints' is assigned but never used in <fornum>
- [ ] Status: Pending

**[231]** 🟡 `TBC\Character\character.lua` L580
- Local variable 'skillModifier' is assigned but never used in <fornum>
- [ ] Status: Pending

**[232]** 🟡 `TBC\Character\character.lua` L580
- Local variable 'stepCost' is assigned but never used in <fornum>
- [ ] Status: Pending

**[233]** 🟡 `TBC\Character\character.lua` L580
- Local variable 'rankCost' is assigned but never used in <fornum>
- [ ] Status: Pending

**[234]** 🟡 `TBC\Character\character.lua` L580
- Local variable 'minLevel' is assigned but never used in <fornum>
- [ ] Status: Pending

**[235]** 🟡 `TBC\Character\character.lua` L580
- Local variable 'skillCostType' is assigned but never used in <fornum>
- [ ] Status: Pending

**[236]** 🟡 `TBC\Character\stats.lua` L215
- Local variable 'damageText' is assigned but never used in getDamage
- [ ] Status: Pending

**[237]** 🟡 `TBC\Character\stats.lua` L216
- Local variable 'damageFrame' is assigned but never used in getDamage
- [ ] Status: Pending

**[238]** 🟡 `TBC\Mixin\ObjectivesItemButtonMixin.lua` L20
- Local variable 'link' is assigned but never used in OnUpdate
- [ ] Status: Pending

**[239]** 🟡 `TBC\Mixin\ObjectivesItemButtonMixin.lua` L20
- Local variable 'item' is assigned but never used in OnUpdate
- [ ] Status: Pending

**[240]** 🟡 `TBC\Mixin\ObjectivesItemButtonMixin.lua` L20
- Local variable 'showItemWhenComplete' is assigned but never used in OnUpdate
- [ ] Status: Pending

**[241]** 🟡 `TBC\Objectives\objectives.lua` L358
- Local variable 'submenuObjectives' is assigned but never used in BlockOnClick
- [ ] Status: Pending

**[242]** 🟡 `core\Immersive\QuestView.lua` L224
- Local variable 'QuestViewMixin' is assigned but never used in <global>
- [ ] Status: Pending

**[243]** 🟡 `core\Misc\blizzardFixes.lua` L1
- Local variable 'GW' is assigned but never used in <global>
- [ ] Status: Pending

**[244]** 🟡 `core\Social\guild.lua` L26
- Local variable 'name' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[245]** 🟡 `core\Social\guild.lua` L28
- Local variable 'guildName' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[246]** 🟡 `core\Social\guild.lua` L28
- Local variable 'guildRankName' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[247]** 🟡 `core\Social\guild.lua` L220
- Local variable 'year' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[248]** 🟡 `core\Social\guild.lua` L220
- Local variable 'month' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[249]** 🟡 `core\Social\guild.lua` L220
- Local variable 'day' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[250]** 🟡 `core\Social\guild.lua` L220
- Local variable 'hour' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[251]** 🟡 `core\Social\guild.lua` L221
- Local variable 'yearlabel' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[252]** 🟡 `core\Social\guild.lua` L221
- Local variable 'monthlabel' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[253]** 🟡 `core\Social\guild.lua` L221
- Local variable 'daylabel' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[254]** 🟡 `core\Social\guild.lua` L221
- Local variable 'hourlabel' is assigned but never used in GuildStatus_Update
- [ ] Status: Pending

**[255]** 🟡 `core\debug.lua` L4
- Local variable 'P' is assigned but never used in <global>
- [ ] Status: Pending

**[256]** 🟡 `core\debug.lua` L25
- Local variable 'gName' is assigned but never used in AddProfiling
- [ ] Status: Pending

### Priority 1: `unnecessary_else`

**[257]** 🟡 `Classic\Actionbar\Binding.lua` L33
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[258]** 🟡 `Classic\Character\advanced_stats.lua` L132
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[259]** 🟡 `Classic\Character\sodEngravingFrame.lua` L37
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[260]** 🟡 `Classic\Character\sodEngravingFrame.lua` L46
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[261]** 🟡 `Classic\Character\spellbook.lua` L438
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[262]** 🟡 `Classic\Objectives\objectives.lua` L281
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[263]** 🟡 `Classic\Objectives\objectives.lua` L284
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[264]** 🟡 `Classic\Objectives\objectives.lua` L544
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[265]** 🟡 `Libs\Core\AceSerializer-3.0\AceSerializer-3.0.lua` L238
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[266]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L114
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[267]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L134
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[268]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L183
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[269]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L230
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[270]** 🟡 `Libs\Core\LibCompress\LibCompress.lua` L811
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[271]** 🟡 `Libs\Core\LibCustomGlow\LibCustomGlow-1.0.lua` L349
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[272]** 🟡 `Libs\Core\LibCustomGlow\LibCustomGlow-1.0.lua` L445
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[273]** 🟡 `Libs\Core\LibCustomGlow\LibCustomGlow-1.0.lua` L646
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[274]** 🟡 `Libs\Core\LibDeflate\LibDeflate.lua` L118
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[275]** 🟡 `Libs\Core\LibDeflate\LibDeflate.lua` L770
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[276]** 🟡 `Libs\Core\LibRealmInfo\LibRealmInfo.lua` L131
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[277]** 🟡 `Libs\Core\LibSharedMedia-3.0\LibSharedMedia-3.0.lua` L300
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[278]** 🟡 `Libs\Core\oUF\elements\tags.lua` L710
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[279]** 🟡 `Libs\Core\oUF\factory.lua` L40
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[280]** 🟡 `Libs\Core\oUF\private.lua` L72
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[281]** 🟡 `Mainline\Character\paperdoll_equipset.lua` L260
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[282]** 🟡 `Mainline\Character\reputation.lua` L809
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[283]** 🟡 `Mainline\Character\talents_pvp.lua` L255
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[284]** 🟡 `Mainline\Character\talents_pvp.lua` L301
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[285]** 🟡 `Mainline\Immersive\Skins\achievements.lua` L1436
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[286]** 🟡 `Mainline\Immersive\Skins\addons\todoloo.lua` L197
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[287]** 🟡 `Mainline\Immersive\eventTracker.lua` L227
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[288]** 🟡 `Mainline\Immersive\minimapInstanceDifficult.lua` L46
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[289]** 🟡 `Mainline\Immersive\minimapInstanceDifficult.lua` L57
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[290]** 🟡 `Mists\Actionbar\Binding.lua` L33
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[291]** 🟡 `Mists\Objectives\arenaFrames.lua` L127
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[292]** 🟡 `Mists\Objectives\objectives.lua` L281
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[293]** 🟡 `Mists\Objectives\objectives.lua` L284
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[294]** 🟡 `TBC\Actionbar\Binding.lua` L33
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[295]** 🟡 `TBC\Character\advanced_stats.lua` L132
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[296]** 🟡 `TBC\Character\spellbook.lua` L470
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[297]** 🟡 `TBC\Objectives\objectives.lua` L281
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[298]** 🟡 `TBC\Objectives\objectives.lua` L284
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[299]** 🟡 `TBC\Objectives\objectives.lua` L544
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[300]** 🟡 `core\API\api.lua` L9
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[301]** 🟡 `core\API\api.lua` L47
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[302]** 🟡 `core\API\api.lua` L57
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[303]** 🟡 `core\API\api.lua` L65
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[304]** 🟡 `core\API\api.lua` L95
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[305]** 🟡 `core\API\storage.lua` L86
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[306]** 🟡 `core\API\utils.lua` L492
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[307]** 🟡 `core\API\utils.lua` L560
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[308]** 🟡 `core\API\utils.lua` L585
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[309]** 🟡 `core\API\utils.lua` L594
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[310]** 🟡 `core\API\utils.lua` L706
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[311]** 🟡 `core\API\utils.lua` L716
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[312]** 🟡 `core\API\utils.lua` L726
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[313]** 🟡 `core\API\utils.lua` L735
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[314]** 🟡 `core\API\utils.lua` L905
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[315]** 🟡 `core\API\utils.lua` L918
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[316]** 🟡 `core\API\utils.lua` L1073
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[317]** 🟡 `core\API\utils.lua` L1101
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[318]** 🟡 `core\Castingbar\castingbar.lua` L208
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[319]** 🟡 `core\DataInfo\system.lua` L38
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[320]** 🟡 `core\GW2_ui.lua` L328
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[321]** 🟡 `core\Immersive\Skins\utils.lua` L333
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[322]** 🟡 `core\Immersive\chatframe.lua` L326
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[323]** 🟡 `core\Immersive\chatframe.lua` L975
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[324]** 🟡 `core\Immersive\chatframe.lua` L984
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[325]** 🟡 `core\Immersive\chatframe.lua` L1474
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[326]** 🟡 `core\Immersive\chatframe.lua` L1684
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[327]** 🟡 `core\Immersive\tooltips.lua` L394
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[328]** 🟡 `core\Immersive\tooltips.lua` L479
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[329]** 🟡 `core\Immersive\tooltips.lua` L576
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[330]** 🟡 `core\Immersive\tooltips.lua` L596
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[331]** 🟡 `core\Immersive\tooltips.lua` L856
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[332]** 🟡 `core\Misc\itemlevel.lua` L169
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[333]** 🟡 `core\Objectives\notifications.lua` L264
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[334]** 🟡 `core\Objectives\scenario.lua` L39
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[335]** 🟡 `core\Stancebar\stancebar.lua` L98
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[336]** 🟡 `core\Tests\mocks.lua` L8
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[337]** 🟡 `core\Tests\mocks.lua` L18
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[338]** 🟡 `core\Tests\mocks.lua` L27
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[339]** 🟡 `core\Tests\mocks.lua` L243
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[340]** 🟡 `core\Units\Grid\elements\auras.lua` L106
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[341]** 🟡 `core\Units\Grid\elements\auras.lua` L187
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[342]** 🟡 `core\Units\Grid\elements\tags.lua` L93
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[343]** 🟡 `core\Units\Grid\elements\tags.lua` L103
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[344]** 🟡 `core\Units\classpowers.lua` L357
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[345]** 🟡 `core\Units\classpowers.lua` L459
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[346]** 🟡 `core\Units\classpowers.lua` L1162
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[347]** 🟡 `core\Units\party.lua` L36
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[348]** 🟡 `core\Units\party.lua` L39
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[349]** 🟡 `core\cooldowns.lua` L37
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[350]** 🟡 `core\cooldowns.lua` L126
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[351]** 🟡 `core\init.lua` L35
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[352]** 🟡 `settings\layouts.lua` L378
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[353]** 🟡 `settings\settingsUtils.lua` L550
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

**[354]** 🟡 `settings\settingsWindowOverviewTab.lua` L225
- Unnecessary else after return/break - code can be simplified
- Suggestion: Remove else and dedent the else body
- [ ] Status: Pending

