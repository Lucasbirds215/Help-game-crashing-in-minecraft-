# Help-game-crashing-in-minecraft-
My Game is crashing becuase when i put something in the ranged tab of custom npcs it gives me a blue screen
this is th crash report 


---- Minecraft Crash Report ----

WARNING: coremods are present:
  Techguns Core (techguns-1.12.2-2.0.2.0_pre3.2.jar)
  MalisisCorePlugin (malisiscore-1.12.2-6.5.1.jar)
  ObfuscatePlugin (obfuscate-0.4.2-1.12.2.jar)
Contact their authors BEFORE contacting forge

// I bet Cylons wouldn't have this problem.

Time: 7/1/21 4:33 PM
Description: Rendering entity in world

java.lang.NullPointerException: Rendering entity in world
	at techguns.client.render.ItemRenderHack.shouldRenderItem(ItemRenderHack.java:124)
	at techguns.client.render.ItemRenderHack.renderItem(ItemRenderHack.java:54)
	at net.minecraft.client.renderer.RenderItem.func_181564_a(RenderItem.java:384)
	at codechicken.lib.render.item.CCRenderItem.func_181564_a(CCRenderItem.java:293)
	at noppes.npcs.client.renderer.RenderProjectile.doRenderProjectile(RenderProjectile.java:124)
	at noppes.npcs.client.renderer.RenderProjectile.func_76986_a(RenderProjectile.java:145)
	at net.minecraft.client.renderer.entity.RenderManager.func_188391_a(RenderManager.java:412)
	at net.minecraft.client.renderer.entity.RenderManager.func_188388_a(RenderManager.java:392)
	at net.minecraft.client.renderer.RenderGlobal.func_180446_a(RenderGlobal.java:839)
	at net.minecraft.client.renderer.EntityRenderer.func_175068_a(EntityRenderer.java:1800)
	at net.minecraft.client.renderer.EntityRenderer.func_78471_a(EntityRenderer.java:1613)
	at net.minecraft.client.renderer.EntityRenderer.func_181560_a(EntityRenderer.java:1384)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:1119)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:398)
	at net.minecraft.client.main.Main.main(SourceFile:123)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Client thread
Stacktrace:
	at techguns.client.render.ItemRenderHack.shouldRenderItem(ItemRenderHack.java:124)
	at techguns.client.render.ItemRenderHack.renderItem(ItemRenderHack.java:54)
	at net.minecraft.client.renderer.RenderItem.func_181564_a(RenderItem.java:384)
	at codechicken.lib.render.item.CCRenderItem.func_181564_a(CCRenderItem.java:293)
	at noppes.npcs.client.renderer.RenderProjectile.doRenderProjectile(RenderProjectile.java:124)
	at noppes.npcs.client.renderer.RenderProjectile.func_76986_a(RenderProjectile.java:145)

-- Entity being rendered --
Details:
	Entity Type: customnpcs:customnpcprojectile (noppes.npcs.entity.EntityProjectile)
	Entity ID: 416
	Entity Name: entity.CustomNpcProjectile.name
	Entity's Exact location: -90.53, 89.52, -19.81
	Entity's Block location: World: (-91,89,-20), Chunk: (at 5,5,12 in -6,-2; contains blocks -96,0,-32 to -81,255,-17), Region: (-1,-1; contains chunks -32,-32 to -1,-1, blocks -512,0,-512 to -1,255,-1)
	Entity's Momentum: -0.09, -0.15, 0.97
	Entity's Passengers: []
	Entity's Vehicle: ~~ERROR~~ NullPointerException: null

-- Renderer details --
Details:
	Assigned renderer: noppes.npcs.client.renderer.RenderProjectile@58d74cdd
	Location: 0.32,1.52,-3.15 - World: (0,1,-4), Chunk: (at 0,0,12 in 0,-1; contains blocks 0,0,-16 to 15,255,-1), Region: (0,-1; contains chunks 0,-32 to 31,-1, blocks 0,0,-512 to 511,255,-1)
	Rotation: -5.456909
	Delta: 0.47999254
Stacktrace:
	at net.minecraft.client.renderer.entity.RenderManager.func_188391_a(RenderManager.java:412)
	at net.minecraft.client.renderer.entity.RenderManager.func_188388_a(RenderManager.java:392)
	at net.minecraft.client.renderer.RenderGlobal.func_180446_a(RenderGlobal.java:839)
	at net.minecraft.client.renderer.EntityRenderer.func_175068_a(EntityRenderer.java:1800)
	at net.minecraft.client.renderer.EntityRenderer.func_78471_a(EntityRenderer.java:1613)

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityPlayerSP['Lucasbirds215XD'/150, l='MpServer', x=-90.84, y=88.00, z=-16.67]]
	Chunk stats: MultiplayerChunkCache: 289, 289
	Level seed: 0
	Level generator: ID 00 - default, ver 1. Features enabled: false
	Level generator options: 
	Level spawn location: World: (-108,88,-159), Chunk: (at 4,5,1 in -7,-10; contains blocks -112,0,-160 to -97,255,-145), Region: (-1,-1; contains chunks -32,-32 to -1,-1, blocks -512,0,-512 to -1,255,-1)
	Level time: 2609941 game time, 1000 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
	Forced entities: 98 total; [EntitySportsPlane['Sports Plane'/17, l='MpServer', x=-153.50, y=94.00, z=44.34], EntityOldMan['The Old Man (106)'/19, l='MpServer', x=-139.25, y=85.00, z=18.60], EntityOfficeChair['entity.chair.name'/23, l='MpServer', x=-112.50, y=83.00, z=-59.50], EntityCustom['Male Researcher'/24, l='MpServer', x=-117.25, y=83.00, z=-58.97], EntityCustom['Male Guard'/25, l='MpServer', x=-115.70, y=83.00, z=-64.45], EntityOfficeChair['entity.chair.name'/27, l='MpServer', x=-114.50, y=92.00, z=-27.50], EntityCustom['Male Researcher'/28, l='MpServer', x=-114.97, y=92.00, z=-22.17], EntityCustom['Male Researcher'/29, l='MpServer', x=-116.87, y=92.00, z=-21.86], EntitySculpture['The Sculpture (173)'/30, l='MpServer', x=-119.51, y=89.00, z=-21.70], EntityLabel['entity.label.name'/31, l='MpServer', x=-110.50, y=90.00, z=-21.50], EntityLabel['entity.label.name'/32, l='MpServer', x=-104.50, y=90.00, z=-22.50], EntityPlayerSP['Lucasbirds215XD'/150, l='MpServer', x=-90.84, y=88.00, z=-16.67], EntityCustom['Mobile Task Force Omega-7 "Pandora's Box"'/33, l='MpServer', x=-98.72, y=88.00, z=-26.50], EntityCustom['Mobile Task Force Beta-7 "Maz Hatters" [melee unit]'/34, l='MpServer', x=-108.33, y=86.00, z=-24.05], EntityEyePod['Eye Pod (131)'/35, l='MpServer', x=-98.59, y=88.00, z=-19.38], EntityCustom['Female Guard'/36, l='MpServer', x=-108.50, y=89.00, z=-25.29], EntityCustom['Male Guard'/37, l='MpServer', x=-102.47, y=89.00, z=-24.26], EntityCustom['Male Guard'/38, l='MpServer', x=-106.45, y=89.00, z=-25.19], EntityCustom['Male Guard'/39, l='MpServer', x=-94.69, y=88.00, z=-22.50], EntityLabel['entity.label.name'/43, l='MpServer', x=-108.50, y=84.00, z=-74.50], EntityLabel['entity.label.name'/44, l='MpServer', x=-110.50, y=84.00, z=-70.50], EntityLabel['entity.label.name'/45, l='MpServer', x=-108.50, y=84.00, z=-68.50], EntityOldMan['The Old Man (106)'/46, l='MpServer', x=-100.51, y=77.00, z=-52.29], EntityLabel['entity.label.name'/47, l='MpServer', x=-110.50, y=84.00, z=-62.50], EntityLabel['entity.label.name'/48, l='MpServer', x=-110.50, y=84.00, z=-54.50], EntityLabel['entity.label.name'/49, l='MpServer', x=-108.50, y=84.00, z=-60.50], EntityLabel['entity.label.name'/50, l='MpServer', x=-108.50, y=84.00, z=-53.50], EntityLabel['entity.label.name'/51, l='MpServer', x=-110.50, y=84.00, z=-48.50], EntityCustom['Male Guard'/52, l='MpServer', x=-108.51, y=83.00, z=-61.29], EntityCustom['Male Guard'/53, l='MpServer', x=-109.07, y=83.00, z=-74.70], EntityCustom['Female Guard'/54, l='MpServer', x=-108.42, y=83.00, z=-74.18], EntityOfficeChair['entity.chair.name'/55, l='MpServer', x=-96.50, y=93.00, z=-12.50], EntityOfficeChair['entity.chair.name'/56, l='MpServer', x=-102.50, y=88.00, z=-1.50], EntityOfficeChair['entity.chair.name'/57, l='MpServer', x=-96.50, y=93.00, z=-15.50], EntityCustom['Male Researcher'/58, l='MpServer', x=-98.76, y=93.00, z=-4.21], EntityEyePod['Eye Pod (131)'/59, l='MpServer', x=-100.50, y=91.55, z=-13.76], EntityCustom['Male Guard'/60, l='MpServer', x=-97.70, y=94.00, z=-14.50], EntityCustom['Male Guard'/61, l='MpServer', x=-95.71, y=88.00, z=0.76], EntityLabel['entity.label.name'/62, l='MpServer', x=-83.50, y=89.00, z=-2.50], EntityLabel['entity.label.name'/63, l='MpServer', x=-84.50, y=94.00, z=-2.50], EntityOfficeChair['entity.chair.name'/64, l='MpServer', x=-82.50, y=88.00, z=-8.50], EntityCustom['Male Guard'/65, l='MpServer', x=-87.70, y=88.00, z=-11.70], EntityCustom['Male Researcher'/66, l='MpServer', x=-92.79, y=93.00, z=-14.65], EntityCustom['Male Guard'/69, l='MpServer', x=-93.46, y=93.00, z=1.77], EntityCustom['Female Guard'/70, l='MpServer', x=-93.70, y=88.00, z=-19.70], EntityCustom['Male Guard'/71, l='MpServer', x=-85.22, y=88.00, z=-13.52], EntityCustom['Male Guard'/72, l='MpServer', x=-93.66, y=93.00, z=4.25], EntityOfficeChair['entity.chair.name'/73, l='MpServer', x=-99.50, y=88.00, z=3.50], EntityOfficeChair['entity.chair.name'/76, l='MpServer', x=-88.50, y=89.00, z=-33.50], EntityOfficeChair['entity.chair.name'/77, l='MpServer', x=-93.50, y=89.00, z=-35.50], EntityToilet['entity.toilet.name'/78, l='MpServer', x=-95.50, y=89.00, z=-39.50], EntityCustom['Male Researcher'/79, l='MpServer', x=-88.50, y=89.00, z=-35.50], EntityYoungGirl['Young Girl (053)'/80, l='MpServer', x=-91.68, y=89.00, z=-29.83], EntityLabel['entity.label.name'/81, l='MpServer', x=-93.50, y=89.00, z=-16.50], EntityLabel['entity.label.name'/82, l='MpServer', x=-82.50, y=90.00, z=-23.50], EntityLabel['entity.label.name'/83, l='MpServer', x=-89.50, y=90.00, z=-30.50], EntityLabel['entity.label.name'/84, l='MpServer', x=-88.50, y=89.00, z=-24.50], EntityLabel['entity.label.name'/85, l='MpServer', x=-80.50, y=95.00, z=-23.50], EntityCustom['Female Guard'/86, l='MpServer', x=-93.29, y=88.00, z=-24.44], EntitySimpleChair['entity.simpleChair.name'/87, l='MpServer', x=-87.50, y=88.00, z=0.50], EntitySimpleChair['entity.simpleChair.name'/88, l='MpServer', x=-87.50, y=88.00, z=8.50], EntitySimpleChair['entity.simpleChair.name'/89, l='MpServer', x=-93.50, y=88.00, z=6.50], EntitySimpleChair['entity.simpleChair.name'/90, l='MpServer', x=-87.50, y=88.00, z=6.50], EntitySimpleChair['entity.simpleChair.name'/91, l='MpServer', x=-93.50, y=88.00, z=8.50], EntityCustom['Male Researcher'/92, l='MpServer', x=-84.18, y=88.00, z=5.32], EntityCustom['Male Researcher'/93, l='MpServer', x=-86.50, y=93.00, z=1.50], EntityCustom['Male Guard'/94, l='MpServer', x=-93.42, y=88.00, z=2.77], EntityCustom['Tickle Monster (999)'/95, l='MpServer', x=-88.30, y=88.00, z=8.50], EntityPinkFlamingo['Pink Flamingo (1507)'/96, l='MpServer', x=-82.51, y=93.00, z=-0.26], EntityCustom['Male Guard'/97, l='MpServer', x=-95.24, y=92.00, z=33.51], EntityShyGuy['Shy Guy (096)'/99, l='MpServer', x=-76.51, y=96.00, z=-70.56], EntityLabel['entity.label.name'/100, l='MpServer', x=-78.50, y=96.00, z=-61.50], EntityOldMan['The Old Man (106)'/101, l='MpServer', x=-74.29, y=91.00, z=-44.49], EntityOfficeChair['entity.chair.name'/102, l='MpServer', x=-78.50, y=89.00, z=-22.50], EntityLabel['entity.label.name'/103, l='MpServer', x=-70.50, y=95.00, z=-20.50], EntityLabel['entity.label.name'/104, l='MpServer', x=-75.50, y=95.00, z=-23.50], EntityLabel['entity.label.name'/105, l='MpServer', x=-77.50, y=95.00, z=-16.50], EntityPlagueDoctor['Plague Doctor (049)'/106, l='MpServer', x=-70.58, y=89.00, z=-16.69], EntityCustom['Male Researcher'/107, l='MpServer', x=-79.30, y=89.00, z=-22.70], EntityLabel['entity.label.name'/108, l='MpServer', x=-77.50, y=90.00, z=-16.50], EntityCustom['MTF Epsilon-9 "Fire Eaters" Agent'/109, l='MpServer', x=-70.41, y=94.00, z=-23.70], EntityCustom['Male Guard'/110, l='MpServer', x=-75.47, y=94.00, z=-23.22], EntityCustom['Male Guard'/111, l='MpServer', x=-70.54, y=94.00, z=-23.01], EntityCustom['Female Guard'/112, l='MpServer', x=-80.70, y=94.00, z=-23.11], EntityInvisibleChair['entity.invisibleChair.name'/113, l='MpServer', x=-68.50, y=87.50, z=-10.50], EntityCustomNpc['main doctor'/114, l='MpServer', x=-67.50, y=88.63, z=-10.50], EntityCustomNpc['Guard  '/115, l='MpServer', x=-72.50, y=88.50, z=-4.50], EntitySportsPlane['Sports Plane'/121, l='MpServer', x=-79.53, y=88.00, z=17.18], EntityOldMan['The Old Man (106)'/122, l='MpServer', x=-57.50, y=94.00, z=-16.50], EntityCustom['MTF Epsilon-9 "Fire Eaters" Agent'/123, l='MpServer', x=-62.45, y=100.00, z=-22.72], EntityCustom['Male Guard'/124, l='MpServer', x=-40.61, y=91.19, z=-6.86], EntityATV['ATV'/151, l='MpServer', x=-174.50, y=92.00, z=62.50], EntitySportsPlane['Sports Plane'/152, l='MpServer', x=-183.50, y=95.00, z=74.47], EntitySmartCar['Smart Car'/153, l='MpServer', x=-174.36, y=92.00, z=64.38], EntitySportsPlane['Sports Plane'/154, l='MpServer', x=-156.50, y=84.00, z=94.55], EntityCustomNpc['Miyama Kyōichirō'/410, l='MpServer', x=-90.37, y=88.00, z=-20.05], EntityPlayerSP['Lucasbirds215XD'/150, l='MpServer', x=-82.37, y=88.00, z=-11.26], EntityProjectile['entity.CustomNpcProjectile.name'/416, l='MpServer', x=-90.53, y=89.52, z=-19.81]]
	Retry entities: 0 total; []
	Server brand: fml,forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:532)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2741)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:419)
	at net.minecraft.client.main.Main.main(SourceFile:123)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.12.2
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 679138488 bytes (647 MB) / 2147483648 bytes (2048 MB) up to 2147483648 bytes (2048 MB)
	JVM Flags: 8 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	IntCache: cache: 0, tcache: 0, allocated: 12, tallocated: 94
	FML: MCP 9.42 Powered by Forge 14.23.5.2854 Optifine OptiFine_1.12.2_HD_U_E3 38 mods loaded, 38 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored

	| State  | ID                      | Version               | Source                                               | Signature                                |
	|:------ |:----------------------- |:--------------------- |:---------------------------------------------------- |:---------------------------------------- |
	| LCHIJA | minecraft               | 1.12.2                | minecraft.jar                                        | None                                     |
	| LCHIJA | mcp                     | 9.42                  | minecraft.jar                                        | None                                     |
	| LCHIJA | FML                     | 8.0.99.99             | forge-1.12.2-14.23.5.2854.jar                        | e3c3d50c7c986df74c645c0ac54639741c90a557 |
	| LCHIJA | forge                   | 14.23.5.2854          | forge-1.12.2-14.23.5.2854.jar                        | e3c3d50c7c986df74c645c0ac54639741c90a557 |
	| LCHIJA | obfuscate               | 0.4.2                 | minecraft.jar                                        | None                                     |
	| LCHIJA | techguns_core           | 1.12.2-1.0            | minecraft.jar                                        | None                                     |
	| LCHIJA | securitycraft           | v1.8.7                | [1.12.x]+SecurityCraft+v1.8.7.jar                    | None                                     |
	| LCHIJA | carryon                 | 1.12.3                | CarryOn+MC1.12.2+v1.12.3.jar                         | 55e88f24d04398481ae6f1ce76f65fd776f14227 |
	| LCHIJA | chiselsandbits          | 14.33                 | chiselsandbits-14.33.jar                             | None                                     |
	| LCHIJA | codechickenlib          | 3.2.3.358             | CodeChickenLib-1.12.2-3.2.3.358-universal.jar        | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
	| LCHIJA | scpcustomsounds         | 1.0.0                 | Cor3s.jar                                            | None                                     |
	| LCHIJA | modcurrency             | 1.12-1.3.11           | Currency-1.12.0-1.3.11.jar                           | None                                     |
	| LCHIJA | customnpcs              | 1.12                  | CustomNPCs_1.12.2-(05Jul20).jar                      | None                                     |
	| LCHIJA | cdm                     | 0.4.1                 | device-mod-0.4.1-1.12.2.jar                          | None                                     |
	| LCHIJA | forgemultipartcbe       | 2.5.0.71              | ForgeMultipart-1.12.2-2.5.0.71-universal.jar         | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
	| LCHIJA | microblockcbe           | 2.5.0.71              | ForgeMultipart-1.12.2-2.5.0.71-universal.jar         | None                                     |
	| LCHIJA | minecraftmultipartcbe   | 2.5.0.71              | ForgeMultipart-1.12.2-2.5.0.71-universal.jar         | None                                     |
	| LCHIJA | cfm                     | 6.3.1                 | furniture-6.3.1-1.12.2 (1).jar                       | None                                     |
	| LCHIJA | gitwebbuilder           | 1.1                   | GitWeb+Builder-1.1.jar                               | None                                     |
	| LCHIJA | scp_lockdown_staff      | 1.0.0                 | H2Os+SCPs+1.8.3+Secure+and+Contain+update+part+1.jar | None                                     |
	| LCHIJA | malisiscore             | 1.12.2-6.5.1-SNAPSHOT | malisiscore-1.12.2-6.5.1.jar                         | None                                     |
	| LCHIJA | malisisdoors            | 1.12.2-7.3.0          | malisisdoors-1.12.2-7.3.0.jar                        | None                                     |
	| LCHIJA | mrtjpcore               | 2.1.3.35              | MrTJPCore-1.12.2-2.1.3.35-universal.jar              | None                                     |
	| LCHIJA | nifty                   | 1.21                  | NiftyBlocks-1.21.jar                                 | None                                     |
	| LCHIJA | projectred-core         | 4.9.1.92              | ProjectRed-1.12.2-4.9.1.92-Base.jar                  | None                                     |
	| LCHIJA | projectred-integration  | 4.9.1.92              | ProjectRed-1.12.2-4.9.1.92-integration.jar           | None                                     |
	| LCHIJA | projectred-transmission | 4.9.1.92              | ProjectRed-1.12.2-4.9.1.92-integration.jar           | None                                     |
	| LCHIJA | projectred-illumination | 4.9.1.92              | ProjectRed-1.12.2-4.9.1.92-lighting.jar              | None                                     |
	| LCHIJA | scootys_scp_mod         | 1.5                   | SCP+Lockdown+Heavy+Expansion+1.5.jar                 | None                                     |
	| LCHIJA | scp                     | 2.3.1                 | SCP+Lockdown-1.12.2-2.3.1-dev.jar                    | None                                     |
	| LCHIJA | area_79_extras          | 1.0.0                 | SCP-XK-Scenario-Version-1.1.0.jar                    | None                                     |
	| LCHIJA | scpua                   | 1.7.7                 | SCPL-xk-unity-1.7.7.jar                              | None                                     |
	| LCHIJA | techguns                | 2.0.2.0               | techguns-1.12.2-2.0.2.0_pre3.2.jar                   | None                                     |
	| LCHIJA | vehicle                 | 0.44.1                | vehicle-mod-0.44.1-1.12.2.jar                        | None                                     |
	| LCHIJA | worldedit               | 6.1.8                 | worldedit-forge-mc1.12-6.1.8-dist (1).jar            | None                                     |
	| LCHIJA | wrcbe                   | 2.3.2                 | WR-CBE-1.12.2-2.3.2.33-universal (1).jar             | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
	| LCHIJA | zerascp                 | 1.0.0                 | zeras-SCPs-1.7.1.jar                                 | None                                     |
	| LCHIJA | mysticallib             | 1.12.2-1.9.0          | mysticallib-1.12.2-1.9.0.jar                         | None                                     |

	Loaded coremods (and transformers): 
Techguns Core (techguns-1.12.2-2.0.2.0_pre3.2.jar)
  techguns.core.TechgunsASMTransformer
MalisisCorePlugin (malisiscore-1.12.2-6.5.1.jar)
  
ObfuscatePlugin (obfuscate-0.4.2-1.12.2.jar)
  com.mrcrayfish.obfuscate.asm.ObfuscateTransformer
	GL info: ' Vendor: 'ATI Technologies Inc.' Version: '4.6.13587 Compatibility Profile Context 19.40.48 26.20.14048.2' Renderer: 'AMD Radeon(TM) Vega 8 Graphics'
	Launched Version: 1.12.2-forge-14.23.5.2854
	LWJGL: 2.9.4
	OpenGL: AMD Radeon(TM) Vega 8 Graphics GL version 4.6.13587 Compatibility Profile Context 19.40.48 26.20.14048.2, ATI Technologies Inc.
	GL Caps: Using GL 1.3 multitexturing.
Using GL 1.3 texture combiners.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Shaders are available because OpenGL 2.1 is supported.
VBOs are available because OpenGL 1.5 is supported.

	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: 
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	CPU: 8x AMD Ryzen 5 3500U with Radeon Vega Mobile Gfx 
	OptiFine Version: OptiFine_1.12.2_HD_U_E3
	OptiFine Build: 20181210-121000
	Render Distance Chunks: 8
	Mipmaps: 4
	Anisotropic Filtering: 1
	Antialiasing: 0
	Multitexture: false
	Shaders: null
	OpenGlVersion: 4.6.13587 Compatibility Profile Context 19.40.48 26.20.14048.2
	OpenGlRenderer: AMD Radeon(TM) Vega 8 Graphics
	OpenGlVendor: ATI Technologies Inc.
	CpuCount: 8
