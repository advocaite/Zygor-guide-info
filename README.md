## how to create a guide
first you need to reister a guide here is a template for you
```local ZygorGuidesViewer = ZygorGuidesViewer
if not ZygorGuidesViewer then return end
if UnitFactionGroup("player") ~= "Alliance" then return end
if ZGV:DoMutex("LevelingACLASSIC") then return end
ZygorGuidesViewer.GuideMenuTier = "CLA"
ZygorGuidesViewer:RegisterGuide("Leveling Guides\\Custom Guides\\My first guide", {
    author = "https://github.com/advocaite",
    image = ZGV.IMAGESDIR .. "Elwynn Forest",
    condition_suggested = function() return raceclass('Human') and level <= 12 end,
    condition_suggested_race = function() return raceclass('Human') end,
    condition_suggested_exclusive = true,
    next = "Leveling Guides\\Custom Guides\\My second guide",
    hardcore = true,
}, [[
step
Welcome to the Your first Guide!
Is this now awesome
confirm begin
]])
```
Save Location: *Interface\AddOns\ZygorGuidesViewerClassic\Guides-Classic\Includes\General*

Suggested Name:**A_Custom_guide_01.lua** or **H_Custom_guide_01.lua** **A= Alliance H= Horde**

open *Interface\AddOns\ZygorGuidesViewerClassic\Guides-Classic\Autoload.xml*

find 
```
<!-- INCLUDES -->
```
below this add the file you saved
```
<!-- CUSTOM -->
		<Script file="Includes\General\A_Custom_guide_01.lua"/>
```
Your Guide should now show up in the location you set in register guide function 

**if this does not work for some reason you can add this template below to the very end of the file called:**
*Interface\AddOns\ZygorGuidesViewerClassic\Guides-Classic\Leveling\ZygorLevelingAllianceCLASSIC.lua*
```
ZygorGuidesViewer:RegisterGuide("Leveling Guides\\Custom Guides\\My first guide", {
    author = "https://github.com/advocaite",
    image = ZGV.IMAGESDIR .. "Elwynn Forest",
    condition_suggested = function() return raceclass('Human') and level <= 12 end,
    condition_suggested_race = function() return raceclass('Human') end,
    condition_suggested_exclusive = true,
    next = "Leveling Guides\\Custom Guides\\My second guide",
    hardcore = true,
}, [[
step
Welcome to the Your first Guide!
Is this now awesome
confirm begin
]])
```


