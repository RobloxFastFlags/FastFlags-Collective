
<h1 align="center"> <img src="https://raw.githubusercontent.com/pizzaboxer/bloxstrap/main/Images/Bloxstrap.png" width="28" > Ultimate FastFlag List </h1>
<h3 align="center"> https://discord.gg/YreqZ7aYmg </h3>
<h5 align="center">Merely because this list highlights abusable fast flags doesn't imply we're promoting using them to unfairly impact others' gameplay. Remember, exploiting in Roblox goes against their ToU, and we don't support such activities. For more information, see Roblox's <a href="https://en.help.roblox.com/hc/en-us/articles/203312450-Cheating-and-Exploiting">Cheating and Exploiting</a> policy and <a href="https://en.help.roblox.com/hc/en-us/articles/115004647846-Roblox-Terms-of-Use">Terms of Use</h5>

## Bloxstrap How to Use:
1. **Open the [Bloxstrap Menu](https://github.com/pizzaboxer/bloxstrap).**
2. **Navigate to `Fast Flags` >> `Fast Flags Editor` >> `Import Json`.**
3. **Paste in the JSON.**
4. **Save and your good to go!**
<img src="/assets/tutorial.gif" width="750"/>

## Normal Roblox Bootstrapper  How to Use:
###### You can also do Roblox Studio
1. **Navigate to your Roblox Installation directory. Typically found at `%localappdata%\Roblox\Versions\` for Windows or `C:\Program Files (x86)\Roblox\Versions`.**
2. **Identify the folder `version-xxxxxxxxxxxxxxxx` ~~containing `RobloxPlayerBeta.exe`~~ You can do this for Roblox Studio too.**
3. **Create a new folder named `ClientSettings`. Inside this folder, place the file `ClientAppSettings.json`.**
4. **Paste the JSON into `ClientAppSettings.json`. (You can utilize ChatGPT to format multiple JSONs for clarity if needed)**
5. **Save and your good to go!**
###### Do note that after roblox updates you have to paste in your fflags again.

[Watch a Video Tutorial](https://streamable.com/rk5an6)

 # List Navigation
* **[Rendering](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#rendering-api)**
* **[Graphical](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#rendering-api)**
* **[UI](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#user-interface)**
* **[Textures](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#textures)**
* **[Physics](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#physics)**
* **[Other FFlags](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#other-fflags)**
* **[Links](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#links)**
* **[FastFlag Community Server](https://discord.gg/YreqZ7aYmg)**

<img src="assets/bitdancer.png" width="888"/>


<h3 align="center">══════⊹⊱≼≽⊰⊹══════</h3>

<h1 align="center">Lightning Technologies</h1>

### Voxel Lighting
```json
{
		"DFFlagDebugRenderForceTechnologyVoxel": "True"
}
```
### Shadowmap Lighting
```json
{
		"FFlagDebugForceFutureIsBrightPhase2": "True"
}
```
### Future Lighting
```json
{
		"FFlagDebugForceFutureIsBrightPhase3": "True"
}
```

<h1 align="center">Rendering API</h1>

### Metal
###### MacOS Only
```json
{
		"FFlagDebugGraphicsPreferMetal": "True"
}
```
### Vulkan
```json
{
		"FFlagDebugGraphicsDisableDirect3D11": "True",
		"FFlagDebugGraphicsPreferVulkan": "True"
}
```
### OpenGL
```json
{
		"FFlagDebugGraphicsDisableDirect3D11": "True",
		"FFlagDebugGraphicsPreferOpenGL": "True"
}
```
### Direct X 10
```json
{
		"FFlagDebugGraphicsPreferD3D11FL10": "True"
}
```
### Direct X 11
```json
{
		"FFlagDebugGraphicsPreferD3D11": "True"
}
```

<h1 align="center">Graphical Settings <sup>& other stuff</sup></h1>

### Draws a circle under avatars
```json
{
		"FFlagDebugAvatarChatVisualization": "True",
		"FFlagEnableInGameMenuChromeABTest2": "False"
}
```
### HyperThreading
```json
{
		"FFlagDebugCheckRenderThreading": "True",
		"FFlagRenderDebugCheckThreading2": "True"
}
```
### Maximum Threads
```json
{
		"FIntRuntimeMaxNumOfThreads": "2400"
}
```
### Minimum Threads
```json
{
		"FIntTaskSchedulerThreadMin": "3"
}
```
### Smoother Terrain
```json
{
		"FFlagDebugRenderingSetDeterministic": "True"
}
```
### Graphics Quality Level
```json
{
		"FIntRomarkStartWithGraphicQualityLevel": "1"
}
```
### Low Quallity Terrain Textures
###### 4 for less quality 16, 32, 64 for higher quality
```json
{
		"FIntTerrainArraySliceSize": "4"
}
```
### Disable Shadows
```json
{
		"FIntRenderShadowIntensity": "0"
}
```
### Preserve rendering quality with display setting
```json
{
		"DFFlagDisableDPIScale": "True"
}
```
### Low Graphics Quality w/ Max Render Distance/FRM Quality Levels
###### Explanation: 1-6 Are low graphics, Above 6 are high graphics. Like the 1-21 graphics slider
```json
{
		"DFIntDebugFRMQualityLevelOverride": "1"
}
```

#### ->FRM Levels<-

```
Low

1 = 3
2 = 2
3 = 6

High

4 = 7
5 = 11
6 = 14
7 = 15 
8 = 17
9 = 18
10 = 21
```

### Low Render Distance
###### [FRM](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#-frm-levels-)
```json
{
		"DFIntDebugRestrictGCDistance": "1"
}
```
### Disable Wind
```json
{
		"FFlagGlobalWindRendering": "False",
		"FFlagGlobalWindActivated": "False"
}
```
### Limits light updates
```json
{
		"FIntRenderLocalLightUpdatesMax": "8",
		"FIntRenderLocalLightUpdatesMin": "6"
}
```
### Disables fade in and fade out animation every light update
```json
{
		"FIntRenderLocalLightFadeInMs": "0"
}
```
### Makes avatars shiny 
###### [everything goes black on <3] ***[DFIntDebugFRMQualityLevelOverride is there to set your graphics to 10, You can change it to anything above 3: [Click here to view](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#-frm-levels-) ]***
```json
{
		"DFIntRenderClampRoughnessMax": "-640000000",
		"DFIntDebugFRMQualityLevelOverride": "6"
}
```
### Disable PostFX
```json
{
		"FFlagDisablePostFx": "True"
}
```
### Pause Voxelizer/Disable Baked Shadows
```json
{
		"DFFlagDebugPauseVoxelizer": "True"
}
```
### Gray Sky
###### Only applies to games with the default skybox
```json
{
		"FFlagDebugSkyGray": "True"
}
```
### Disable Player Shadows
```json
{
		"FIntRenderShadowIntensity": "0"
}
```
### Force LOD on Meshes
```json
{
		"DFIntCSGLevelOfDetailSwitchingDistance": "0",
		"DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
		"DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
		"DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```
### Lighting Attenuation
```json
{
		"FFlagNewLightAttenuation": "True"
}
```
### Enable GPULightCulling
###### Combine with [Lighting Attenuation](https://github.com/RobloxFastFlags/FastFlags-Collective?tab=readme-ov-file#lighting-attenuation) for better vision
```json
{
		"FFlagFastGPULightCulling3": "True"
}
```
### Frame Buffer
###### Explnation: 0 makes white screen 1-3 makes other players have laggy movement, 4 is stable has better performance than 10 and less input lag
```json
{
		"DFIntMaxFrameBufferSize": "4"
}
```
### High Quality Textures 
###### *[1-3]*
```json
{
		"DFFlagTextureQualityOverrideEnabled": "True",
		"DFIntTextureQualityOverride": "3"
}
```
### Lower Quality Textures 
###### *[1-3]*
```json
{
		"DFIntPerformanceControlTextureQualityBestUtility": "-1"
}
```
### No avatar textures
```json
{
		"DFIntTextureCompositorActiveJobs": "0"
}
```
### Remove Grass
```json
{
		"FIntFRMMinGrassDistance": "0",
		"FIntFRMMaxGrassDistance": "0",
		"FIntRenderGrassDetailStrands": "0",
		"FIntRenderGrassHeightScaler": "0"
}
```
### Force MSAA 
###### *[0, 1, 2, 4, 8]*
```json
{
		"FIntDebugForceMSAASamples": "4"
}
```
### ShadowMap Bias 
###### ***[Future & ShadowMap]***
```json
{
		"FIntRenderShadowmapBias": "75"
}
```
### Enables Network Debug Tracker menu
##### Instructions: CTRL+F8
```json
{
		"DFFlagDebugEnableInterpolationVisualizer": "True"
}
```
### Humanoid Outline
##### Draws an outline around every part and every humanoid
```json
{
		"DFFlagDebugDrawBroadPhaseAABBs": "True"
}
```
### Buggy ZPlane Camera
```json
{
		"FIntCameraFarZPlane": "1"
}
```
<h1 align="center">User Interface</h1>

### FPS Unlocker in Roblox Menu Settings
```json
{
		"FFlagGameBasicSettingsFramerateCap": "True",
		"DFIntTaskSchedulerTargetFps": "0"
}
```
### GUI Hiding Toggles
```json
{
		"FFlagUserShowGuiHideToggles": "True",
		"GuiHidingApiSupport2": "True"
}
```
### Darker Dark Theme
```json
{
		"FFlagLuaAppUseUIBloxColorPalettes1": "True",
		"FFlagUIBloxUseNewThemeColorPalettes": "True"
}
```
### Subscriptions Page
```json
{
		"FFlagLuaAppDevSubsEnabled": "True"
}
```
### No Transparency V4 Menu **(2023)**
```json
{
		"FStringInGameMenuModernizationStickyBarForcedUserIds": "UserID"
}
```
### Revert Old Report Menu
```json
{
		"FStringReportAbuseMenuRoactForcedUserIds": "null",
		"FFlagEnableReportAbuseMenuRoactABTest2": "False",
		"FFlagEnableReportAbuseMenuRoact2": "False",
		"FFlagEnableReportAbuseMenuLayerOnV3": "False"
}
```
### Custom MicroProfile Scale
```json
{ "DFIntMicroProfilerDpiScaleOverride":  "100" }
```
### Hides gui
```json
{ "FFlagDebugAdornsDisabled":  "True" }
```
### Dont Render UI
```json
{
		"FFlagDebugDontRenderUI": "True"
}
```
### Enable Audio Controller
```json
{
		"FFlagTrackerLodControllerDebugUI": "True"
}
```
### Disable Autocomplete
```json
{
		"FFlagEnableCommandAutocomplete": "False"
}
```
### Chrome UI TopBar
```json
{
		"FFlagEnableInGameMenuChrome": "True",
		"FFlagEnableReportAbuseMenuRoactABTest2": "True",
		"FFlagChromeBetaFeature": "True",
		"FFlagEnableInGameMenuChromeABTest2": "True"
}
```
### Pin Chat on Chrome UI
```json
{ "FFlagEnableChromePinnedChat":  "True" }
```
### Chrome UI Topbar Removal
```json
{
		"FFlagEnableInGameMenuChromeABTest2": "False",
		"FFlagEnableReportAbuseMenuRoactABTest2": "False"
}
```
### Disable Bubble Chat
```json
{ "FFlagEnableBubbleChatFromChatService":  "False" }
```
### Disable Selfview
```json
{ "FFlagCoreGuiTypeSelfViewPresent":  "False" }
```
### Remove VC Beta Badge
```json
{
		"FFlagVoiceBetaBadge": "False",
		"FFlagTopBarUseNewBadge": "False",
		"FFlagEnableBetaBadgeLearnMore": "False",
		"FFlagBetaBadgeLearnMoreLinkFormview": "False",
		"FFlagControlBetaBadgeWithGuac": "False",
		"FStringVoiceBetaBadgeLearnMoreLink": "null"
}
```
### Hide guis
###### ***Instructions: Replace "ID" with any group ID that you are in.***
| Key combination   | Action                                                                    |
| ----------------- | ------------------------------------------------------------------------- |
| Ctrl + Shift + B  | Toggles GUIs in 3D space (BillboardGuis, SurfaceGuis, etc)                |
| Ctrl + Shift + C  | Toggles game-defined ScreenGuis                                           |
| Ctrl + Shift + G  | Toggles Roblox CoreGuis                                                   |
| Ctrl + Shift + N  | Toggles player names, and other BillboardGuis that show up above a player |
```json
{
		"DFIntCanHideGuiGroupId": "ID"
}
```
### Disable Fullscreen Title Bar
```json
{
		"FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### Set Custom Font Size
```json
{
		"FIntFontSizePadding": "1"
}
```

<h1 align="center">Textures</h1>

### Fix Textures
```json
{
		"FFlagMSRefactor5": "False"
}
```
### No Textures
```json
{
		"FStringPartTexturePackTable2022": "{\"glass\":{\"ids\":[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\"color\":[254,254,254,7]}}",
		"FStringPartTexturePackTablePre2022": "{\"glass\":{\"ids\":[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\"color\":[254,254,254,7]}}",
		"FStringTerrainMaterialTable2022": "",
		"FStringTerrainMaterialTablePre2022": "",
		"FFlagMSRefactor5": "False"
}
```
<h1 align="center">Physics</h1>

### Remap R6 to R15 Rigs
```json
{
		"FFlagRemapAnimationR6ToR15Rig": "True"
}
```
### Disables PGS Solver
###### Projected Gauss-Seidel physics, or PGS physics, is a more reliable but more costly physics solver released in summer of 2015. The solver has a lot less "give" than spring physics, in terms of parts won't want to go into each other at all, making joints less flexible. This allows for parts to have less of a tendency to go through each other. As of October 21, 2015, the joints called glue joints are supported in the system, and will not break under pressure. The solver takes more processing power to work over spring physics, which will cause games to act slower. This solver runs at 240 Hz.
```json
{
		"FFlagSimDefaultPGSSolver": "False"
}
```
### Adjust Hip Height Clamps
###### https://www.roblox.com/bundles/63/Mage-Animation-Package
```json
{
		"DFIntHipHeightClamp": "-48"
}
```
### Random High Jumps
###### https://youtu.be/2JkA4hWCAWw
```json
{
		"FFlagSimAdaptiveTimesteppingDefault2": "True",
		"DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### Drunk
```json
{
		"FFlagSimAdaptiveTimesteppingDefault2": "True",
		"DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
		"DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### No Animations
```json
{
		"DFIntReplicatorAnimationTrackLimitPerAnimator": "-1"
}
```
### Stick unanchored parts to you
##### - = up, + = down
```json
{
		"DFIntSolidFloorPercentForceApplication": "-1000",
		"DFIntNonSolidFloorPercentForceApplication": "-5000"
}
```
### Max Raycast Distance
###### Raycasting is the use of intersection tests to solve problems in ROBLOX. The most common use of raycasting is to determine the first object intersected by a ray. This is done by casting a virtual ray from a certain point in a direction and determining the first surface it intersected with.
###### Break legs collision from 2 to -inf, kinda break camera on values over 3 noclip cam on 3
```json
{
		"DFIntRaycastMaxDistance": "3"
}
```
### Possible Super Jump
```json
{
		"DFIntNewRunningBaseGravityReductionFactorHundredth": "1500"
}
```
### Change DataSender Rate
###### a.k.a dos not let you load games
```json
{
		"DFIntDataSenderRate": "-1"
}
```
### Disable Touch Events
```json
{
		"DFIntTouchSenderMaxBandwidthBps": "-1"
}
```
### Fake Lag
```json
{
		"DFIntS2PhysicsSenderRate": "1"
}
```
### Invisible 1
```json
{
		"DFIntS2PhysicsSenderRate": "30"
}
```
### Invisible 2
###### Locks your character's position on the server to (0, 0, 0), having the side effect of turning you invisible. This only affects the server and other clients, not you. server-sided things that rely on your position, like clicking to get tools, will not function. In some games these can be abusable. Here is a list of them: [Link](https://docs.google.com/document/d/1_kQr-tkc97lcg7ZvFfJdt8UzaziIfwuJPrzR6sTOLHo/)
```json
{
		"DFIntGameNetPVHeaderTranslationZeroCutoffExponent": "10"
}
```
### Invisible 3
###### Restricts the client from sending any physics-related information. This means other people can topple you over.
```json
{
		"DFIntPhysicsSenderMaxBandwidthBps": "1",
		"DFIntPhysicsSenderMaxBandwidthBpsScaling": "0"
}
```
### Clientsided Invisible
```json
{
		"FIntParallelDynamicPartsFastClusterBatchSize": "-1",
}
```
### Warp & Slowmotion
```json
{
		"DFIntMaxMissedWorldStepsRemembered": "1"
}
```
```json
{
		"DFIntMaxMissedWorldStepsRemembered": "1000"
}
```
### Noclip
###### adjust the value so u dont fall through the ground
```json
{
		"DFFlagAssemblyExtentsExpansionStudHundredth": "-50"
}
```
### Hip Height
###### Very controllable bounce, only works with negative values, 0 allows you to hover
```json
{
		"DFIntMaxAltitudePDStickHipHeightPercent": "-200"
}
```
### Wallglide
```json
{
		"DFIntUnstickForceAttackInTenths": "-4"
}
```

<h1 align="center">other fflags</h1>

### Disable In-game Advertisements
```json
{
		"FFlagAdServiceEnabled": "False"
}
```
### Disable Telemetry 
```json
{
		"FFlagDebugDisableTelemetryEphemeralCounter": "True",
		"FFlagDebugDisableTelemetryEphemeralStat": "True",
		"FFlagDebugDisableTelemetryEventIngest": "True",
		"FFlagDebugDisableTelemetryPoint": "True",
		"FFlagDebugDisableTelemetryV2Counter": "True",
		"FFlagDebugDisableTelemetryV2Event": "True",
		"FFlagDebugDisableTelemetryV2Stat": "True"
}
```
### Adjust Scroll Speed
```json
{ "FIntScrollWheelDeltaAmount": "140" }
```
### Surf the web inside of Roblox
###### Click the Beta badge or the 13+ badge to open the webview browser.
```json
{
		"FFlagTopBarUseNewBadge": "True",
		"FStringTopBarBadgeLearnMoreLink": "https://google.com/",
		"FStringVoiceBetaBadgeLearnMoreLink": "https://google.com/"
}
```
### Sounds use physical velocity and become distorted
###### <2017
```json
{
		"FFlagSoundsUsePhysicalVelocity": "True"
}
```
### Shows the state of a flag
```json
{
		"FStringDebugShowFlagState": "FLAG_HERE"
}
```
###### e.g
```json
{
		"FStringDebugShowFlagState": "DFIntTaskSchedulerTargetFps, ChannelName"
}
```
### MTU 
```json
{
		"DFIntConnectionMTUSize": "MTU_HERE"
}
```
### Increase Ping 
```json
{
		"DFIntDataSenderMaxBandwidthBps": "150"
}
```
### No Internet Disconnect 
###### *[You will still be kicked but the message wont show.]*
```json
{
		"DFFlagDebugDisableTimeoutDisconnect": "True"
}
```
### Quick Game Launch 
###### *[BUGGY]*
```json
{
		"FFlagEnableQuickGameLaunch": "True"
}
```
### Allows you to change voice chat distance 
###### default: [Min 7 Max 80]
```json
{
		"DFIntVoiceChatRollOffMinDistance": "7",
		"DFIntVoiceChatRollOffMaxDistance": "80"
}
```
### Disable In-Game Purchases
```json
{
		"DFFlagOrder66": "True"
}
```
### Disable Chat
```json
{
		"FFlagDebugForceChatDisabled": "True"
}
```
### Limit audios that are being played
```json
{
		"DFIntMaxLoadableAudioChannelCount": "1"
}
```
### Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's a non-functioning UI too. Also adds a blue circle to your humanoid.
```json
{
		"FFlagDebugHumanoidRendering": "True"
}
```
### Custom Disconnect Message
```json
{
		"FFlagReconnectDisabled": "True",
		"FStringReconnectDisabledReason": "You're stupid and I hate you"
}
```
### Display FPS
```json
{
		"FFlagDebugDisplayFPS": "True"
}
```
### Verified Badge
###### Clientsided
```json
{
		"FStringWhitelistVerifiedUserId": "UserID"
}
```
### Verified Badge on everyone
###### Clientsided
```json
{
		"FFlagOverridePlayerVerifiedBadge": "True"
}
```
### Applies cool colors to stuff
```json
{
		"FFlagDebugDisplayUnthemedInstances": "True"
}
```
### Show Outlined Chunks
```json
{
		"FFlagDebugLightGridShowChunks": "True"
}
```
### Remove Disconnect Blur/Loading Blur
```json
{
		"FIntRobloxGuiBlurIntensity": "0"
}
```
### Disable Dynamic Heads Animations
###### https://roblox.fandom.com/wiki/Dynamic_Head
```json
{
		"DFIntAnimationLodFacsDistanceMin": "0",
		"DFIntAnimationLodFacsDistanceMax": "0",
		"DFIntAnimationLodFacsVisibilityDenominator": "0"
}
```
### failsafehumanoid
###### gray avatars
```json
{
		"FFlagFailsafeHumanoid_3": "True"
}
```
### Automatically unmutes your mic on join (VC)
```json
{
		"FFlagDebugDefaultChannelStartMuted": "False"
}
```
### Overlay that shows what you type 
```json
{
		"FFlagDebugTextBoxServiceShowOverlay": "True"
}
```
### opt-out Experience Language
###### Removes the Experience Language option in settings
```json
{
		"FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Disable New Chat Translation Settings
```json
{
		"FFlagChatTranslationSettingEnabled3 ": "False"
}
```
### Lets you change the zoom out limit
###### Only applies to games that has not changed the default zoom limit
```json
{
		"FIntCameraMaxZoomDistance": "9999"
}
```
### Limits number of animations being played
```json
{
		"DFIntMaxActiveAnimationTracks": "0"
}
```
### Prevents Remote Events from running
```json
{
		"DFIntRemoteEventSingleInvocationSizeLimit": "1"
}
```
### Mess with voice chat volume
###### default 1000
```json
{
		"DFIntVoiceChatVolumeThousandths": "100000"
}
```
### Removes the head roll limit for face tracking
```json
{
		"DFIntAvatarFaceChatHeadRollLimitDegrees": "360"
}
```
### VR Controller transparency
```json
{
		"FIntVRTouchControllerTransparency": "0"
}
```
### No sounds
```json
{
		"FFlagDebugRomarkMockingAudioDevices": "True"
}
```
### local rcc
[?](https://github.com/rsblox/local_rcc)
```json
{
		"FFlagDebugLocalRccServerConnection": "True",
		"FFlagRefactorPlayerConnect": "False"
}
```
### Exclusive Fullscreen
```json
{
		"FFlagHandleAltEnterFullscreenManually": "False"
}
```


<h1 align="center">Links</h1>

### [Make Your Own Custom Roblox Textures](https://github.com/GoingCrazyDude/roblox-custom-textures/blob/main/README.md) *[Github Repo Link]*
### [Bloxstrap](https://github.com/pizzaboxer/bloxstrap) *[Github Repo Link]*
### [NVIDIA Shaders Guide](https://github.com/catb0x/Roblox-Shaders-Guide) *[Github Repo Link]*
### [EnableAnselForRoblox](https://github.com/DED0026/EnableAnselForRoblox) *[Github Repo Link]*
### [potato fflags](https://github.com/catb0x/Roblox-Potato-FFlags) *[Github Repo Link]*
### ~~RCOOL~~ We couldn't save this one.
### [Roblox Channel Checker](https://cdn.discordapp.com/attachments/1225631712285823059/1228285379518529567/rct_source.7z?ex=662b7ce6&is=661907e6&hm=32091b6b6c30a4d700303d6b1ae79cae8db0dedb80682e627cd7cca03aaa25c9&) *[Download Link]*
### [Bindable Lag Switch](https://github.com/Hermivore8151/Bindable-LagSwitch) *[Github Repo Link]*
### [MEGA FLAG LIST](https://discord.com/channels/1099468797410283540/1139962301991104582/1170417533355036712) *[Bloxstrap Server]*

###### -> ‧⁺̣˚̣̣*̣̩⋆̩·̩̩୨˚̣̣̣̣͙୧·̩̩⋆̩*̣̩˚̣̣⁺̣‧ You've reached the bottom of the list! ‧⁺̣˚̣̣*̣̩⋆̩·̩̩୨˚̣̣̣̣͙୧·̩̩⋆̩*̣̩˚̣̣⁺̣‧୨ <-

# List Information
* Version: 8.6.3 [4/12/2024]
* **121 Currently Listed**
* Creation Date: 9:46 PM 08/25/2023 
* Rentry Publish Date: 12/09/2023

[.](https://open.spotify.com/track/4uhvMW7ly7tJil31YYscAN)

##### -> FastFlags 2024®eal <-

-> [FVariables.txt](https://raw.githubusercontent.com/MaximumADHD/Roblox-Client-Tracker/roblox/FVariables.txt) <-

-> [Roblox FFlag Tracker](https://github.com/MaximumADHD/Roblox-FFlag-Tracker) <-
