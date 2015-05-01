# Combustion-Engine-Crashs-the-Game
Hey guys, everytime, when tryed to use the Combustions Engine, it always give a bug and closes the game. I alredy updated the Forge, the Build Craft and the Industrial Craft too... Can someone give me a solution of what to do? I'm playing at 1.7.10.
---- Minecraft Crash Report ----
// Surprise! Haha. Well, this is awkward.

Time: 30/04/15 23:02
Description: Unexpected error

java.lang.IllegalArgumentException: Cannot create a fluidstack from a null fluid
	at net.minecraftforge.fluids.FluidStack.<init>(FluidStack.java:36)
	at net.minecraftforge.fluids.FluidStack.<init>(FluidStack.java:67)
	at buildcraft.energy.TileEngineIron.getGUINetworkData(TileEngineIron.java:280)
	at buildcraft.energy.gui.ContainerEngine.func_75137_b(ContainerEngine.java:57)
	at net.minecraft.client.network.NetHandlerPlayClient.func_147245_a(NetHandlerPlayClient.java:1151)
	at net.minecraft.network.play.server.S31PacketWindowProperty.func_148833_a(SourceFile:26)
	at net.minecraft.network.play.server.S31PacketWindowProperty.func_148833_a(SourceFile:9)
	at net.minecraft.network.NetworkManager.func_74428_b(NetworkManager.java:212)
	at net.minecraft.client.multiplayer.PlayerControllerMP.func_78765_e(PlayerControllerMP.java:273)
	at net.minecraft.client.Minecraft.func_71407_l(Minecraft.java:1602)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:973)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:898)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at net.minecraftforge.fluids.FluidStack.<init>(FluidStack.java:36)
	at net.minecraftforge.fluids.FluidStack.<init>(FluidStack.java:67)
	at buildcraft.energy.TileEngineIron.getGUINetworkData(TileEngineIron.java:280)
	at buildcraft.energy.gui.ContainerEngine.func_75137_b(ContainerEngine.java:57)
	at net.minecraft.client.network.NetHandlerPlayClient.func_147245_a(NetHandlerPlayClient.java:1151)
	at net.minecraft.network.play.server.S31PacketWindowProperty.func_148833_a(SourceFile:26)
	at net.minecraft.network.play.server.S31PacketWindowProperty.func_148833_a(SourceFile:9)
	at net.minecraft.network.NetworkManager.func_74428_b(NetworkManager.java:212)
	at net.minecraft.client.multiplayer.PlayerControllerMP.func_78765_e(PlayerControllerMP.java:273)

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityClientPlayerMP['nidsley1'/306, l='MpServer', x=-64,69, y=64,62, z=126,77]]
	Chunk stats: MultiplayerChunkCache: 1056, 1056
	Level seed: 0
	Level generator: ID 00 - default, ver 1. Features enabled: false
	Level generator options: 
	Level spawn location: World: (-68,64,108), Chunk: (at 12,4,12 in -5,6; contains blocks -80,0,96 to -65,255,111), Region: (-1,0; contains chunks -32,0 to -1,31, blocks -512,0,0 to -1,255,511)
	Level time: 1260484 game time, 1610556 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
	Forced entities: 105 total; [EntitySkeleton['Esqueleto'/9475, l='MpServer', x=-34,47, y=24,00, z=59,94], EntityCreeper['Creeper'/9478, l='MpServer', x=-35,50, y=24,00, z=60,50], EntitySheep['Ovelha'/17, l='MpServer', x=-77,03, y=62,00, z=135,34], EntitySkeleton['Esqueleto'/8728, l='MpServer', x=-27,50, y=15,00, z=47,50], EntityBat['Morcego'/8735, l='MpServer', x=-45,47, y=29,89, z=54,00], EntityBat['Morcego'/8742, l='MpServer', x=11,50, y=50,00, z=149,00], EntityBat['Morcego'/10024, l='MpServer', x=-17,54, y=17,29, z=164,92], EntityBat['Morcego'/10026, l='MpServer', x=-17,30, y=18,21, z=165,41], EntityZombie['Zumbi'/9005, l='MpServer', x=-135,50, y=13,00, z=55,50], EntityBat['Morcego'/10031, l='MpServer', x=-24,25, y=19,10, z=165,25], EntitySkeleton['Esqueleto'/9015, l='MpServer', x=-47,50, y=24,00, z=48,50], EntityZombie['Zumbi'/10047, l='MpServer', x=-37,50, y=35,00, z=57,50], EntityZombie['Zumbi'/11590, l='MpServer', x=-99,50, y=10,00, z=124,50], EntityMechanicalArm['desconhecido'/595, l='MpServer', x=-65,00, y=63,00, z=129,00], EntityBlock['desconhecido'/596, l='MpServer', x=-69,25, y=67,25, z=133,25], EntitySheep['Ovelha'/85, l='MpServer', x=-139,94, y=74,00, z=111,97], EntityBlock['desconhecido'/597, l='MpServer', x=-66,75, y=28,00, z=133,25], EntityBlock['desconhecido'/598, l='MpServer', x=-66,75, y=67,25, z=130,75], EntityPig['Porco'/86, l='MpServer', x=-131,28, y=63,00, z=136,09], EntityBlock['desconhecido'/599, l='MpServer', x=-66,60, y=27,00, z=133,40], EntityPig['Porco'/87, l='MpServer', x=-135,06, y=63,00, z=159,22], EntitySheep['Ovelha'/88, l='MpServer', x=-133,72, y=63,00, z=160,22], EntitySheep['Ovelha'/96, l='MpServer', x=-125,91, y=68,00, z=89,03], EntityHorse['Cavalo'/97, l='MpServer', x=-119,09, y=63,00, z=97,00], EntityPig['Porco'/98, l='MpServer', x=-115,31, y=63,00, z=112,22], EntitySheep['Ovelha'/99, l='MpServer', x=-132,81, y=63,00, z=115,50], EntityCreeper['Creeper'/101, l='MpServer', x=-114,50, y=63,00, z=142,50], EntityPig['Porco'/102, l='MpServer', x=-120,03, y=63,00, z=148,84], EntityZombie['Zumbi'/8295, l='MpServer', x=-27,50, y=15,00, z=147,50], EntityZombie['Zumbi'/9323, l='MpServer', x=-23,50, y=35,00, z=80,91], EntitySquid['Lula'/109, l='MpServer', x=-107,09, y=56,00, z=69,78], EntitySquid['Lula'/110, l='MpServer', x=-101,56, y=56,31, z=74,59], EntitySheep['Ovelha'/111, l='MpServer', x=-99,16, y=63,00, z=105,78], EntityZombie['Zumbi'/112, l='MpServer', x=-99,50, y=10,00, z=112,50], EntityHorse['Cavalo'/113, l='MpServer', x=-103,81, y=61,08, z=120,34], EntitySheep['Ovelha'/114, l='MpServer', x=-99,72, y=63,00, z=117,84], EntityPig['Porco'/115, l='MpServer', x=-104,94, y=63,00, z=136,06], EntitySkeleton['Esqueleto'/116, l='MpServer', x=-103,50, y=57,00, z=146,50], EntityZombie['Zumbi'/7802, l='MpServer', x=-57,56, y=11,00, z=48,91], EntitySpider['Aranha'/8314, l='MpServer', x=-50,50, y=34,00, z=108,50], EntitySquid['Lula'/127, l='MpServer', x=-88,50, y=56,00, z=71,50], EntityBat['Morcego'/9343, l='MpServer', x=-39,44, y=21,67, z=58,56], EntitySquid['Lula'/128, l='MpServer', x=-91,91, y=56,00, z=70,13], EntityBat['Morcego'/9344, l='MpServer', x=-47,00, y=21,82, z=52,22], EntitySquid['Lula'/129, l='MpServer', x=-106,81, y=56,31, z=76,38], EntitySquid['Lula'/130, l='MpServer', x=-97,53, y=56,16, z=73,72], EntitySquid['Lula'/131, l='MpServer', x=-81,78, y=56,00, z=85,50], EntitySkeleton['Esqueleto'/10371, l='MpServer', x=-24,50, y=16,00, z=195,50], EntitySquid['Lula'/132, l='MpServer', x=-86,53, y=56,13, z=81,22], EntitySkeleton['Esqueleto'/10372, l='MpServer', x=-25,50, y=16,00, z=196,50], EntitySquid['Lula'/133, l='MpServer', x=-70,59, y=56,31, z=79,50], EntitySkeleton['Esqueleto'/10373, l='MpServer', x=-24,50, y=16,00, z=199,50], EntitySheep['Ovelha'/134, l='MpServer', x=-100,81, y=63,00, z=129,69], EntityCreeper['Creeper'/10374, l='MpServer', x=-23,50, y=16,00, z=195,50], EntitySheep['Ovelha'/135, l='MpServer', x=-83,50, y=70,00, z=159,50], EntityCreeper['Creeper'/10375, l='MpServer', x=-23,50, y=16,00, z=198,50], EntitySheep['Ovelha'/136, l='MpServer', x=-81,50, y=71,00, z=157,50], EntitySquid['Lula'/152, l='MpServer', x=-76,06, y=56,22, z=84,78], EntitySquid['Lula'/153, l='MpServer', x=-70,88, y=56,00, z=81,38], EntitySquid['Lula'/154, l='MpServer', x=-84,16, y=56,00, z=83,50], EntitySquid['Lula'/155, l='MpServer', x=-75,50, y=56,31, z=85,94], EntitySquid['Lula'/156, l='MpServer', x=-71,50, y=56,31, z=82,44], EntitySquid['Lula'/157, l='MpServer', x=-78,19, y=56,31, z=83,56], EntitySlime['Slime'/158, l='MpServer', x=-71,69, y=12,00, z=104,69], EntityZombie['Zumbi'/167, l='MpServer', x=-58,53, y=11,00, z=47,94], EntitySkeleton['Esqueleto'/168, l='MpServer', x=-55,50, y=35,00, z=53,50], EntitySquid['Lula'/169, l='MpServer', x=-63,47, y=56,08, z=77,50], EntitySheep['Ovelha'/170, l='MpServer', x=-59,69, y=63,00, z=175,34], EntitySheep['Ovelha'/171, l='MpServer', x=-48,34, y=63,00, z=169,19], EntityZombie['Zumbi'/177, l='MpServer', x=-42,50, y=19,00, z=52,50], EntityBat['Morcego'/178, l='MpServer', x=-28,46, y=12,74, z=73,20], EntityClientPlayerMP['nidsley1'/306, l='MpServer', x=-64,69, y=64,62, z=126,77], EntitySpider['Aranha'/179, l='MpServer', x=-43,84, y=45,00, z=62,78], EntitySpider['Aranha'/180, l='MpServer', x=-41,72, y=41,00, z=54,59], EntitySpider['Aranha'/182, l='MpServer', x=-41,81, y=41,00, z=64,63], EntityBat['Morcego'/183, l='MpServer', x=-32,53, y=29,10, z=72,00], EntityBat['Morcego'/184, l='MpServer', x=-22,64, y=16,40, z=78,11], EntitySkeleton['Esqueleto'/185, l='MpServer', x=-38,16, y=45,00, z=67,69], EntitySquid['Lula'/186, l='MpServer', x=-59,25, y=56,11, z=73,50], EntitySheep['Ovelha'/187, l='MpServer', x=-39,94, y=63,00, z=90,97], EntitySheep['Ovelha'/188, l='MpServer', x=-37,22, y=63,00, z=165,34], EntitySheep['Ovelha'/189, l='MpServer', x=-32,72, y=72,00, z=196,66], EntityBat['Morcego'/196, l='MpServer', x=-37,66, y=12,28, z=67,20], EntityBat['Morcego'/197, l='MpServer', x=-34,01, y=12,99, z=65,28], EntityCreeper['Creeper'/198, l='MpServer', x=-30,50, y=32,00, z=73,50], EntityZombie['Zumbi'/199, l='MpServer', x=-28,50, y=32,00, z=74,50], EntityBat['Morcego'/200, l='MpServer', x=-32,74, y=23,22, z=66,78], EntitySheep['Ovelha'/201, l='MpServer', x=-22,31, y=57,45, z=76,31], EntityZombie['Zumbi'/203, l='MpServer', x=-18,50, y=24,00, z=83,50], EntitySheep['Ovelha'/204, l='MpServer', x=-25,38, y=63,00, z=181,53], EntitySheep['Ovelha'/205, l='MpServer', x=-19,53, y=64,00, z=191,25], EntitySheep['Ovelha'/215, l='MpServer', x=-10,81, y=63,00, z=76,47], EntitySkeleton['Esqueleto'/216, l='MpServer', x=-11,50, y=63,00, z=161,50], EntitySheep['Ovelha'/217, l='MpServer', x=-17,63, y=63,00, z=183,53], EntityZombie['Zumbi'/9961, l='MpServer', x=-2,94, y=17,00, z=190,50], EntitySheep['Ovelha'/234, l='MpServer', x=4,41, y=66,00, z=81,16], EntityCreeper['Creeper'/9962, l='MpServer', x=-9,50, y=16,00, z=188,50], EntitySheep['Ovelha'/236, l='MpServer', x=11,50, y=62,16, z=111,28], EntitySkeleton['Esqueleto'/237, l='MpServer', x=0,59, y=41,00, z=127,13], EntityCreeper['Creeper'/238, l='MpServer', x=14,31, y=35,00, z=116,69], EntityZombie['Zumbi'/10994, l='MpServer', x=-97,50, y=16,00, z=159,50], EntityEnderman['Enderman'/8693, l='MpServer', x=15,53, y=18,00, z=87,28], EntityBat['Morcego'/10493, l='MpServer', x=-15,50, y=13,84, z=174,04], EntityBat['Morcego'/10494, l='MpServer', x=-22,72, y=19,69, z=80,51], EntityBat['Morcego'/10495, l='MpServer', x=-26,34, y=11,82, z=72,24]]
	Retry entities: 0 total; []
	Server brand: fml,forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:373)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2444)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:927)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 8.1 (amd64) version 6.3
	Java Version: 1.8.0_45, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 242216592 bytes (230 MB) / 674402304 bytes (643 MB) up to 1060372480 bytes (1011 MB)
	JVM Flags: 6 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx1G -XX:+UseConcMarkSweepGC -XX:+CMSIncrementalMode -XX:-UseAdaptiveSizePolicy -Xmn128M
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 12, tallocated: 96
	FML: MCP v9.05 FML v7.10.130.1395 Minecraft Forge 10.13.3.1395 15 mods loaded, 15 mods active
	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	FML{7.10.130.1395} [Forge Mod Loader] (forge-1.7.10-10.13.3.1395-1710ls.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Forge{10.13.3.1395} [Minecraft Forge] (forge-1.7.10-10.13.3.1395-1710ls.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	CodeChickenCore{1.0.3.28} [CodeChicken Core] (minecraft.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	NotEnoughItems{1.0.3.60} [Not Enough Items] (Not-Enough-Items-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	Backpack{2.0.1} [Backpack] (Backpacks-Mod.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Core{6.1.5} [BuildCraft] (buildcraft-6.1.5.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Builders{6.1.5} [BC Builders] (buildcraft-6.1.5.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Transport{6.1.5} [BC Transport] (buildcraft-6.1.5.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Silicon{6.1.5} [BC Silicon] (buildcraft-6.1.5.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Factory{6.1.5} [BC Factory] (buildcraft-6.1.5.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	BuildCraft|Energy{6.1.5} [BC Energy] (buildcraft-6.1.5.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	IC2{2.2.657-experimental} [IndustrialCraft 2] (Industrial-Craft-2-Mod-Experimental-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	cfm{3.4.7} [§9MrCrayfish's Furniture Mod] (MrCrayfishs-Furniture-Mod-1.7.10.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	ReiMinimap{1.7.10} [Rei's Minimap] (ReiMinimap-1.7.10-3.6.jar) Unloaded->Constructed->Pre-initialized->Initialized->Post-initialized->Available->Available->Available->Available
	GL info: ' Vendor: 'ATI Technologies Inc.' Version: '4.4.13283 Compatibility Profile Context 14.501.1003.0' Renderer: 'AMD Radeon R9 200 Series'
	Launched Version: 1.7.10-Forge10.13.3.1395-1710ls
	LWJGL: 2.9.1
	OpenGL: AMD Radeon R9 200 Series GL version 4.4.13283 Compatibility Profile Context 14.501.1003.0, ATI Technologies Inc.
	GL Caps: Using GL 1.3 multitexturing.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Anisotropic filtering is supported and maximum anisotropy is 16.
Shaders are available because OpenGL 2.1 is supported.

	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: []
	Current Language: Português (Brasil)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Anisotropic Filtering: On (16)
