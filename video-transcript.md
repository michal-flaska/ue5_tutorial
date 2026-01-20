# hello

i created a transcript of the video so i dont want to spend a lot of time when i get lost when i can find the text faster. This is not here to recreate/replace the original video.

---

## video chapter timestamps
```
⌨️ (0:00:00) Introduction
⌨️ (0:01:31) System Requirements
⌨️ (0:03:34) Installing The Engine
⌨️ (0:06:12) Creating A Project
⌨️ (0:09:54) Unreal Editor Basics
⌨️ (0:23:27) Creating Levels
⌨️ (0:29:50) Landscapes
⌨️ (0:35:42) Blueprints
⌨️ (0:42:57) Blueprint: Variables
⌨️ (0:49:42) Blueprint: Structures
⌨️ (0:54:37) Blueprint: Enumerations
⌨️ (0:59:36) Blueprint: Functions
⌨️ (1:05:58) Blueprint: Macros
⌨️ (1:09:25) Blueprint: Collapsed Graphs
⌨️ (1:12:56) Blueprint: Branching
⌨️ (1:14:51) Blueprint: Switch
⌨️ (1:17:43) Blueprint: While Loop
⌨️ (1:21:23) Blueprint: For Loop
⌨️ (1:25:10) Blueprint: Array
⌨️ (1:28:24) Blueprint: Flip-Flop
⌨️ (1:30:21) Blueprint: Do-Once
⌨️ (1:32:25) Object Oriented Programming
⌨️ (1:39:29) Blueprint: Classes
⌨️ (1:49:49) Blueprint: Actors
⌨️ (2:02:41) Blueprint: Casting
⌨️ (2:05:01) Basic Inheritance Hierarchy
⌨️ (2:08:32) Blueprint: Character
⌨️ (2:31:52) Blueprint: Timer (Example)
⌨️ (2:37:05) Action Mappings
⌨️ (2:43:26) Expose On Spawn
⌨️ (2:46:38) Interaction System
⌨️ (2:53:09) Blueprint: Linetrace (Raycast)
⌨️ (3:03:17) Blueprint: UI
⌨️ (3:32:12) Blueprint Function Library
⌨️ (3:35:17) Plugins (Basics)
⌨️ (3:40:39) Modelling Tools
⌨️ (3:46:45) Static Mesh
⌨️ (3:48:13) Nanite
⌨️ (3:50:02) Materials
⌨️ (4:05:31) Skeletal Mesh and Anim BP
⌨️ (4:22:32) C++ Prerequisites
⌨️ (4:39:37) C++: Basics
⌨️ (4:45:04) Advanced Inheritance Hierarchy
⌨️ (4:55:28) C++: Variables
⌨️ (4:58:11) C++: Functions
⌨️ (5:00:04) C++: UCLASS, UPROPERTY, UFUNCTION
⌨️ (5:09:11) C++: USTRUCT
⌨️ (5:17:52) C++: Using Unreal’s Functions
⌨️ (5:22:10) C++: Enumerations
⌨️ (5:24:53) Converting Blueprint To C++
⌨️ (5:40:52) Blueprint Interface
⌨️ (5:46:38) C++ Interface
⌨️ (5:54:40) BlueprintImplementableEvent
⌨️ (5:57:02) BlueprintNativeEvent
⌨️ (6:01:40) C++: Array
⌨️ (6:11:30) C++: Map
⌨️ (6:17:31) Actor (Advanced)
⌨️ (6:39:54) Character(Advanced)
⌨️ (6:50:43) Player Controller(Advanced)
⌨️ (6:52:46) Game Mode (Advanced)
⌨️ (6:56:47) Game State (Advanced)
⌨️ (7:06:17) Game Instance
⌨️ (7:15:20) Creating Plugins
⌨️ (7:33:53) Third Party Libraries(Static)
⌨️ (7:51:42) Third Party Libraries(DLL)
⌨️ (8:05:29) Networking
⌨️ (8:07:06) Create/Join Sessions
⌨️ (8:15:24) Network Replication
⌨️ (8:22:48) Blueprint: Variable Replication
⌨️ (8:27:53) Blueprint: RPCs
⌨️ (8:43:46) Networking In C++
⌨️ (9:01:22) Unreal Engine Source
⌨️ (9:04:54) Switching Engine Versions
⌨️ (9:12:11) Packaging
⌨️ (9:17:13) BONUS
```

---

## transcript

00:00:00
un rail engine is a 3D computer Graphics game engine that has been used to create many popular games in this full course for beginners surov will teach you how to use Unreal Engine 5 surov has seven years of game development experience and has developed multiple games hi there game devs welcome to my beginner to Advanced game development course on Unreal Engine 5 in this course we'll be taking a deep dive into the engine and hopefully by the end of this course you would be able to create a game

00:00:31
completely by yourself now before you actually start developing a game in Unreal Engine some of you guys may have a question on what sort of a system to get for Unreal Engine now the docs is a bit outdated on this page however uh this page whatever is there is uh insufficient in my opinion I have been working on Unreal Engine for almost 7 years now and I feel this system isn't going to be handling anything so 8 gigs of RAM isn't enough and for the video card I would recommend at least going for something like a,

00:01:14
1650 or an RTX 3050 if you were to ask me I have worked in unreal for about 4 to 5 years with a 1050 TI that totally works however your experience isn't going to be that great and you will have to turn down all the settings as well and for the CPU a ryzen 5 or an Intel i7 would do six course or higher uh preferably eight or even 12 course would be better but make sure if you do get more number of course you scale up the other components as well there are a couple of things for example in visual

00:01:53
studio uh when you compile a program you will actually need more RAM as you scale up the number of cores on your CPU so that's one thing to note and if you scroll down you you would see this list over here although this system is highly Overkill and the GPU is outdated of course one noteworthy thing is a solid state drive which I highly recommend do not use a hard drive for your active projects the experience isn't going to be that great so with that all being said let's actually start

00:02:30
by talking about the installation [Music] process now there are two ways in which you can get hands on Unreal Engine one is through the epic games launcher so just search epic games launcher download the launcher and once you actually log in and do the regular signup stuff you can go ahead and click on Unreal Engine and head into library and you should be able to add an engine version now as of this date the the latest table build is 5.0.3 however 5.1 is in preview and we we shall hopefully upgrade to that it

00:03:08
has quite a few exciting features which I would love to show and the other way is to download the source code now you could use git or something and copy the link and clone it like that or you could just download the zip file from here and then there are a bunch of steps to actually install it uh we'll be going through this later in the course and also for more advanced users those of you who will be working with dedicated servers might need the source build as well now if you guys don't have access

00:03:43
to this repository you just have to request the permission uh this is a private repository by default and it's pretty easy to get it and once you do get access to it you'll be able to view this page there are quite a few tutorials on YouTube on how to do that so you guys could check any one of those out once you install the unreal editor through the epic games launcher uh you'll also need a code editor in order to work with the C++ files so generally you use visual studio for it now the documentation goes pretty

00:04:20
well on what components you need and stuff and if you do need any additional components uh the installer is going to prompt you and it's pretty straightforward for to be honest now you don't require vs 2019 you could use 2022 there is absolutely no issues uh I'll be showing you guys how to set the default code Editor to be vs 2022 as well a bit later so that's about it for the code editor I guess now we can go ahead and create a project and let's create a game so I'm in the epic games launcher

00:04:56
right now and before we actually launch the engine I just wanted to talk about the installation options try your best even though it looks large to have debugging symbols those are going to help us out [Music] later now you can go ahead and click launch once the loading is done you should be inside the unreal project browser where you can create your projects now yours might look a bit different I haven't selected templates so I don't see first person third person and all that however Our intention here

00:05:34
is to learn so we aren't really going to use those templates we might look into them a bit later on but for now we'll be starting with a blank project and a couple of noteworthy things two things actually the first thing is the project location I always suggest having an unreal projects folder in your solid state drive and maybe move them to a secondary drive if you're not working on them now for the project defaults everything is fine except blueprint and C++ uh basically every C++ project will

00:06:11
have blueprint and everything else that you'll need to work with the editor however when you select a blueprint project there is one additional step if you want to start working with C++ as well please note that blueprint and C++ work complimentary with each other and every project in my opinion should use a combination of the two and shouldn't be purely C++ nor should be purely BL blueprint so let's create a C++ project and let's leave it at desktop maximum and we didn't download the stter content

00:06:45
so we don't have it but that's totally fine we can add it later on now for the project name we can go ahead and name it let's call it beginner to Advanced course or I'll just call it beginner course so let's create that once you open your project a visual studio window like this with your project solution open should be open by default if not head into the editor go to tools and click on open Visual Studio 2022 and here's where I'll just show you guys how to change the default code

00:07:26
editor let's say you have a slower computer head into to editor preferences and over here type in code editor and you should be able to change it to visual studio code or whatever let's say you do change it to vs code over here under Tools again you should be able to find refresh Visual Studio code project once you do that you should be good to go one thing that you will immediately notice is my editor layout does not look exactly like like yours the reason is I have set mine to the Unreal Engine 4

00:08:04
layout so the way you do that is by heading into Windows load layout and this is the one you'll probably have and you can hit control space in order to get your uh content drawer but I feel like it just adds an additional step in viewing your content and I honestly prefer the Unreal Engine 4 layout but it's completely up to you everything else should be in the same place so I'm going to be using the u4 layout you can choose to use the default one if you wish and in case you want to go full

00:08:38
screen here in the ue4 layout just get your viewport into Focus just in case you're wondering the middle large portion of the screen is called the viewport once you get it into Focus hit f11 on your keyboard to go full [Music] screen let's start talking about the actual GUI of the unreal editor so the first thing is your menu bar which contains file edit window tools build select and so on these are just the normal options that you would see on in any other computer software so let's say

00:09:18
you wanted to save everything you would go go ahead and click save all however there's a key over here as well on the content browser which you will be using more often in this editor and under edit you also have a couple of important things obviously for undo redo and functionality like that you'll prefer the shortcut keys so for example let's say I add in a light over here and I go to edit you could undo that but I just prefer using contrl Z and control Y and the editor preferences project settings

00:09:53
and plugins are a couple of options which you will use quite a bit we will be getting into all of those in detail later on now window as the name suggests has to do with uh your actual GUI so here for example if I wanted to know what game mode I have and again we will be getting into all of that so I can just go to world settings which contains the game mode info so it says game mode override none we can set that to be game mode for example and stuff like that it all depends on what you exactly need you

00:10:29
could grab in a second viewport as well in case you needed it stuff like that and under Tools the only thing which we'll probably use here is going to be creating a new C++ class and occasionally we might need to refresh our project file and nothing else actually find in blueprints is something handy so in case you have written some blueprint code and you want to find it like in your entire project then it's a useful thing and build is for building your lighting and stuff basically uh baking

00:11:06
your lighting uh select not really sure who would use that because most of the operations over there can be done by shortcut keys so that's your menu bar and under this there's another panel over here where you have another save button and under this select mode option over here here you have quite a few options landscape is something which you will use uh when you're working with you know larger Maps so you can go ahead and create Landscapes so what I'll do is I'll create a brand new level to

00:11:43
Showcase those things and over here in blueprints this is where you would access your level blueprint and I will get to what is that a bit later this option right here is mostly for cinematics so let's say you're making a trailer for your game or something uh these are the things which you would use and this is just to play your game so if I hit play I can see what the game looks like while you're playing it one more thing let's say you wanted to look at how your game looked while you're

00:12:13
playing without actually playing it you can press G on your keyboard and it it's going to go into game mode which will show you exactly how your game will look when it is being played and next up uh you have this button right here where it allows you to launch the game and stuff we'll be going into this a bit in detail later on now for those of you guys who have slower computers you can head into settings over here engine scalability settings and you can set Yours to low now how do you check your frame rate

00:12:51
you may ask because that's a major concern I feel like you do require about 50 to 60 FPS in order to have a smooth editor experience so the way you check that is by hitting your tiled key under your Escape key that is if you guys aren't familiar once you do that your focus should be in this enter console command window at the bottom of your screen type in stat FPS and you might see that it's locked at 120 if you have a fast computer so what I'll do is I'll type in t. Max FPS s and you can just type in a

00:13:31
crazy value like 999 so this is my actual uncapped frame rate now this introduces us to another window this is known as the console now the console is really useful basically almost every setting you see over here and quite a few other settings which we will talk about later can be set using the console it's quite handy let's say you're debugging your game and you don't have an actual button to change your graphic settings you could use the console and change it as well there are

00:14:08
many other uses for it for example in multiplayer you can simulate lag and stuff like that in order to represent an actual multiplayer game so that's the console and your output log is your output log so let's say have printed something it's going to stay on your screen for about 2 seconds or how much ever you set the duration but the output log is always going to have the print so for example now we haven't gone into blueprints but I'll just print something and show you guys if I just type in print string

00:14:46
hello you see you get hello over here but it's gone after 2 seconds however in the output log you should be able to still see Hello it should be all the way down as you see you get hello now don't worry about all these errors it's really nothing to worry about so that's about it and on the left hand side you have the place actors panel where you know you have various options you'll really not be using this you'll generally just drag those from the content browser it just contains the

00:15:28
same old things and the recent stab may be helpful if you're placing the same object over and over again one thing that you might use this for is for a player start player start is basically where your player is going to spawn just press G on your keyboard if it ever disappears you're probably in game mode if you don't see it and if you want to get close to it like how I did uh make sure that is selected and press F on your keyboard F stands for focus and it's going to go near it the camera

00:16:02
is going to go near that now once that's done let's talk about this massive chunk of the screen this is known as the viewport this is where you'll actually arrange your level and do stuff so for example if you want to place something you drag that in the viewport and that's going to be added into your level now in order to navigate your viewport there are quite a few methods which you can use one is known as the Maya style navigation where you use alt and your mouse buttons and there are

00:16:36
many other styles which I won't get into it's kind of pointless but there is one style which I personally prefer and I feel almost everyone is going to prefer that that is by using your right Mouse button and your W this is similar to how you move in video games except you're holding the right Mouse button here so hold down your right Mouse button and you can use your w a s and D keys and move your mouse so this gives you all degrees of freedom so you can rotate you can pan around you can do

00:17:09
everything so this is my favorite way of navigating just try it a couple of times it's just a matter of getting the feel of it and if I want to speed up the camera which I will get into later you can use your scroll wheel along with this and your camera speed is going to change there are a couple of options again here now here uh instead of the console command you could use this as well to show your FPS and quite a few other options which you would generally not use screen percentage is basically a resolution

00:17:42
scale you could set that all the way up there I'd leave mine at 100 and this is to change between perspective and orthographic views let's say you're aligning something from the top you would go to your top orthographic View now you might see everything is wireframe so you can change that here as well go to LIT let's say there are shadows interrupting your work you could head into unlit there are many other view modes which you generally use for optimization and things like that but generally you would stay in lit

00:18:20
unlit or wireframe itself maybe a couple of times you might use one of these uh other settings but I've never found myself needing those so that's there and scalability is basically the same thing which we saw over here I can set that to cinematic for example in my case it shouldn't really matter that's about it and in these options on the right hand side this one basically allows you to select objects so let's say I click on this I select this now let me get closer a bit let's head into perspective so if I

00:19:05
click on this I can select it now when I click on something now I'll create another Point light when I click on something and I have it selected if I want to move it I can press W on the keyboard or if I want to rotate it I can press e on the keyboard and if I want to scale it for a light it's kind of useless but it is going to scale the radius I believe so for that I can hit r on my keyboard in order to scale things or you could use these uh buttons over here so this is for move this is for

00:19:45
rotate and this is for scale all right so once that said uh this uh button right here changes between uh local and World space now over here if I just drag in a cube for example under shapes you should find Cube and if I change this to local space now when I rotate this Cube you see the Gizmo rotates along with it and now I can move it along its rotation but let's say I wanted to rotate it along with the world's XYZ the way I do that is by heading into World space so now you see it's aligned to the word XYZ

00:20:30
that is your actual coordinate axis but this cube is rotated as you can see so if I want to move it along that rotation I can head into local space again if you're familiar with 3D modeling software these will sound pretty familiar to you the next thing is grid snapping now if I were to come close enough you would see that it's moving in increments it's not moving smoothly that's because grid snapping is enabled and snapping distance is set to 10 so I can just click on this button and

00:21:04
disable grid snapping and now you see the object moves smoothly same goes with rotation if I disable that I can smoothly rotate the object if I enable that it's going to rotate in increments of 10 same with the scale as well now this map is pretty huge and it's taking quite a while for me to actually go this far so the way I can actually move faster is by using this camera speed button so if I head into eight as you see we are moving very fast one more thing is if you scroll while using your right click and W ASD

00:21:50
basically I'm using that to move if you use right click and W ASD and you scroll at the same time you can actually adjust your camera speed so I have my right Mouse button held I have W ASD to move and if I scroll forward I'm going to move real fast now let's say scroll backwards I'm going to go slower so you can adjust your camera speed with your scroll wheel as well and of course you can adjust it over here and if you want the camera to be even faster you can go ahead and set this

00:22:22
multiplier thing and that's about it [Music] now let's actually start creating something so the way you would actually go about doing stuff is creating something under your content folder now you might have some things over here if you have enabled starter content and stuff but in our case we don't have anything so one thing is whenever you create new levels it's always advisable to have a Maps folder in your content folder where you actually put all your Maps so head into this folder and in

00:23:04
order to actually create a blank level where you can start making your own right click click on create basic asset level or you can head into file new level anyway is okay and we can call this one beginner course level you could call it anything you want double click on it to open it up and I've already saved it uh it's asking us to save this map actually so actually don't save this now head into your project settings and this is where we start talking about some of the things which you might need

00:23:48
the first thing is maps and modes so in order to decide which level is going to open when you start the editor this is where you actually set it so anything associated with your project will be over here so for example your input bindings is something which you'll use a lot so all of those are there in the project settings so we can change the editor startup map to be beginner course level and we can set this to be beginner course level as well close that and if you were to notice there is actually a

00:24:19
small note here it says uh these settings are saved in default engine.ini which is currently writable what do I mean by that is if I head into my project directory and if I head into config there are actually many config files so for example if I open up default engine.ini it says edit a startup map equals and it has the relative path of the map and you have a bunch of other settings as you can see these are useful we will actually talk about console config file in detail later on there are other config files as well

00:25:04
most of which you won't use you would mostly just use default engine.ini now heading back to our level you see everything is completely empty now one of the first things that you will need is a sky actually so if you just search in Sky you're going to find a skylight Sky atmosphere we are just going to be using a skylight for now and if you just type in atmosphere you would you get the same Sky atmosphere here so you can go ahead and drag that as well and if you type in fog you'll be

00:25:42
able to get exponential height fog now you will see the effects of it if you Tinker around with this yourself basically all of these things just do what they say so exponential height fog is going to add fog and if you want to change the properties of this always head into your details panel and this is where you'll adjust all the properties now for something like fog the location and stuff doesn't matter so anything you place the location of it is going to be stored here location rotation and scale just

00:26:16
know that location rotation and scale combined in Unreal Engine is known as a transform we'll be using that a lot now let's say you had a light which was fixed and you want the Shadows to just be baked in and you have nothing to calculate dynamically you could set your light to be static or it it goes the same with any other object if you're not going to be moving it it's going to be static stationary is almost like static but there are a couple of things which dynamically changes it's generally used

00:26:51
for your directional lights which acts as your sun basically so we can drag that as well so if I type in directional light you see we get everything else that we need if I remove the fog you would see that the fog went now for example here I have lost my directional light and or any other component so in order to navigate to that you can use this outliner window which will have a list of all the objects that are in your scene you can do quite a few things actually if you want you could select these and you could actually put those

00:27:29
in one folder so I can go ahead and right click create a folder and I can just drag those inside this folder you could do that as well in the outliner so now let's say you lose your directional light you can head over here and let's just call this one sky for example let's just call it Sky actors I'll tell you guys why we call them actors a bit later on so you can drag in Sky atmosphere Skylight and stuff like that so these are the basic components of your Sky now if I go ahead and zoom

00:28:05
into my directional Light press e on my keyboard and rotate it you see the sun moves along with it so let's say we wanted an evening Sky we would use something like this and if you would notice the mobility set to stationary you could set it to movable then everything will be calculated dynamically and you won't have to build build the lighting you could set it to stationary as well you could set it to static if you don't have any moving objects in your level now let's go ahead and just save

00:28:45
everything now let's start actually creating something in our [Music] level so first of all remember I told you about the land skipe tab this is what you would use if you have a larger world but for our purposes I'll just show you guys how to work with Landscapes even though we aren't really looking for a large world so here you can select your landscape material but you can change it anytime anyways and let's say you wanted a water body or something or uh let's say you wanted to have multiple multiple

00:29:24
layers you know in your landscape you can click on enable edit layers uh and these things are basically a transform and stuff like that and these things are just these options number of components and the overall resolution arej just the size of your landscape so you can play around with that to see uh what the Precision or rather I should say the detail level of the landscape and the size should be depending on that you can increase that or you can go ahead and use a height map I actually have a sh on my channel on how to use

00:30:00
height Maps properly in Unreal Engine but for our purposes we'll just create our own so let's just create everything with the default options and let's hit on create so it is going to take a while and once we're done with that we have a landscape now if I go ahead and press play as you can see I can navigate around this landscape just like you can navigate in any other level so now what I'm going to do is I'm going to edit the landscape now these are the tools that we'll be using to

00:30:42
edit our landscape so you have to be under landscape mode and under this section over here you would find sculpt you can increase the tool strength you can get the brush type over here as well uh one thing that you will use is probably the alpha brush brush basically you can have your own mask and stuff but for our purposes we are going to be using the regular old Circle brush so I'll just increase the size uh this need not be the limit actually I can set this to 10,000 as well so if I go ahead

00:31:14
and do that you see we have kind of a mount in here now what if I wanted to randomize the bumpiness in the map I could use noise so you see it's going to be like this but this is overkill so I can go ahead and change the tool strength to something like 0.05 and as you see this is a lot more reasonable so this is what noised uses flatten as the name suggest is going to flatten your landscape at that level so let's say select this level everything else is going to go to that level if I use flatten now obviously you can

00:31:50
increase your tool strength if you wish completely up to you and there are many other things such as the brush fall off so basically if you want a softer brush so you could use the brush fall off and increase that if you want a completely hard brush you could go ahead and use this but as you can see it produces harsh effects so we aren't going to be using that again completely up to you and erosion is basically if you wanted to create natural looking slopes and stuff so for example so I'll just reset some of these

00:32:25
settings here so something like this you could experiment and find out what what each one does but generally you would stick to sculpt smooth flatten ramp and maybe sometimes You' use erosion and you would use uh noise and let me show what ramp does real quick so if I select ramp and if I go ahead and click somewhere and click in another place and and click on ADD ramp you see it Bridges those two locations with a straight line and this is going to be a ramp you could add a ramp anywhere like this so I can

00:33:12
go ahead and do this and I can click enter or I can press add ramp on the menu over there and it's going to add a ramp now if you had a character or something you can walk over it now again we can use the smooth tool in order to smoothen this up out so now these two in this intersection looks seamless so these are basically a landscape editing tools there is not much depth to it and not sure what Aras does actually so I've never used array to be honest you would just undo changes if you really had

00:33:51
to and one more thing if you wanted to do the inverse of an operation so let's say I am sculpting a land skip so let's say I wanted something like this so I'll increase the tool strength so make that let's say 0.14 now this is one way but what if you wanted a pit instead of a hill the way you do that is by holding shift it's going to reverse the operation and it is going to make a pit same goes for the other tools as well shift is going to be the inverse of the operation so that's about what you'll

00:34:29
use in the unreal editor most of the time so now we can start creating our own assets make sure you're first of all go into select mode again don't forget that and now we can go ahead and start talking about [Music] blueprints so let's start talking about blueprint B blueprint basically is the visual scripting language which is used to write game logic in Unreal Engine so blueprint code can be written in many types of assets if you right click go to blueprint class you can write blueprint

00:35:05
code in most of these assets and we will get to some of the important ones a bit later for example actor PA character player controller game mode there are few others such as the game State player State and so on we'll be getting into all that now the most basic type of blueprint is going to be a level blueprint so if you head into this menu over here click on open level blueprint you'd see you'd get a blueprint associated with your level now B in play is as the name suggests something which

00:35:35
is called as soon as the game begins or in this case as soon as you open the level please do not interpret begin play as when you click on the play button this is only called once you load into the level so let's say you loaded into another level the begin play for that level will be called as well in order to actually start writing code you would use some built-in functions or you could write your own so the way you do it is if you right click for example and if you just type in I don't know let's

00:36:09
say set location now let's say you want it to set the location of something in your level let's actually do that uh since this is objectoriented you will need context for everything so you need to know for Which object you're actually moving so for example let's say we have a point light here now one handy thing which I forgot to mention before let's say it's up over here and you want to snap it to the ground you can hit end on your keyboard and it's going to go to the ground level

00:36:39
now we have this have that selected and head back into your level blueprint if you right click you get an option create a reference to point light now internally this is a pointer to this object or rather I should say to this actor anything that can be placed in a level is called an actor just remember that now if I drag off of this now I want to get its location let's say for example now the search bar is really useful for that you don't really need to know the function names especially in blueprints

00:37:13
so just type in get location and you see get actor location now I can go ahead and print it for example so if I right click and type in print you see print string now now this is called a function even this will be called a function so let's say I drag off of this and I type in set actor location again uh every getter will usually have its own Setter if it can be set so what we are saying what we are implying by this is set the location of this point light to be zero which is what we have defined over

00:37:55
here now let's say we just wanted to move it up a bit so we can do plus and on the Z we can do 200 because Z is the up AIS in Unreal Engine and we can set that to be the new location so if I go ahead and press play don't see much uh see mobility of the light is set to stationary so we have to make it movable of course uh remember what I was telling you guys earlier with static and stationary you would assume it to be in the same place but with movable it's fully Dynamic so now if I press play you see it became

00:38:35
dimmer in case you guys wanted to see the change if you just press D on your keyboard and left click you get a delay node or you could right click and search for delay but I prefer using D if you press D and left click you get a delay node uh let's just keep a delay of 2 seconds and then let's move it up so if I press play as you see it got dimmer because it went up now this blueprint function has a couple of pins on the left so these are called pins the stuff from which you can drag off of now the Triangular one or

00:39:15
the pentagonal one I don't know what shape this is the one which drags off the white wires these ones are called execution pins so this function will be executed only when this pin goes from left to right so only when you connect something to it from the left and when this is executed this is going to be called and once this is done this is going to be executed now this one is a function as well get actor location is a function too however it does not have an execution pin you might notice the

00:39:47
reason is this is a pure function you can define a pure function whenever you need a function to return immediate values so what I mean by that so for example if I have this hit result and let's say I print this out so I can't print out a hit hit result I I figured so let's just take location now this is just a sweep hit result so let's say we move it somewhere and it collides with something in between it's going to return a hit result if you have sweep enabled uh now if I print this out this

00:40:22
value right here is actually cast so let's say I copy a print string and let's say I print this out again set actor location is not going to be called once again this value what you had is going to be cached in your memory however over here if I just drag off of get actor location and let's drag off of this once again so let me drag this over here this value is not cast what I mean is get location is executed each time I'm calling this print string wherever I am referring to this value the entire

00:41:07
function is going to be called once again and in this case it makes sense because whenever we execute get actor location we want the live location of of the actor not the location which it was in previously if we go by that logic we would get the location before it was set so we will get the live data using a pure function and the target Works in a similar way we are getting the point lights location so the target is point light now one more thing you might notice is event tick tick is basically a

00:41:41
function which is called on every frame so if I just hit print and if I just print out tick for example you would see it prints it a bunch of times basically every time a new frame is drawn uh the tick function is called [Music] now whatever I told you guys is just a vague overview of how blueprint works so I just talked about execution pins and that it's object oriented and types are color coded but now let's actually start talking about them one by one so the first thing you would want to do in any

00:42:17
sort of a programming language or if you're writing any code is first of all be able to store data and that's done through variables now the way you create a new variable able in Blueprint is by clicking on this little plus icon on the left hand side this menu is available in almost every blueprint so click on the plus icon and you can create a variable now let's just call it my variable for example now over here since blueprint is based on C++ obviously you you have to define a type for it so by default it's set to

00:42:54
Boolean but you can select any one of the other types I'll go some of the important ones if you're familiar with C++ these things will seem pretty simple to you guys so Boolean is basically a true or false value so for example if I drag my variable and let's say you want to get the value of a variable you can drag it and hit get so this is going to be the value so off of this pin let's say I I type in if we'll get to branching and stuff a bit later but I can do stuff like this since this is a

00:43:27
true or false value if this variable is true this execution pin is going to come out if the value is false this execution pin is going to come out so that's basically how it works same way with all the other types so I can click on this variable and change the type to integer which is basically a non-fractional number int 64 is basically a 64bit integer so let's say you have larger numbers so you would use integer 64 however I don't really find many cases for it float is a decimal number and then you have name String and

00:44:03
text all of which are string types most of the times you would be using string however in some cases you would use name as well for example in tags which we will talk about later and text is mostly used for uh UI and stuff like that so if whatever you see in menus and things like that uh the text the strings over there are stored as TT XT so that's the data type you'll use now a vector is a struct with three floats in it x y and z now obviously if you don't know what a struct is we will again talk about that

00:44:42
no issues Rotator is a similar thing except uh there is a limitation on what values you can have you can only have a value of zero up until 360 beyond that the Rotator is going to be invalid and and transform is basically a struct again which contains a vector a rotator and a vector so location rotation and scale so this is transform these are the fundamental types which you use most of the time however if you go under struct you would see there are a lot more you'll not use most of these uh some of the

00:45:23
common ones that you'll use are things such as hit result so hit result is a common one that you'll use now if I compile this and if I go ahead and drag this out and if I go ahead and break and one more thing if you want to get this variable there's a shortcut if you hold control and drag it you'll get the value and if you want to set this variable you can all drag it so that's just a small tip I can give you guys so now break hit result is going to show us all the different variables inside this now

00:45:56
similarly you can do that with any other struct if you just drag off of this and try type in break you can do that or with some structs you can you can even do split struct pin or actually with all strs so that's basically another way to see what members are there in the struct so for example uh similar to this this was the same struct over here so you see initial overlap so this going to be there blocking hit location and things like that so that's basically your struct that's how it works in Blueprint

00:46:30
and one different type is going to be our object type variable so for example if I select an actor and this was an object type as well if I drag off of this the variable which is color coded in your sky blue or your light blue color so these are basically object references internally when you write these in C++ so let's say you create an object reference for blueprint in C++ you can expose C++ variables to blueprint by the way they are stored as pointers so basically it's the memory address to that object now if some of

00:47:08
these things sound confusing to you just stick along and watch the course till the end and if you guys still have any confusions make sure you guys do check out a video on pointers and I will go over actors and stuff like that basically uh this very aable is going to refer to an actor and since this is a pointer and the default value is none so if I go ahead and click on this you see it says None So what this means is this is not a valid pointer and if we actually had some logic in C++ it would

00:47:43
throw an exception so that's basically how object types work and you also have enumerations which are are in in some disguise just your bite which is an unsigned 8 bit integer so basically uh for example if I just grab a random Eno here I can do a switch which we'll talk about so basically depending on the value of this variable you can perform your logic so a common thing that you would use it for is let's say you have a weapon in a game and depending on the type so let's say your weapon is fully

00:48:22
automatic you would have an enumeration so one of these enumerators is going to be full auto the other one is going to be semi-auto the other one's going to be bolt action and depending on that you would execute the appropriate logic so that's one way of using enums there are many applications of course we will get to most of them [Music] later now that's about how you basically create variables so now let's actually talk about a few special types of variables namely structs and enums now I

00:48:57
did show you what's a struct and an enum but I'm pretty sure it went all over your head if you're a beginner so let's just delete that and click on this variable and hit delete to delete that as well compile and save that now go ahead and right click create a new folder and call it structs and I'm doing this in my content folder uh you could do it in the same place if you want to follow along right click go ahead into Blueprints and create a structure and for now let's just call it my

00:49:32
struct Now structs by definition in C++ is going to be similar to your classes so basically you wrap a bunch of data and methods into a single unit however in Blueprint uh a structure purely refers to a collection of variables you cannot have functions for structs in Blueprint sadly however you could just create a library for that so you have blueprint function libraries and you could just create functions for your structs anyways so the way you work with this is you can create a bunch of member

00:50:12
variables a a very simple example is going to be a 2d Vector andreal engine already has a 2d Vector type but just for demonstration purposes let's just create one so let's just call this X and make this of type float because it's a decimal number add in another variable make it of type Y and make this of type float once again so basically my struct is going to contain these two variables now if I head back into my level make sure you save this and if I go ahead and right click somewhere and type in my

00:50:51
struct you see you get an option called Break make and set members so if I go ahead and press break you see you get options X and Y now just like how you create an integer or any other variable you can create a struct as well so let's just call this one I don't know maybe my variable once again and it's going to be of type my struct so my struct is the type so this is our user defined data type now I can go ahead and get this I can rightclick perform split structure pin once again so this is basically how structs work

00:51:30
basically you have one variable which stores multiple variables within it so this can be very handy for example in this hit result you have all these variables now it they not need not be the same type the types can be heterogeneous so I could have an integer over here I could have a string over here so let's say I have a student struct I could store name his role number and Stu like that so just a v example over there so that's basically how structs work in Blueprint so I'll just delete that we don't really need it

00:52:07
but we'll keep my struct uh let's actually have something more descriptive let's say we have name and let's say we have points this makes no sense right now but we can use this a bit later on and you could anytime add a new variable but remember avoid removing variables from St structs sometimes they do cause some issues with the blueprint so be careful with that in C++ though it won't be too much of a problem since you refer to the members by their names so that's one thing to note now one more

00:52:42
thing if you guys want to set the members of a struct what you would do is you just type in set members and you can get the struct name that is my struct in our case so we can use this and set the members now over here on the right hand side under default category you can get any one of the variables as spins and you can set the value now obviously you will need to tell it with struct so let's say you created a variable of type my struct so my struct you can go ahead and pass that as the struct reference now this is a

00:53:18
reference because this pin over here is diamond in shape or rhombus or whatever that is so that means it's a reference so it is referring to the actual uh variable that you pass in so it is going to adjust the value of this [Music] variable we will deal with a lot of structs as we move on however there's one more special type which I would like to mention and those are enumeration so I will right click create a new folder and I'll call this one enums open it up and over here I can head into blueprints again and type in

00:53:59
enumeration so this is basically a list of values and you could perform your logic depending on this list so let's just uh create an enum and let's call this one my enum again now over here you can add enumerators which basically are list items so let's say add three items so for example let's take names of fruits so Apple banana let's say and maybe a mango now once you do this these are basically the enumerators which are there and I will show you guys what it actually implies so I'll just go ahead

00:54:41
and create a new variable and I'll call this one I don't know let's say fruits choice for example and it's going to be of type my enum now internally ultimately an enumerator is just a number basically it's a number between 0 and 256 so for example over here apple is going to be indexed to one banana is going to be mapped to two and mango is going to be mapped to I mean one and uh mango is going to be mapped to two so 0 1 2 so that's how it's going to be internally now obviously you can give a description

00:55:21
as well over here in Blueprint uh so if I just drag this in now by by default it is set to Apple you can see the default value on the right hand side and we will talk about all these options a bit later on in the variable section so just to be brief uh if you are like creating new objects in your scene uh you would need some of these and for multiplayer and stuff you would need replication and we will talk about them in depth so nothing to worry about now you can cast it to a string so unreal has it built in to give this out

00:55:56
as a string so if you see you should get apple printed whoops I have something on tick so let's just delete that so nothing sprinting uh okay we have a delay of 2 seconds uh let's just delete the set act location stuff and just print this in and we could actually change this as well you can copy this and paste it by hitting control D so if you click on this and hit control D you can duplicate it and if you drag off of this you'll see you can perform a switch so basically if the value of fruits choice

00:56:39
is Apple it's going to perform this logic so let's just say healthy for example and for banana let's just give something else so it honestly doesn't matter copy that over and let's say we give tasty for mango so if I go ahead and press play you should see it says apple and healthy now if I set this value so if I alt drag it and I set this to banana now you should be able to see that it prints the second string so this is basically Al how enums work and this was actually uh a bit of a

00:57:32
lengthy way I did it there's actually another shortcut you can use in Blueprint in C++ though this is the only way uh you would just type in switch instead of using this node so one more shortcut is if you drag off of this and type in select depending on the value of this enum you can make it do certain things so let me remove the switch here so now what I'm saying is if the value of fruit's choice is Apple this is the value that will be passed so in this case I'll just type in one for example

00:58:07
and over here I'm going to type two and three so what we are seeing is if the value of this enumeration is Apple it's going to print out one so the value which will be returned here is going to be this value same with the other two choices so if I press play you see it says apple and it says two that's because we we had set our choice over here if I change this to Mango over here we are going to get three so that's basically how enumerations [Music] work now that we have a basic

00:58:42
understanding of data types in Unreal Engine let's start talking about the core scripting features in Blueprint so the first thing that you can do is create functions now a function is basically a block of code which adds functionality to your program so what I mean by that so in order to create a new function you can go ahead and click on this plus icon right here and we could call it whatever we want we could call this one my function and generally speaking you would use Pascal case so basically each

00:59:17
uh word is going to start with an uppercase character so generally that's a convention you use you could use a space as well in Blueprint but generally it's not a good practice now I can call this function from my event graph now if you see you have opened two tabs one is the event graph and one is my function so I can close my function and I can double click on this on the left hand side to open it as well now if I drag this in or if I right click and type in my function you can go ahead and call it so basically this is

00:59:52
going to execute my function so let's go ahead and actually do something with it now inside my function this is blank right now I can just go ahead and print a string and we can call this one my function is executed so I think I butchered the spelling but doesn't matter so if I go ahead and press play you see my function is executed now we can also pass in values so I have created this points variable here so just create a new variable and make it of type integer and call it points now if you head into your

01:00:31
function and click on this block right here you can actually add input and output parameters so if I click on the plus icon and change the type to integer and I can call this one points so I can take this points value from outside the function so if you look at this now you see I can pass in points so that's pretty handy now I can go ahead and print this out as well so I can print out my function is executed and I can print out points as well and if you double click on the wire you can use the reroute node to keep things a

01:01:11
bit clean now if I press play you see you get my function is executed and you get zero now if I change the value of points for example you see we get that number so this is basically how input parameters work now what if you had some return value now let's say instead of points this was health so let me just call this one Health so compile that and over here if I click on this once again I can add in an output and you see it creates a return node for us so this is basically like your return keyword in C++ so when

01:01:51
your function goes to this it's going to exit the function and the value whatever you want is going to be returned now you need not have it you can have an empty return node as well now in our case let's just return a Boolean and let's just call it B killed for example and let's change the name of this to be Health as well and we could do a simple if check we will talk about if as soon as we finish functions events and stuff like that so if I can't do that so let me just grab in an if if this value that is

01:02:30
our health is less than zero or less than or equal to zero then what we can do is if it is true and if you type in contr D you can have two return nodes so if our health is less than zero it's going to be true otherwise it's going to be a false now you can go ahead and print this out over here now our health is 32 so we should have false let's say we set our health to be minus1 which is invalid of course but we get true so this is how you can return values outside a function now one aspect of functions

01:03:16
which I did not cover and I'm recording this a bit later it's is going to be local variables so what if you had some variable which you wanted only within a function uh so let's say for example we have a variable temp for example so let's say you wanted a number to be stored temporarily inside so for that case you would use this local variable option they work exactly the same as you would as it works in C++ and one more thing the input parameters whatever you take are also local variables so you can just grab an

01:03:53
in and instead of dragging this actually you can right click and type in in and if I just get it so I should find it at the very end of somewhere or rather let me just type it get in so in is a really commonly used word so that's the reason we are getting it so many times here so let's actually change it so let's just type in in1 2 3 let's say so in1 23 so you can get it actually so you don't actually have to drag this let's let's say you have a large blueprint craft you don't have to

01:04:28
drag it actually you could you could just do this over here that works totally fine as well even over here actually you could do this and it's totally valid so that's about it for local variables as you use them you will kind of understand their purpose but without a solid example we will not actually be able to tell the use case however once we actually get to the end where we actually create something that is when we'll get to practical [Music] examples at the base level those are

01:05:05
what functions are and we will go a lot more in depth about functions events and stuff so not to worry about that I've just gone ahead and deleted that let's create a new one once again and now let's talk about the limitations and let's talk about the next type of scripting feature in Blueprint now one limitation that you would see is you cannot add a DeLay So if I right click and type in delay you actually don't get a delay node the reason is you cannot have latent nodes inside a function in

01:05:36
Blueprint so delay is actually a latent function so what I mean by that is it actually takes some time to execute so let's say I cut cut or copy this and paste it in here you see I cannot do that it says one or more copied notes could not be pasted into this graph so the way you can hand handle this is you can use a macro now macros and blueprints are more like functions than C++ macros so they work a little bit different now if I call this one my macro for example I can go ahead and add a delay

01:06:13
so I I can hold down D on my keyboard and left click and I can add in a delay one thing you'll notice is by default it doesn't have any input or output pins you can go ahead and add that but there is another advantage of Mac now for example let's say we uh we have a database on our server and let's say it takes some time to retrieve the data so let's say it takes around5 seconds for your computer to connect to the database and retrieve the data this is just an example it could be anything

01:06:47
that takes time for example uh the prime number program takes some time to execute after you go to a larger number so while this is being executed now let's say you just wanted to print out something saying that it's starting and then you want to do something else when it's completed this is where it can come handy now you can type in print string and you can call this one starting now you could come in here and now you'll notice this execution pin got disconnected you can't do them parallell

01:07:25
but there's a work around for that you can type in sorry sequence and over here you can just print this out and then you can go ahead and perform this and oh here in the output as well you can drag this in and a a handy thing which you cannot do in your return node in your function is you can have one more of these so now if I just give a longer delay so that we can recognize it and if I drag in my macro and if I print out strings over here and over here so we'll call this one done and here let's just

01:08:05
print uh starting underscore outside for example so if I press play starting now and starting outside got executed first then after 2 seconds our done was executed so things like that can be done by macros which you cannot do in functions [Music] now the whole point of using our own macros and functions is of course code reusability so let's say I want to call this macro once again I can just type in my macro and I can call it now one difference I would like to mention and then we'll head into the next one which

01:08:49
is collaps scphs is with a function let's say I call this my function my function I can actually execute this from another blueprint but this is not true for level blueprints it's a little more tricky to do it from level level blueprints you you guys will understand why once we actually head into classes and stuff but I'll just show you guys a simple example so I'll just create a blueprint here of type actor and we'll talk in depth about this later and let's say create a function as you can see the

01:09:25
same uh features in the blueprint are available here and let's just call it one test for example compile that now if I were to get an object reference to new blueprint so I'll just do that by dragging it into the level so I'll drag this and I'll create a reference and if you can notice I can actually call test from here however if I create a macro so let's just call this one test M for test macro you would see even once I save and compile everything I cannot call test m i see

01:10:06
test but I don't see test M so that's one more difference between a macro and a function you cannot call a macro from you know uh other blueprints but you can call functions from other blueprints of course if you set the aess specifier to be private in that then you can't call functions either but you can by default now what if you didn't want to reuse them what if you just had this code but this looks a bit messy so you wanted them to be shown as one node let's say this whole thing did something one you

01:10:42
could just press C on your keyboard and comment it however there's another feature in unreal called collapsed graphs now you can right click and click on collapse nodes and it's going to create a collapsed graph now you can have inputs and outputs here as well but in my experience I have never really bothered using them and let's just call this one my collapse graph and if I go ahead and type in my collapse graph by right clicking so let's say type in my collapse graph you see I cannot call it because this is not

01:11:21
a function this is just all of this code just stuffed into this collapsed graph so I lost my event graph here can head back in or you can click on this way so that's basically a collapsed graph that's about it and when we actually use them you will get an idea you can actually have further execution so let's say I have this so it's going to come out of here as well so stuff like that so I'll go ahead and delete that it's not of much relevance [Music] now that we have studied about functions

01:12:03
macros and collapse graphs let's actually look at implementing the various programming constructs inside blueprint so we'll use the level blueprint again and after this we will get to actually working with blueprint classes now the first thing that you would want to do is do an if check and we already did that several times so if you right click and type in branch or you could just type in if or you could hold down B on your keyboard and left click that's another shortcut which I like to use you would bring up a branch

01:12:35
node so a branch node takes in a Boolean and depending on its value it's either going to go true or false this is an execution pin again so depending on the value of this variable you can go ahead and execute some logic so instead of Health let's say I have B Alive as a variable so if the player is alive for example so put that in so if the player is alive then we are going to go ahead and run this logic otherwise we are going to run this now there's another thing which you can do with booleans

01:13:13
which I probably mentioned for enums but you can actually do a select as well so if I go ahead and select you can go ahead and do this so again you can actually get uh this return value to to change depending on the value of this variable so this comes in pretty handy now this is the most basic type and there's nothing much to explain really so you could go ahead and print something and maybe do something else and if he's not alive maybe you can go ahead and you can quit the game or anything like that so that's basically

01:13:50
it [Music] now the next construct that you'll use is switch now switch is something which we already talked about but we are going to go a bit more in depth now now I'll change this variable to an integer again or rather I'll just undo everything so that we have our integer back okay I saved it in between so we can't so I'll just change the variable type and for this we are going to rename this to let's say health again now I have health so oops let's just compile that again control drag it now

01:14:34
if I drag off of this and type in switch you would see that I get the switch on int node now basically what this means is if I just click on ADD pin and you can also set the start index so let's say you want it to be1 to start with you could do that as well -2 for example so what you're basically saying is if the value of health is one head into this execution pin otherwise default is basically like an else so if none of these correspond so let's say we have 1 2 and three if the health is neither one

01:15:13
nor two nor three it's going to head into default so for example if I just go ahead and print now since our health is zero and we are starting at one we should get hello printed in theory so we get hello if I go ahead and drag off of one you're not going to get anything now the same thing if I just change the value to one I change the health variable value to one now you should get hello so this is how switch Works generally you would be using this with enumeration so for example we have my

01:15:49
enim over there so let's just delete everything in the graph now my enum my enum now if I grab this into the graph and if I then type in switch you see you get the options so if Health okay we can rename that to something a little more descriptive so let's just type in some enum so if our enum if some enum is Apple this is going to be executed if some enum is banana this is going to be executed if some enum is mango this is going to be executed so this is basically how switch works so that's about it actually now

01:16:37
this was for your uh selection and to evaluate [Music] condition now coming to the iterative constructs let's say you wanted to print numbers from 1 to 10 you can use a loop now if you guys are familiar with cc++ these will seem much much easier to deal with there are basically two types of Loop and there is a version of while loop called do while loop so the types are while and for and there is one more type which you use a lot which is for each and we will get to that once we start talking about arrays now if I

01:17:17
right click and type in while you see you get while loop so what this basically means is as long long as this Boolean is true so I can change this to Boolean once again as long as this is true this value is going this Loop body is going to be executed so for example uh let's say uh let's actually make this a number again let's change this let's say we wanted to print numbers from 0 to 10 so i' set the sum enum or we'll call this one num we can set num to be equal to 0 by default and

01:17:57
now we can do an if check as long as number is less than or equal to 0o or rather 10 we can go ahead and print our number so we can go ahead and type in print string and we can just controll D print it out now obviously the this is an infinite Loop you have to change the value of num itself so what I can do is I can set set num to be equal to num + 1 so this is one way to do it also if you were to notice if you just drag off of the s i in Plus+ you can actually do increment as well so this is basically

01:18:42
like your num ++ in C++ that's how you would interpret that now if I go ahead and press play you should see we get numbers from 0 to 10 as expected so that's basically how you use a wi Loop and once this Loop is done again you can go ahead and print something so let's say printed numbers printed numbers now you see it prints from 0 to 10 and it just goes to complet it this is how you'd execute your logic one thing to note though avoid using Loops in your program especially in Blueprint

01:19:21
unless the array length is you know less than about a few 100 it's fine but let's say you're dealing with larger data sets please refrain from using Loops in Blueprint uh try to use as much as you can in C++ because blueprint if I haven't mentioned yet is slower compared to C++ when you call Print string for example this is actually a function call in C++ so the actual function of print string is written in C++ it actually takes a little bit of processing to actually switch between

01:20:00
blueprint and C++ blueprint is kind of like your jvm where it actually runs on a virtual machine so blueprint code is going to be comparatively slow than C++ but in this case this code is pretty simple so you don't really need to do that we will get to where to use blueprint and C++ much much later there's not nothing much to worry about for simple games [Music] now the other type is going to be a for Loop so if I just type in for Loop you see you get for Loop this is how you basically execute your for Loop however

01:20:39
this is a little more or actually much more easier than what you have to do in C++ in C++ you give an initialization expression an update expression uh and a conditional expression I mix mixed up the order but anyways you get the point and you got got to actually give the body of the loop like that but here in Blueprint you just type in a first and a last index which makes it very very simple for you to execute a for Loop and if you were to just drag this in let's say I just type in 0 and 10 and I just

01:21:12
go ahead and print this we don't even need a variable at this point we can just grab this and we can go ahead and run this and it's going to print 0 to 10 so this is how you use a for Loop now there is another variation known as the for each Loop which is used uh similar to range based for Loop in C++ to iterate arrays and stuff like that we will talk about that now again the completed works the same way once this Loop is completed executing you can go ahead and print something or execute whatever logic you

01:21:49
have so this is your for Loop and there is another variant of for Loop called the for loop with break so if I just type in for loop with break you see you get this now let's say I wanted to stop at a certain point let's say uh I mean in this case it's kind of useless to do it but let's say I want it to stop in between let's say I have some logic we can just grab in some random logic uh let's say this number divided by 15 you know uh we have to make this float remember because integer division

01:22:26
works in a different way so let's say this number divided by 15 if it is greater than 3.5 we want to break let's say we have that logic so we are going to print as long as this number divided by 15 is greater than 3.5 so do that if this is true we are going to break whoops and if we go ahead and print this uh we can just go ahead and print the number instead and once this is completed we can print something else now obviously to tidy this up you can use a reroute node and you can do this so this is one way to keep your

01:23:06
blueprint craft tidy so we can type in completed so that's done and we have a compiler error it says so okay we'll we'll take that in as a float so convert this pin to a float convert this pin to a float and then let's just do that and let's compile this again save and go ahead and press play now we would see it's 52 so if we actually bring up our calculator so we get 51 by5 is going to be 3.4 and 52 / 15 is going to be 3466 so that should be the last number so now if I do 53 divided by 15 you see

01:24:04
you get 3.53 which is greater than 3.5 so it did not print [Music] that okay now that we've talked about iterating now it's a good time to head into R for each Loop now for this we'll need to learn about another data St structure now this is a variable right over here where you select the variable type to the right of it you get an option to change it to an array set or a map now an array is basically a collection of homogeneous elements so basically in this case num is now no longer a single number instead

01:24:48
it is a collection of numbers and why I say homogeneous is because I can only have integers in this list I can't have have zero and I can't have a string in the next index so basically each item is going to be referenced by an index so the first item which you put in is going to be zero and stuff like that you can put in any number and if I have to iterate through this I will use a for each Loop now if I go ahead and print this out you would be able to see that I print in all the elements in that array

01:25:21
so I printed in 2 and 32 which is is what exactly what we have so that's basically how it works now one more thing you can have it of any type in case you guys were confused I'll create a new one for example uh let's just call it one St Str array and let's make it of type string and let's compile that and I can go ahead and add a few elements I can I can just type in any set of characters and I could iterate through this as well so I can just drag this in compile that and go ahead and run this

01:26:01
program now you see you can print that as well so this basically stores multiple of the data types elements and one more thing since this is an array this is more of a theory thing but uh the elements here so this string so let's just actually name it 1 2 and 3 for our reference so one is 1 2 and 3 these are actually stored in continuous memory locations so iterating through them is actually a relatively cheap option now unfortunately Unreal Engine does not provide us with a link list structures in Blueprint we have to

01:26:37
implement that ourselves if we need it to but most of the times you'll be using arrays and Maps you will not be using sets or link lists most of the time however it is Handy to use Link list in some very rare occasions but we will not be going over that anyways so let's just delete all of this we are done with this so that's basically your array and your for each Loop now you can have an array of structures as well it's totally fine so I guess we called our my struct if I'm not wrong we could have an array of

01:27:08
those that's about it basically you could store any type of element now I can go ahead and click on the plus icon and I can add the name and points and it works just as you would expect so I can go ahead and delete this we don't need that anymore [Music] now along with your regular if switch and your Loops unreal in blueprints provides us with a a couple of Handy nodes which you might need one of them is called flipflop so what does it mean so flip flop is basically basically this is how

01:27:47
a flip-flop works if this execution pin goes in once a is going to be executed otherwise if you come here again B is going to be executed so let me actually show you what I mean so if I just drag this in and if I print and let's just say a is executed and now if I just go ahead and give in a delay of let's say a a second and if I copy this over and let's just type in B is executed give a delay of a second and again head back over there so I'll just use a reroute to make things a little more clear for you

01:28:31
guys now make sure you guys do comprehend this logic correctly if I go ahead and press play you would see it says a is executed B is executed and it's going to be alternating like that so that's the use of a flipflop you could use this uh for key presses so let's say you wanted something to happen when you press the key once but you wanted something else to happen when you press the key again so for example let's say you have a scoping in uh thing in your game so let's say you're scoping into your

01:29:03
weapon let's say the first time when you flipflop to a you want the guy to scope in and when you flip flop to B you want your weapon to scope out so that's basically one place where you can use flip-flop so it's pretty simple [Music] now one more thing which the engine provides is do ones now do ones and there's also gate node which you might need but I've honestly never gotten an actual use case for this so there's nothing much to really worry about this but it's it can

01:29:43
come in handy depending on your game especially if you're going for you know puzzle type games maybe not really sure so do ones basically as the name suggests it just allows you to execute this one time so let's say I print this string and I go back to this this is no longer an infinite loop it's just going to execute it once look it just executed hello and that's about it now let's say I want to call this function just once again so what I can do is I can drag this into reset so if anything goes into

01:30:20
this reset the function which goes after completed will be ow to execute once again so that's basically how du once works I don't think there's any explanation required for it so if I do it on tick so basically every frame it's going to allow you to do it once again and if I just go ahead and reexecute this I know this is an infinite Loop but we do have a little bit of a duration for us in the tick so that's how it will work okay so it did stop the execution over there that's a different thing but

01:30:52
yeah basically reset is going to let you to do that once again so I can actually get a more practical example so let's say we have a delay of 2 seconds and we do this I can actually use a sequence so sequence remember the node which we used before so after not. 2 seconds I can go ahead and reset that and after let's say not. 5 seconds I can try executing that once again so if I go ahead and press play you'll see it works as a [Music] expected whatever we spoke until now was just the basics in order to get you

01:31:34
started with Unreal Engine but in order to actually practically create a game we need to First go into some background so that we can learn how to use classes and objects now if you guys aren't aware on real engine or any game engine in general is going to be working on the principle of object oriented program a bit of a background here so there are two main programming methods that we'll talk about now the first one is procedural programming so this is the approach used in languages such as C

01:32:06
where basically our approach is mainly using functions so procedures that's what basically procedural programming stands for so you have a main function and you have several other functions now this is the most simplest form of what it could be how however you could have a function over here as well so let's say you have function 4 for example and maybe function 4 can call function two or vice versa doesn't really matter but basically your whole program is divided into multiple functions and there is

01:32:40
some global data on which it operates on so you have some data over here and maybe function 3 accesses some data here stuff like that could happen in procedural programming however the approach which is used in unreal in objectoriented programming language such as C++ is going to be objectoriented programming of course as the name suggests and here we use a principle known as classes and an instance of this class is known as an object so let me be a little more specific here so all the data and

01:33:19
functions so for example or in this case uh this was a method this was the main function so we have one method here another one and we also have some data over here so all of these is going to be encapsulated into a unit known as a class and I will get to some examples later so once we have this encapsulated we can go ahead and create instances of these called objects so basically your class acts as a template for these objects now the first question that pops up in your mind mind would be why do we

01:33:56
use objectoriented programming over procedural well it's pretty simple to explain that so if we look at the wrong approach that is procedural programming you would know that you would have a character let's say for example so let's actually talk about a character which you'll have in a game and how you would approach it with both programming methods so in procedural programming you would have a character character of course you're not defining any unit known as character but let's

01:34:28
say we have a character in a program and you you're going to have several functions so you have move turn jump of course you'll have other functions I just took the most Bare Bones example and obviously you'll have the characters transform and if you guys forgot about what transform is transform is basically location rotation and the scale combined then you're also going to have a velocity for the character and other variables pertaining to your game play however there is one problem which

01:35:00
you might notice we do not have a unit which we can recognize as a character so we have several functions let's say we call the move function for example now when we move when we call the move function we actually have no idea which character we are moving so character itself is not actually an entity so we don't have an actual entity known as a character our program just has functions same with the transform we cannot instantiate another character so this code this entire code isn't reusable so

01:35:40
that's the problem now what if we head back into the objectoriented type so if we head back and if you can see here we have a class and we have instantiated several objects now if you were to actually model a character with this you would have your character class obviously with the above mentioned functions and data I didn't want to rewrite that so you would have a character class and now that we actually have a unit which we can identify as a character we can go ahead and instantiate a character and let's say we

01:36:15
call it character one so we are going to instantiate it so we are going to instantiate it and let's say we have another player let's say an En me so we can go ahead and reuse that once again and instantiate character 2 so now we don't have to rewrite all the functions and whenever we are actually writing code we have an idea of which exact character we are referring to so character 2 is actually a realtime entity and this is known as an object so character one is an object character 2

01:36:47
and character 3 all these three are objects now if you were to remember in our blueprint noes we had a Target pin so if I bring in for example set actor location so I'll just use the same note so set actor location now you would notice there is a character pin now if you were to just hover over it it says actor object reference now in our programming approach what this basically means is we have set actor location defined in our class so let's let's say for example we have something like this

01:37:27
so we have our actor class now anything that can be placed in the level is called an actor so let's actually create that so actor so inside this inside actor you actually have a set actor location method so set actor location I'll not write the whole thing and let's say you instantiate actor one so let's call it A1 for example when you instantiate actor 1 your program needs to know on which actor set actor location has to be called so we have actor one so that is our Target so when

01:38:03
we call set set actor location in our case in a blueprint we call set actor location now it needs to know on which actor it has to perform it so when you call this in the through the target pin in Blueprint that's how you do it in the Target pin you specify that and the program knows that it has to set a1's location so that's how it basically [Music] works all right so it's time we apply whatever we learned just now so head into your content folder and create a new folder and we'll just call this one

01:38:42
Blueprints and inside here we'll create all our blueprint classes and we will compare all of them so basically the most Bare Bones one which you can create is an object now please do not confuse this with an actual object we are creating a class and the class name is going to be object we are basically deriving a class from this object class this is how you basically start in Blueprint however as you proceed further you will understand note that this is not an actor so I cannot drag this into

01:39:10
a level now if as I'd mentioned before Unreal Engine already has a 2d Vector structure but just to Showcase what we can do with such classes let me just actually create a 2d Vector so let's just call this one 2D Vector for example now please note you cannot name a type with uh number beginning in you know uh C++ however you can do that in Blueprint so let me just call this on Vector 2 for example so if I open this up you you would see you have a standard blueprint editor you have an event graph but you

01:39:50
don't have your viewport and stuff like that which you would see in an actor now one more thing you would notice is you don't have an event begin play so you get an option to add a custom event which is basically like defining a function but it does not return anything and you can call it just like a function and we will be using a lot of custom events so you would get an idea of what I mean now in Vector 2 we are going to have two variables the first two are going to be floats so obviously we'll think about

01:40:22
what we can have later on so it's going to be an X and A Y so these are the variables which are encapsulated inside this Vector to class note that this is not an object this is a class and when we actually create an instance of this we create a vector to so that's how it basically works now we don't want this X and Y variable to be directly accessible now the reason I want it this way is for data security now I don't want be directly able to write any random value to X and Y let's say this

01:40:58
was exposed and you could actually change this directly in memory what would happen is now for example let's say I have a vector 2 object so let me just create that so use the construct object function so construct object from class so I think I misspelled that so construct object from class yep there we have it so I'll just delete this and if you go ahead we will get access to our Vector 2 so Vector 2 for example now we have a vector 2 object over here so this is actually a vector 2 object we could go ahead and promote

01:41:41
that to a variable so it's going to create a variable of the type and let's just call this one R Vector now we don't want any other external entity to actually be able to directly set X so this would be prone to lots of exploits basically so that's the reason what you generally do in objectoriented is you make this private you see the option over here called private now basically you will not be able to access X and Y from here so now if I type in get X you see I can't get it if I type in set X I cannot set X

01:42:24
so that's one way of providing security to the data now what if you just wanted to access the value that's pretty simple you would just go ahead and create a function so you type in get x value for example so get X and get Y and we are going to make this pure functions because we are just returning the immediate value and we could add a compact node title and call This One X and we'll call this one y now in the return node we could just go ahead and return the value so return node and we can go ahead and uh grab our

01:42:59
y here and return that and over here as well we can go ahead and return X so grab in the return node and return X so now if you wanted to access X or Y you can go ahead and type in get X so you will get access to the x value however you will not be able to edit X directly so again for that we can go ahead and create Setters so Setters are basically just functions which are going to set the value so let's say I type in set X and I type in set set y I accidentally typed X again so set y all right so once that's said we can

01:43:46
go ahead and take in the value and this is going to be of type float and we can go ahead and set our y to be equal to that and we can go ahead and type in the the return node we don't really need it in this case but anyways we'll have it and in our set X function we could do the exact same thing we could add in an input pin and call this one value once again value and we can go ahead and add in a return node whoops we didn't need that now what if you just wanted to set this entire Vector now when we set R Vector we are

01:44:35
actually just getting a reference to it we are not actually setting our members so we can go ahead and write a function for that again we could get add a get Vector to and we could also have a set Vector too so something like this this was just to show you guys how you would work with classes and objects so for get Vector 2 we can go ahead and actually return the value so we can go ahead and add in the return node and we can get our X and our y so things like that so for a set to we can go ahead and alt track

01:45:27
this alt track this once again now obviously please do understand that this is kind of Impractical unreal already has a struct built in which handles all this for us I'm just trying to show you an example of how you would actually use it so this is how you do it so now if I type in set Vector 2 you see I can actually set its value and the target is R Vector so we are adjusting this value and we could go ahead and write in a few more functions so for example uh we could write a function to print the

01:46:05
vector 2 so print Vector 2 so we can go ahead and type in print string and we need a world context object however it is going to take the outer object by default I believe but anyways in these context what you would want to do with something which I haven't seen much is you would just get the outer object there is a function for this basically the outer object is the object from which this object was created so in our case it's our level blueprint and we can call the print function from there the reason is it

01:46:40
actually needs to know uh where to actually print the string so that's the reason actually so now I can just type in self self refers to this object itself so we can just pass that in now we can go ahead and actually print something so in our case we can get our X and one handy function which you'll use a lot is going to be upend so we can go ahead and type in X for the x value give a space and then print out our X move that over there to keep things clean and we can go ahead and do the

01:47:18
same for the Y as well so we can go ahead and give a space and we can type in y with a colon and we can go ahead and print that so we have our y we can go ahead and convert that once again and we can go ahead and print that if you right click you can actually remove the extra pin so that's an option available as well so now this is how you would do it now if I go ahead and press play obviously we are not calling it anywhere so now now that we have R Vector we can go ahead and call Print Vector 2 so this is going to print our

01:48:00
Vector so this is how it works and obviously we can also test out our set functions so we can type in set Vector 2 and we can just give some random values to this and if we go ahead and print Vector 2 we should get that value so this this is basically how you would work with the most basic type of object now this is mostly useful in cases where you only need some data and methods and you want uh methods basically because in Blueprint you cannot have struct methods so in those cases you would use an

01:48:43
object type so we are not going to be messing with this any further [Music] now the the next type which you will use is going to be an actor now this is probably the most commonly used type and most of the other types of classes which you'll create will also be derived from actor so let me just create that right click go to blueprint class and create an actor it's directly available here or you could search down there so if I create an actor we'll call this one my actor for example now if you are to

01:49:20
notice if I drag this I cannot do that because you cannot place a vector two in your scene right however I can drag my actor and I can place it in the scene and if I hit F on my keyboard I can actually see it now this is just a visual representation in the editor so that you can actually see it however if you hit G on your keyboard to go to game view it actually won't be seen now if you were to open your actor you would see the editor is a little more complicated than your basic object you have three tabs the viewport the

01:49:52
construction script and the event graph where you'll be working with most of the time we will separately talk about construction scripts and we'll also get to the viewp put but of our relevance is the event graph right now and we will talk a little bit more about actors you would also notice that we have our begin play antick which we missed in our basic object type class now if we wanted to have multiple of these actors so let's actually do something practical let's say we have

01:50:23
add a pickup actor in our game so we have pickup actor and it's generally a convention you do something like this bpor pickup because more often than not or here if you see the parent class it says actor right so more often than not you'll actually create another class of your own in C++ so any code that needs to run fast or something you would put that in C++ and then you would derive BP pickup from the C++ pickup actor so that's why it's a convention I usually name it like this so I can go ahead and grab this so

01:51:02
I have BP pickup whoops deleted the wrong thing so I can delete my actor here BP pickup 2 will be created so these two are pickups and both of these contain all the variables and functions which this creates so we can go ahead and edit our blueprint just like how we would usually all right so it's time to dive a little bit more deeper into some of these events and let's actually start writing some practical code so event begin play is called not when the game begins actually that's the wrong way to

01:51:36
interpret it however event begin play is called when this actor is instantiated so for example we have our BP pickup here and since this is placed in our level this will get created as soon as our level starts so it is technically called when the game starts however if I just go ahead and print this and let's just call this begin play you would see two begin plays because we have two instances of our BP pickup however it need not be called when the game begins it is called when the pickup actor is actually created so

01:52:17
when BP pickup is created that is when it is called so let's delete a vector two stuff we don't really need it it now in order to actually create an actor remember that every actor is going to have a location rotation and scale so that's the reason you cannot just create an object because you do need uh certain number of uh default parameters in order to actually be able to place something in the scene so without a location the engine has no idea of where to place it that's the reason actor exists now if

01:52:48
you head back into your level blueprint let's actually give a delay of a few seconds just to show you guys so let's say we give a delay of 2 seconds and in order to create an actor you call a function known as spawn actor so spawn actor from class and over here under spawn transform we could just set that to zero for now it's since we don't have any visual representation it doesn't matter honestly so once that's done we can go ahead and select our BP pickup and we can go ahead and compile

01:53:21
it now if I press play you see begin play is called but 2 seconds later another begin play is called if you guys couldn't catch that I'll give a longer delay begin play and another begin play was called and if you would notice in the outliner you would actually notice another instance being created here so if you are to notice there is another BP pickup that is created so that's basically how it works and tick is called every frame however it it need not be once again so if I just go ahead or I can just go and

01:53:57
reuse it actually so instead of this I'm going to type in tick and now this should be called every frame let's let's only have one pickup actor and let's go ahead and not spawn this so if you want to disconnect pins like that by the way you can go ahead and press alt over here and it's going to disconnect the pin so we don't need that now if you were to notice it's going to constantly print tick so this should be about 200 to 300 times a second on my computer so if I just type in stat

01:54:37
FPS whoops miss that startat FPS it's locked at 120 so it's 120 times a second so if you want to increase it actually you can remove the cap by typing in t. Max FPS space Max FPS give something like 9999 or 1,000 all right so I don't know why I did that now head back into your blueprints under your pickup and under your class defaults you can actually disable your tick so you can go ahead and disable and as you can see nothing's being printed now there's another thing you can actually change this parameter at

01:55:18
runtime as well people don't know this but any and all details which are there in this panel over here so let's say for example I go to my class defaults I will definitely be able to change most of these at run time so for example we have start with tick enabled so we should be able to enable or disable tick at run time so let's actually just type in tick enabled and as you can see there is actually a function which lets us do it so if I go ahead and actually enable tick first of all

01:55:54
and if I go ahead and disable it after 1 second you would notice that tick is being printed and a second later it stops printing tick so that's basically how it works and not only that any and all parameters and you can actually change the tick interval as well let's say it's printing too often you could just set it to 0.5 so it will be roughly 0.5 seconds now as you can see it is not printing as frequently so that's basically one as ECT in blueprints that that is Handy to know because any and

01:56:26
all settings that will be there will be usually uh exposed as functions to be adjusted at runtime otherwise again you have your class defaults where you can actually set them I think whatever we did till now is clear now so we can go ahead and delete this code we won't be using it as of now so now let's go ahead and actually write some code for the pickup itself so let's say we have had an object and we had to pick it up first things first there is no visual representation for the object so let's

01:56:58
say we actually just go ahead and oops we go ahead and press play you would see that you can't actually see anything now if I zoom into this so as you can see you can't actually see this pickup so first of all let's actually add in a model and stuff like that now there is one thing uh the default scene route is not actually required if I delete it I won't be able to however I can actually add in a static mesh now a skeletal mesh is a mesh which contains bones and stuff like that so basically your characters

01:57:36
and anything with animations is going to be a skeletal mesh basically however your models like your pickups and stuff usually are going to be static meshes so that's basically how it works as you use them you will understand so now if I drag this into the default scene route I'll go ahead and delete the visual representation and the static mesh will be replaced now one thing to note when you do this the most high component the component which is the uppermost in the hierarchy over here is called the root

01:58:12
component so for example this default scen root is the root component now when I drag the static mesh this is the root component and if physics has to be simulated related in our case let's actually try that let's make the pickup fall down and follow the laws of physics so in that case we will need it to be the root components so that's one thing to note now if I go ahead and select a mesh so for example I can just select this random sphere that we have I think it's way too big so yeah we got to adjust that now I can

01:58:47
go ahead and enable simulate physics so now if I go ahead and press play you see that it falls like you would expect so we basically simulated physics now we have a visual representation now how are we actually going to pick this up now actually let's select something a little more smaller because I don't think this is convenient okay this seems like a reasonable size so if we go ahead and press play we are simulating physics so absolutely no problem with that and one thing to remember in case you are not

01:59:28
simulating physics make sure you do have collision and stuff like that uh if you uh if we actually encounter such an issue I will go ahead and show you guys how to deal with that so we have physics now now we can go ahead and set up some logic now we want to be able to pick this up when we overlap it let's say for example so we can do on actor begin overlap AP so what this says is when another actor overlaps this actor so in our case it's going to be this when it overlaps this actor we can go ahead and perform some

02:00:06
logic and Unreal Engine has set this up for us now there is one problem though this is just our Cube which is our model however we don't have an actual bound so our code won't really be able to know know when to actually call on actor begin overlap so even if I disable Collision so the way you do that is you can head over here and from physics actor you could go ahead and change it but we do need physics so we can't do that even if we actually bump into this you won't really notice anything happen

02:00:42
so if I go ahead and bump into to this nothing is really going to happen now if I actually go ahead and create a bound so the way you do that is right click or rather go to add and you can type in uh sphere I believe sphere Collision yes so when you create a sphere Collision we could call this one bounds you would have created a sphere and you can't see that because the size is too small can go ahead and increase the sphere radius now these are our bounds so as soon as we enter this our on ACTA begin overlap

02:01:16
will be triggered so we can go ahead and print it and if you were to notice the Collision preset over over here under the details panel select this and head into your Collision preset you see it says overlap all Dynamic and obviously if you select custom you can go ahead and edit each Channel and we will talk about this later so if I go ahead and press play you see we get hello every time we overlap [Music] it now hello is going to be printed every time any other actor overlaps this however we want to print hello only if a

02:01:55
character overlaps it and it need not be a character as well now in unreal character is actually a derived class of another class known as pawn and I will talk a little more in depth about this right now so basically this is how it's laid out in unreal basically we are looking for a pawn and I will get to that in just about a minute so we can type in pawn and if you were to scroll down you would see cast to pawn so cast is another programming feature now if you were to feed in an object to this

02:02:32
you can check whether it is a pawn object so now if I go ahead and print this out now uh you would go ahead and actually get hello just normally the reason is when you are actually controlling your camera over here you you are actually controlling a pawn actor anything that can be possessed by a player controller is known as a pawn and we will talk a little more in depth right now and just to clear your doubts on whether this logic actually worked let's say it wasn't a pawn so which means it's not a

02:03:12
player basically so if I copy this over and instead of hello let's just print not player and now if I go ahead and play you would see you won't get anything and if I overlap it it says hello but if I go ahead and copy this over and let's say keep it above this and if I press play you see you get not player printed that is because the Box overlapped another box or rather our BP pickup overlapped another BP pickup however those are not characters so this cast right here failed because the

02:03:52
object which came from this actor begin overlap was not a pawn hence we got not player [Music] printed now since we are still at the beginner part of the course I'll just tell you guys the most basic form of inheritance hierarchy which is there in unreal however once we get to the more advanced part I will tell you guys more in depth but as far as what you guys need to know so at at the base level the most simplest typee of class from which you can instantiate objects is known as object in Blueprint so object is the

02:04:30
simplest type and from that the most basic one which you can create is going to be an actor now an actor is basically an object which has a transform and can be placed in the level as you would have figured by now now under this you have various other classes however for the most basic level we are going to be considering only to so there are many more and we will talk about many others once we actually come to the advanced part but these are the two which you do require to get up and running so the

02:05:04
first one under this is going to be your controller so a controller as the name suggests is a a class which has functionality for your buil-in to take player input and stuff like that and under controller you also have a special type known as a player controller and there are others such as AI controller so you have a player controller so player and I'm just going to put this so player controller now a player controller is basically a a controller which belongs to an actual player you also have other

02:05:43
things such as AI controllers which is assigned to CPU players basically so if you you have enemies in game for for an offline game or something you would assign an AI controller now another class that you'll need is pawn and that's what we talked about so this is called Pawn now a pawn is basically a class which is an actor obviously and can be placed in the level and note that you cannot place a controller in a level although it is derived from actor it is actually an exception controllers player

02:06:17
States game states there are a few other classes which are exceptions and you can't place them in the the level however pawns can be placed in the level and a pawn is always possessed by a player controller so a player controller is going to be possessing a pawn so when you call the possess function and you give the target as a pawn you are going to be possessing the pawn and one special type of Pawn which has a lot of functionality built in for us already is called a character most of the times you

02:06:49
will be working with characters and not Pawns however you can use puns so by character I mean a character such as a living being basically so generally if you have like a human or if you have like an animal or something like that you would generally use characters however if you have something like a vehicle you would usually stay away from characters because it has some properties which are not realistic for those however it is completely possible to use a character class for something like a vehicle as

02:07:21
well so so you can possess a character as well there is no harm in that pawn or any derived class of Pawn can be possessed by a player [Music] controller since we have the basics in order to get us started we can go ahead and actually create our own character class or I should rather say Pawn class which is also a character class in our case so we can create that as well as a player controller and and I'll show you guys how to set those and how we can go about interacting with this pickup using

02:07:58
those so right click go ahead and create blueprint class and as you would see you have character and player controller right here because they are really really common so type in character and let's just type in bpor character again you can you can name it appropriately or as per your wish now if I go ahead and open it up you see this looks a little more different and it already has something set up for us and some of these are quite handy especially the character movement component which is there and if I haven't mentioned yet

02:08:34
whatever we did here under the components tab these are called components basically basically every actor is made up of several components and you can actually create your own components as well and make them behave as you wish but as of now just know that these these are just constituents of these this actor and these are the constituents of BP pickup and this is these are the constituents of BP character basically now we haven't set a mesh and we don't really have one so let's just take okay we have a character

02:09:11
tutorial TPP and one thing to note this Arrow actually represents the forward direction of the character so you can go ahead and move it down and you can go ahead and rotate it 90° so let let me have snapping enabled so rotate it by 90 and you can go ahead and bring him all the way down until I feel it's correct now we don't have any animations but I'm not really sure if we do have an animation blueprint for him so let's just check tutorial animation blueprint I guess tutorial 2p animation blueprint

02:09:49
so yeah we do have an animation blueprint for him now if you want to change the default character that you'll be using the way you'll do that is by first of all heading into Window World settings make sure that is enabled and then over here on the right hand side head into World settings and under game mode override you can go ahead and set your own game mode now if I were to just select game mode I still cannot edit it so I will get to Game Mode classes later on because they're not that important

02:10:21
but for now you can just go ahead and create a new game mode and it could be of type game mode base or it could be of type game mode it doesn't really matter but I would suggest sticking with game mode base and let's just call this one uh bpor game mode uh I just did something there so yeah bpor game mode that's what we'll call it and now under this we will get our option to select the game mode now since this is our custom o custom made game mode we get the option to select the default Pawn class and over here we

02:10:59
can select our BP character and if I save everything and if I go ahead and press play you would see that we have indeed possessed our character and you were to notice that the camera is a bit off so what you can do is you can actually create a camera if I go ahead and type in camera under the comp component section you can create a camera and you can align it as per your requirement so this should be about correct so I feel rotating this a bit maybe a bit back maybe a bit to the side would be nice so there you have it so

02:11:40
this is our character however we are not actually able to move the reason is we haven't actually written the code for it to take our input Now setting up input in unreal is really really easy and I will show you guys The Brood force method as well as the proper way to do it so The Brood force method is for example we want W to be able to make us move forward so you can press W and if you just give a space and type in keyboard you would be able to get W and we can make the character move forward so in order to make your

02:12:17
character move basically there's a function for us built in all already under the character movement and not character movement I believe it's there in our Pawn class I believe or a character class so if you write click and type in add movement input so it's written in our Pawn class we can go ahead and make him move and if you were to notice we have to provide a direction and a scale value scale value is useful if you're on a joystick or something where you can partially press down so let's say you're

02:12:50
halfway pushing the joystick uh knob so in that case it would be 0.5 so the scale value can be given through an axis value now if you were to notice uh there is another problem here when I actually plug this in it's not really going to work as you would expect so for our direction we need the forward direction of the character so a very simple way to do that is typing in get forward Vector so get actor forward vector so get actor forward Vector so that's the way you would actually get the world Direction that's how you would

02:13:27
do it and if you were to notice it's not going to work as expected at all the reason is this has to be called every frame in order to actually work so the way you do it is Type in uh or rather we can do it on event tick for example so if we go ahead and do it on event tick I'm just doing this to show you guys how to do it if I do this now we would see that our character is moving forward now the most obvious question is how am I actually going to set this up so there is something known as an axis

02:14:06
mapping which runs every frame basically what add movement input does is it moves you a very very slight amount and by calling this multiple times in a single second you are going to be adding considerable amount of movement now if I head into my project settings and under input this is the right way to do it the brood Force way would have been like doing this on tick and I'll just show you this really shouldn't be your option but I'll just show you just in case so for example we could just have a Boolean

02:14:38
here and we could just set this to true for example and when you release it we could set this to false now this is wrong so don't really worry about the logic this is just going to work but you shouldn't really do this so we could do if new variable is true we want to move otherwise we don't want to do anything so if I go ahead and press play I can press W and move but as soon as I release it I'm going to stop this is the Bro Force way to do it but unreal has a much more elegant system to

02:15:08
do it so we can go ahead and delete all of this head into our project settings once again and under input you would see action and access mappings now we want an access mapping because we do want to be able to control the scale and since add movement input is actually a function which depends on the scale value so remember what I told you about the joystick so we can create an a axis mapping so for things such as jump where there is no scale value so it's either jumping or not jumping so wherever you

02:15:42
have a toggle you would have an action mapping wherever you you have some value which goes linearly would have an access mapping so we can call this one move forward and make that Pascal case and we could have W on the keyboard for that and again for move backward we could reuse this actually so s is going to be move backward and for the scale value you can make this negative 1 now if I right click over here and if I type in move forward you would notice that we have an axis mapping so if I grab this into this

02:16:26
input event or rather if I bring this into this axis move forward event and for the scale value if I put this under axis value now this will work exactly as I would want it to so if I go ahead and press W it's going to work and even s is going to work now for us so this is basically how you do axess mappings similarly you could do it for move right so we could have move right or we could call it move sideways and we' have our A and D keys so we have our a key and we have our D key so D is going to

02:17:04
be this one and it's going to be negative one so let's actually just test it out so it's not really doing anything because we didn't set up the logic obviously so move sideways whoops axis move sideways so once you have the event setup you can go ahead and add the movement input and again you can get the right Vector of the actor so basically the right direction of the actor is going to be your right Vector so your forward Vector is always in this arrows Direction and your right Vector is going

02:17:45
to be a vector in this direction basically so right vector and if I go ahead and press play so it's always one so that's the reason it's happening so if I plug that into the axis value I'm moving reverse actually right now so that's just a simple mistake I did here so I can type in minus one for this and I can type in plus one for this now everything should work as expected so if any of your directions are reversed just multiply the axis value by minus one now as you can see we are able to move forward left

02:18:20
right and all of that good stuff now that is about it for the keyboard input however if you were to notice I really can't rotate the character so let's actually set that up first so first things first head back into your BP character and the functions which we require to set up keyboard input I mean Mouse input for a character is going to be your controller pitch input and your controller your input so controller pitch input and controller your input so these are the functions that we need now again since our Mouse needs to

02:18:59
be captured as much as possible because it it has to detect every tiny movement so we again need to create an axis mapping so go ahead into inputs and create two new access mappings and call one look around and the next one call it look up and for this look around is going to be the x axis of the mouse so type in Mouse X and for this one type in Mouse y so that should be good and over here if I go back and if I type in AIS AIS look around and we can go ahead and add your input over here and over here access

02:19:57
lookup oops I missell that so head back into input so look up now if I go ahead and compile this and press play you would see that I am able to look around however I really am not able to you know look up and down that's mostly because your character isn't really meant to rotate along with it so that's the reason it's happening so if I head into my camera and enable use Pawn control rotation and if I press play you see I am able to rotate my camera however there's one small problem here we are

02:20:48
again uh doing it reverse so again in that case as I told you guys before just change the scale value to1 now if I go ahead and press play you would be able to see that our camera is working as expected now there is one slight issue though that is uh our view is kind of off which you can fix but when we actually look up our character doesn't seem to be looking up but the the reason that's not happening is because you can't just rotate the whole character now if I were to actually go to this uh main tab over

02:21:29
here under BP character and if I search for control rotation so if I type in control rotation and if I enable it to use pitch you would actually see that I am in fact able to do that but there is a small problem now if I hit f8 to unpossess my character you see he just rotates like that however we want only his spine to rotate and that is something which we have to set up using an animation blueprint which we will do later so for now we'll just disable this and even for the Y part you could you

02:22:04
could disable this and you could technically do something like this and maybe set up some other logic in order to actually rotate your character but for our purposes we'll only do it for the pitch another tiny thing that I would love to to cover here is how do you actually set up different sensitivities because obviously right now the current sensitivity may be a little too much for some for some maybe it's a little too less so the way you do that is you just multiply this axis value by your sensitivity value that's

02:22:41
basically how you do it so multiply this and multiply this as well press contr D to duplicate that now we could just promote this to a variable however remember that this BP character refers to only the character which we are playing so let's say we we are playing a death match or something where your character dies and you respawn with a new character you would have to pass in the variable every time so instead of doing this we are going to set this up in a class which will be common even when your character is

02:23:17
destroyed so the class which we'll use and as you would expect is called player controller so go ahead and create BP player controller so make sure everything is in Pascal case now if you open this up now over here we can go ahead and create a variable and call this one sensitivity and now uh this is going to be of type float obviously and let's make this one private and let's create a method to get this sensitivity now this player controller is going to be persistent even after your character dice so that's the reason

02:24:01
we using it and since we need the immediate value this will be pure and for the return value we are just going to return the sensitivity now obviously the reason we doing it this way is you don't want an external entity to actually modify sensitivity that would be crazy and one more thing make sure you set this value to anything other than zero cuz if it's zero your mouse obviously will not move so maybe something like 0.5 so once that's done I should be able to set my player controller first of all

02:24:35
over here in your game mode override for your BP game mode go ahead and change your player controller to the one you created save that and open up your BP character and now on begin play what we can do is we can actually get our player controller so we can type in get player controller and we can cast this to our as you would guess BP player controller so we are getting our player controller and we are checking if it is a BP player controller obviously we set it over there in the game mode so it will be

02:25:10
there is no there's no way it's going to head into cast failed so we can just right click and make this a pure cast so this just helps us save some space in the graph this will be a success for sure and we can go ahead and type in promote to variable and we'll call this one PC ref for player controller ref now go ahead and compile that again you can go ahead and make this one private but honestly it doesn't matter in this case so on begin play we have gone ahead and stored our player

02:25:41
controller and from our player controller object we can go ahead and get the sensitivity go ahead and get the sensitivity go ahead and do the same thing over here compile that and if I go ahead and press play you would see our sensitivity works and not only that actually if I go ahead and change the value so let's say I make this 01 or rather 0.05 for example 0.01 would have been too less now as you can see I can make very precise movements so now this sensitivity option definitely works so this is how we would

02:26:20
actually go about setting up sensitivity obviously if you really didn't care you could just have a variable here and stuff like that doesn't really matter honestly and there's another thing which you could do is first on begin play itself you could go ahead and pass your sensitivity over here and you could promote this to a variable over here and instead of calling the function every time and make this one private once again instead of calling the function every time you can go ahead and use the

02:26:54
sensitivity variable so that's a little more better in terms of performance this is something which you could do as well now remember we are only able to do this because the player controller is always created before your character spawns let's say your player controller is not yet created by the engine you can't actually do this so let's say I go to my player controller and I'm not sure if I can do it on begin play maybe it would work on begin play but technically if I type in get player

02:27:28
character and if I type in cost to my BP character and if I go ahead and print the string copy that over and I'll just type failed for this and doesn't matter to be honest and I'll type in success ESS now if I go ahead and press play you see we get success however this happens only because our player controller is probably created or rather the begin play is actually called after the character is created as well however now I'll just show you guys another class now we'll discuss more in depth about

02:28:13
this but if I just type in game instance I can go ahead and create a game instance class and this is actually referring to your your whole game application so if I type an event in it this is when your game starts this is It's not like the begin play where you are actually you know talking about when this entity is created the event in it is actually called uh act when the game starts so that's one difference so oh here if I go ahead and put this logic over here and if I go ahead and go to my

02:28:49
project settings and change the game instance game instance to new blueprint we'll delete that soon and if I go ahead and press play you see it says failed because our character is not yet created so that's one thing to note the the begin play logic only worked because our character was already created now let's say we added a 2C delay now this is going to work so now if I do this it's going to work because our character is now successfully created so that's basically one thing that you

02:29:22
guys need to understand just make sure all your entities are valid before you actually set them and we can go ahead and revert our game instance so again we'll talk about all of this more in depth this is not something which you would really worry about at a beginner level now save everything and that should be good to go to go a little more in depth on the part where you know you would actually check if this object is created so in our case I mean everything just worked out smoothly but what if it

02:29:54
didn't what if this wasn't valid yet because as I told you guys the default value is none what if this wasn't valid well there is a fix for that as well there is actually a function called is valid so if I go ahead and type in is valid there's actually a macro which is created for us so what we can do is we can go ahead and actually do this so if we we can convert this to a normal impure cast so on begin play we can go ahead and do this we can check if it is valid and if it is not valid we would not want

02:30:34
to do anything but uh I mean if it is valid we want to set the reference obviously uh but if it is not valid we want to again check after a while and if it is valid obviously uh after setting the reference you would want to go ahead and set the sensitivity and do the regular [Music] stuff now what if it's not valid now how do we actually check once again so for this you would use a technique known as polling so polling is where you repeatedly call a certain function until a certain condition is met and you

02:31:14
actually get your desired result so the way you can do this is by using a timer and that takes us to the next next important concept now if I right click and type in set timer you would see you you would get a few notes over here however the only one which you'll use is set timer by function name set timer by event is kind of pointless in my opinion because even if you do use this you can actually refer to an event by the function name itself so most of the times you would be using set timer by

02:31:47
function name so use set timer by function name now it returns as a timer handle which allows us to control this timer and what this basically means is it is going to call the function with a given name so we can right click on this and type in collapse to function and let's call this one for example get references or let's call this one initialize and we don't really need this in the event graph and over here we can copy over this name so what we are basically saying is after certain time call this function once

02:32:25
again so we can have a very small time such as point1 seconds and make this one looping because if you just uh set this to0 o1 without the looping it's just going to execute it once and we can go ahead and store the handle of the timer so we can call this one initialization timer and once we have that this timer is now set and we could just comment it out and call this one polling for references again you could name it a little more descriptively you could give it a color as well that's one cool

02:33:03
feature in unreal honestly you would never use it but yeah I just showed it and under initialize we need to stop the timer once we actually finish everything so once we finish setting the sensitivity there's no reason for this function to run again so we can go ahead and get our timer handle first of all and if you just type in clear You' get an option called clear and invalidate timer by handle go ahead and call that this is how you stop the timer copy this and if it is not valid we don't really want to

02:33:37
do anything and if the cast failed again we don't really want to do anything so again yeah this cast is bound to fail actually this uh check is kind of useless in this case so we can just go ahead and do this because if we don't have a play controller this cast will obviously fail but anyways I'll just keep it like this and now if I go ahead and run this what will actually happen is every 01 seconds it is going to repeatedly call the function until we have cleared it so once we get all the

02:34:14
references we go ahead and clear the function I mean clear the timer there are some key differences though between doing this and using a delay obviously you could have done this as well so you could have done delay and let's say we gave 0.01 once again and over here we can go ahead and call initialize and we can go ahead and loop this obviously we can call this first so initialize then after 0.01 seconds we could do this and maybe we could check if we have all the references we could maybe return a Boolean over here or

02:34:47
something and do something like that the difference between a delay and a timer is that a timer is going to be very very precise it is going to be precise usually up to micro or even Nan seconds if you have a precise timer this one I believe is precise up to a couple hundred microc so as far as my testing is concerned you could use Chrono in C++ and actually test it so this is going to be accurate however a delay is going to be very very inaccurate so that's one thing to note if you want something to

02:35:19
time accurately you would use a timer or in our case we needed the looping functionality so that's the reason we used the [Music] timer since we have built a fundamental idea on how inputs work now we can go ahead and check the other type of input that is input action mapping now before that let's actually just uh clean this up a little bit so just comment it out and and type in movement movement and maybe you could type in movement and Camera maybe so movement and camera so now we can just group these

02:36:02
now head back into your project settings and under input again if you look at action mappings you can go ahead and add one and we can call this one interact and we could set that to the F key now the advantage of using it through the project settings like this rather than brood forcing so you could do F over here as well so if I just type in F and give a space and type in keyboard I can actually do this but this is not the proper way to do it because this uh these action mappings can be actually changed through your in-game

02:36:41
settings menus so you can actually create a menu inside the game and allow the user to change or allow the player to change these key bindings so we'll call call this one interact now so action event interact and this gives us a pretty basic press and released option so when we actually press it so we want to be able to pick up an actor now how are we going to actually set this up so first things first remember we had our actor begin overlap instead of doing it here it's always advisable we do it from the

02:37:19
character so do your actor begin overlap here actor begin overlap once you call the actor uh begin overlap oh here for the other actor instead of casting to a character since we are the character ourselves here because we are inside the character class right now we can cast to the pickup instead now that we have casted to BP pickup we are checking if this is actually a pickup now there is a better way to do it using interfaces but that is a much higher level concept than casting but I will definitely get to

02:37:58
that a little later in this course so we'll probably change this to use an interface even that is casting at the very fundamental level but that's a more elegant solution to do things now if this is actually a pickup we can go ahead and actually store it so promote to variable and let's just say let's just call this one nearby pickup nearby pickup and what we can do is on our actor end overlap so end overlap over here we can go ahead and again cast it first things first and if it is we can check if it is equal to the

02:38:43
nearby pickup and if it is equal to the nearby pickup and we have left its bounds we can go ahead and remove it and invalidate the reference so we can alt drag it and we can set it to be equal to none that is going to invalidate our reference so that's about it now once we have our reference what we can do is we can head in our interact function check if this is valid one more way you can do it is by right clicking and converting this to validated git so if our pickup is valid which means we are near a

02:39:19
pickup so what we can do is we can actually call a function for now let's just print out a string let's say so or rather we can just destroy it so type in Destroy and you will get destroy actor if I go ahead and press play and if I go close to it and if I hit interact you see I destroy the pickup and if I do that once again that is not going to work the reason is once our pickup is destroyed it's no longer valid so what we have to do basically is check once again if we have any pickups nearby so

02:39:54
that's actually really easy to do so once we destroy it we know that our nearby pickup isn't actually valid so we can go ahead and set our nearby pickup to the nearest one now how do you check that again using a function so we want to see if we are overlapping so type in overlapping and you already see you actually get options for get get overlapping actors which is exactly what we need and for the class filter it's obviously going to be BP pickup and over here we get an array of actor

02:40:31
references instead of getting all of them we can just get the first one this is an array so obviously we have to get the first index of the array so once we get that we can go ahead and cast this to BP pickup once again and it is going to be sucessful all the time so we can just make this a pure cast because we are actually using the class filter here and then we can go ahead and set the nearby pickup so now our logic should work for both the pickup so if I hit f one of the pickups got destroyed so I shouldn't have moved back

02:41:12
actually so if I press f one got destroyed if I press F again the other one got destroyed as well and there are no errors so this is basically how you do something like a pickup now obviously before you destroy it let's say you had some properties let's say for example let's say this was a health portion or something which gave your player a couple of Health points so we can add in I don't know let's say health points obviously you'll have a better inheritance hierarchy and we will get

02:41:47
into that so Health points make this a float let's say we have 10 so what we can do is for now we can just go ahead and print it so we can grab this health points and we can just print it out so move all of this logic a bit over there to make space we can just print that before destroying it make sure you call Print before destroy otherwise you're going to get a log error now if I go nearby if if I press F we are going to get 10 printed every time so that's basically how you do [Music]

02:42:31
it however let's say you wanted to change some of these properties depending on which pickup it is now apart from having these as a variable you can go ahead and check these two options called instance editable and expose on spawn what these will do is allow us to edit these properties when we actually spawn it so let's say we spawn a pickup for example so over here let's say I do spawn actor let's say we spawn a pickup you see we actually get an option to change our health points so we could

02:43:13
do something like 90 for example and for the spawn transform we can just uh get a random location let's say uh let me just add in something for us to recognize so something which you would use for such a case is called a Target point so you can use a Target point so this will represent a tar a point in space you can copy this over and we can go ahead and paste it in or okay maybe we can't do that here you can do it in the details panel so 1150 and negative whatever this value is and 6 50 so

02:43:52
650 and we have health points set to 90 over there now as you would see we actually spawn another pickup now if I go ahead and pick these up you get 10 but when I go near this I get 90 however it need not be restricted to spawning it through the blueprint you can actually edit expose on spawn variables right here as well so even when you're placing them in the level you could have this to be 20 for example so if I go nearby you would see 10 20 and this one is obviously going to be 90 so stuff

02:44:31
like that which you can do using expose on spawn you can expose any variable on spawn and they will be passed right into the actor and the value which you pass in would be set to that variable and now we can go ahead and remove this logic that was just for showcasing purposes and we can go go ahead and uh collapse the to function and call this one whoops call this one pickup and along with this maybe we could also have something like door open or something let's say this is not valid we could go ahead and perform door open

02:45:08
or something like that we could go to the return node and we could have a sequence node here so first we would check for a pickup and we could also do something like a door open or maybe anything else probably maybe if you had some sort of an interaction system with the player or something so you could interact with the other player stuff like that which you can do using these input bindings and using the overlap [Music] events to Showcase that let's actually do one more of the interaction events

02:45:48
now I will show you guys how to do it the better way with interfaces letter but this is The Brood Force way and if you have maybe one two or maybe three or not more than four interactions you could use this method itself the one which we did with casting so this is totally okay for small things now let's actually do it so right click create a new actor and let's call this one interaction actor maybe we could just uh nudge it or something so let's say we H we have another static mesh make that the root component and we

02:46:26
need some sort of bound so sphere Collision maybe and for the mesh let's just take a cone for example and also I've gone ahead and uh deleted the code which we had inside BP pickup since we are not using it and over here go ahead and simulate physics make sure you don't forget that and we can go ahead and and okay maybe we can have a smaller one for example so I'm not really sure I'm just looking for any mesh that's available to us because we haven't imported ours okay

02:47:03
this is way too big okay this sphere seems like a reasonable size we can go ahead and increase our bounds that's about it and once again oh here we can head into our BP character and and what we can do is we can copy over the same logic so instead of nearby pickup we are going to have something else so if this cast fails so if whatever we are nearby is not a pickup we can check if this is actually an interaction actor so we can do cast to interaction actor and again other actor is what we are checking if it is the interaction

02:47:45
actor we can go ahead and promote this to variable and call this one interaction actor again I prefer going with Pascal case all right now when we actually go away from it we can again do the same cast so we can copy this over we can paste it and for this actor if it is equal to the interaction actor which we were nearby so copy this over grab in the interaction actor if it was in fact the interaction actor then we can go ahead and invalidate it and set that to be equal to none so that should be about it now over

02:48:35
here in the interaction logic we can go ahead and check if this is valid right click convert to validated get so if we are near an interaction actor uh what we can do is we can instead of drawing let's actually add impulse so add impulse so add impulse so in so we want to add impulse to the root component here which is simulating physics basically these are the physics functions you have impulse Force torque and all sorts of stuff obviously you could spend some time and study those but we'll not get into that

02:49:16
so we have sphere here so static mesh is the root component so we need to get the static mesh if I go ahead and scroll all the way down I should see get static mesh now this variable refers to the component even components are objects so you can just get them as variables and for the impulse what we can do is we can go ahead and get the forward direction of a character get forward vector now you could change it according to your this is logic based so nothing much really and we can multiply this by a

02:49:56
certain value so we can make this one a float and change this to a float make this let's say something like 10,000 something big maybe get actor for Vector multiply that by 10,000 and that should be good to go now we can collapse this to a function and we can call this one nudge ball or something cuz the sphere looks like a ball so nudge ball maybe and if I go ahead and press play okay we have a compilation error so we can check what's that so it says let's read the error first of all

02:50:41
okay it was just uh it just compiled it in the wrong order it compiled character before this so it didn't know what static mesh was now we should be able to go ahead and play this and first of all we don't have an interaction actor let's actually create one go ahead and press play now if I go ahead and bump into this oops I shouldn't have bumped into that if I press F on my keyboard when I'm overlapping it uh the bounce is a little too small let me just increase that so increase the radius don't scale

02:51:19
it up and one more thing if you want to see the bounds just for testing purposes you can set this flag called hidden in game to false so now it is going to be visible in the game as well so if I look around yeah there we have it so we can enter our bounds and now if I press F on the keyboard you see we actually nudge it so the force is way too small so I can go ahead and make this something like 50,000 let's say so if I go ahead and press F4 here you see we are actually nuding it so this is the way you would set up

02:52:00
interaction using casting obviously you can use interfaces to simplify things a little bit but yeah this is the basic [Music] idea all right so in order to understand whatever I just told now in case it went above your head please do Tinker around and try some of the functions yourself using the context sensitive and the and the search bar basically so when you right click and let's say you drag something off of this you can go ahead and type any random function so for example if I just press a you get a

02:52:40
bunch of functions maybe you could have a look at all of these maybe have a look at documentation and maybe try out some of your own logic and try out something else maybe add in another actor to do something else which maybe add in a door and make it open or something so you guys should be able to try it out yourself and once you are actually done with that now we can go ahead and talk about the next part now until now we talked about the basics and I'm pretty sure you can write some basic

02:53:13
game logic with whatever we have done already but there are a couple of functions which the engine provides us which is going to make our job a lot easier the first one and one of the most commonly used ones which I would like to talk about is Ray casting now if you guys are familiar with other engines you guys would know what a raycast is but in Unreal Engine you call it a line Trace so if I right click and call line Trace so you see you get a bunch of options the one you'll use most of the time is

02:53:43
line Trace by Channel multi is basically used when you have penetration and stuff when you are detecting multiple hitss in the same line I'll I'll tell you guys what's line Trace first so line Trace is basically a function which lets us draw a line from a given starting point to a given ending point and in between these two points if you're actually hitting anything you are going to get it as a hit result so I can get access to the hit location and in case you want to see the line itself you can uh change this

02:54:17
draw debug type enum and make this for duration and if you guys wondered this is an enumeration that's the reason we getting these options so none for one frame for duration and persistent are the enumerators so if we select for duration we are going to get uh the line for some time persistent means the line is going to be shown to us forever until you close the game of course so let's actually do something with this so let's actually set up an input event let's say when we click our left Mouse button so

02:54:51
we can type in left Mouse now I'm just setting this up bro Force because I don't really know what exactly we are going to set up once we actually get to the examples we'll do that now for the start location you can choose the camera's location of the player because this is where you would be seeing stuff so you can select the camera's location for example so if I go ahead and and get the start location the way you do that is there are a couple of ways you could do this and you could do get location so

02:55:29
you can get get World location and you could use this as a starting point and the way you would go forward towards the center of your screen is going to be first of all by getting the forward Vector so you can get the forward Vector of this camera and multiply this by a certain value Again by a float uh we'll do that add that to the starting location so starting location plus forward Vector into a certain number of uh certain number that is going to be your end and we can go ahead and change this to a

02:56:09
float and we can do let's say 50,000 I mean the number is arbitrary obviously unreal uses s CM remember that so anything that you type in will be in cm so 50,000 cm is going to be divided by 100 so it's going to be like 500 M now if I go ahead and Press Play If I press my left Mouse button you see you get a line drawn over there so if I press f8 you see I can actually see the line which was drawn so the red thing which you see that is the line which was drawn and as you can see uh where where

02:56:48
it hit the surface it actually registered a hit and in order to show that there is one more thing which you can do actually Oh and about the other options Trace channel is something we'll talk about later but basically you can do stuff like uh ignoring several uh types of objects so let's say you had uh a shooter game and let's say you wanted to like ignore teammates you could use it for that but you would use tags for that as well but there are several other use cases camera is another thing depending

02:57:21
on what type of objects you want to you want the hit to detect you would do that and actually if you were to notice if I select my mesh and if I scroll down to the Collision part so I'll just type in Collision instead of searching for it like this so Collision you are to notice it says character mesh for the preset and over here if you see there is actually visibility and Camera so what you can do is you can actually make it block certain things so now let's say I wanted this line Trace which

02:57:57
is using visibility right now to block it I would have to change this to custom and make this one block visibility so then I would be able to I would be able to make this line block it stuff like that which you could do now obviously I'll change it back to character mes we didn't do anything but still so over here change it back to character mesh and let's say you want it to ignore the camera Channel you could do that as well now let's say you wanted to just Mark the place where you actually hit so

02:58:34
now we have access to the hit location so there is a function called Draw debug sphere you can actually draw many other shapes but sphere is the one which you'll use most often and the center is obviously the place where you hit it so out hit location and radius 100 maybe we can have 10 seconds for the duration and thickness let's just say two units line color let's set that to maybe something like a greenish yellow or something now if I go ahead and Press Play If I left click you see it's drawing a sphere

02:59:09
where it actually hit it and you could change some of the properties let's say you wanted a more uh detailed sphere I don't know why you would want that though and maybe reduce the radius of the sphere you could do that as well so as you can see we are registering a hit over there so that's what it's basically showing us so this is how you do a line Trace basically you draw a line from one end to the other and you can detect hits obviously for shooting a weapon and stuff like that

02:59:38
you use it now there is another way you can actually determine the start and end location now whatever logic you have here is fine if you only have one One camera but what if you had a first person view and a third person view for example let's say you had two cameras you cannot check which camera you're using and stuff that would make the logic complicated so the way you do it is you would use a function called get player camera manager now this is going to get the current camera which you're using and

03:00:11
it's going to be an actor so we can just type in get actor location and and this is going to be your cameras location so let's say you switch between cameras this is going to work universally regardless of which camera you're using however since in this logic we are using this camera's reference let's say we had another camera this logic is not going to work it is going to work with respect to this camera so instead of this I can go ahead and replace it and we can get the actor for Vector

03:00:46
again get actor forward vector and we can replace this by this and we can go ahead and delete it and the rest of the logic Remains the Same obviously and now if I were to press play you would see that the logic does not work okay we didn't plug it in so the actor location is going to be the start of course not zero press play and the logic works exactly the same one more thing you'll notice is that the line Trace is going exactly to the center of our screen if you were to notice that's one more thing the reason

03:01:23
it's happening like that is because we are going from the center of our Viewpoint and going exactly forward to the view so that's the reason it's actually going right at the center of the screen and if you had a Crosshair in game it would land right at the center so this was Ray casting there are many other options as well such as hit actor so you can cast it so let's say we cast it to pickup for example so we can check if we actually hit a pickup so if we actually did hit a pickup what we can

03:01:56
do in fact is we can go ahead and run some logic let's say we destroy it so I'm just showing you guys one more example to make things clear so if I press play so that's not a pickup so nothing happened but if I hit a pickup as you can see we are destroying it so something like a gun [Music] all this is fine but we do not have any sort of a user interface now apart from the lighting needs to be rebuilt thing you can actually uh delete that by typing in disable all screen messages so oops I didn't type that so disable all

03:02:38
screen messages so you can go ahead and type that and it's going to remove that so there's nothing much really we don't even have a simple health bar so we can go ahead and add a couple of components on screen so in order to create widgets on the screen if you want user interfaces the way you do that is using widget blueprints so let's get to that inside your content folder I want you guys to create a new folder and we can call this one UI and inside this we can call this one for example HUD to denote headsup

03:03:14
display now open it up and inside this folder right click and create a widget blueprint by heading into user interface now you could do it through the blueprint class menu as well type in widget blueprint you should you should find a widget blueprint somewhere over here so user widget is the one actually so go ahead and select that and we can call this one HUD bpor HUD generally I also like to addore WB to represent widget blueprint but but if we are going to have separate folders for each one it's not really

03:03:52
required open it up and you will get a blank canvas and you'll have two tabs over here on the top you have a designer and a graph as well so what we'll be using most of the time is the designer and to add the logic for it we are going to use the graph if you guys have used the QT framework in C++ the functions and stuff work pretty similarly over here here but since this is going to be in Blueprint it's going to be much much easier to comprehend now the most basic type of uh widget that you can add is a canvas

03:04:29
panel so add in a canvas panel before this actually used to come by default without you having to actually add it now you won't worry about most of the settings actually the only thing that you'll worry about is custom or fil screen actually these are the only two which you'll most probably use custom is basically used if you have stuff like drop down and you're making like a child widget for something and I will show you guys examples for that when we go to the higher level part so for now we'll use

03:05:00
fill screen so this is going to take up the entire screen now in order to actually create this now there is nothing but we we can just create it nonetheless generally it's not advisable to create it in in the character widgets usually would be created in something a little more persistent such as a player controller so we have one set up already so we make sure you set that in the game mode open it up and we could do it on begin play add in a custom event and this is where you actually use custom events so you

03:05:33
could use a function no harm with that but let's use custom events this is what you would use them for so we are going to be calling this one for example create HUD and we can call that so create HUD over here we can go ahead and type in create widget we'll get to select it so BP HUD is what we want to create and we can promote this to a variable and call this one HUD or you could call it HUD ref if you really want to be that specific now we have a reference to the HUD however we still haven't actually

03:06:13
created it we have just internally stored it but if you want to show it on the screen type in add to viewport so now this should be added to your screen however there is there is another thing which you could do actually there is another option called add to player screen however this is not really used that much so this is usually used for split screen and stuff like that we'll not get into this so you'll use add to viewport mostly most of the times all right so now under your HUD for the

03:06:53
health bar obviously we need a progress bar so type in progress bar and unreal has everything built in for us so let's add it at the bottom left hand side of the screen that's the reason it chose the canvas panel so that we can easily uh just drag stuff in with other types of widget it's usually like a layout which you create so it's going to be harder for you to just move things around all right so let's add the progress bar and on the right hand side under the details Panner we can rename

03:07:25
it we can call this one health bar and we can set all sorts of parameters maybe we can make this one 350 by 45 and over here you'll see another tab called anchors now anchor is basically telling you the position with respect to it basically for example let's say set it to bottom left in this case bottom left is ideal so this is going to be your 0 comma 0 and with respect to that your Y and your other values are going to be set so when I say the anchor is at the bottom left and my position is 88

03:08:05
what I mean is I have placed this progress bar 88 units to the right of this anchor and Y is basically your vertical Direction so - 120 is 20 units upwards basically and size X and size y will remain the same alignment is basically telling you what to take as this the reference point so if I make this 0. five you'll see it's going to Center off so it's the distance between this and the center now same with the Y so if I type in 05 it'll move a little bit down or up actually because it was

03:08:44
over here so now the point shifted over there so it mov a bit up and if you want to Center something exactly at the center of the screen so for example a Crosshair so you would set the anchor to be this the center one and over here you'll change the alignment to 0. five and set the position to 0 and zero now this is going to be perfectly centered regardless of your resolution now another reason to actually use this so let me just actually move this back so zero zero another reason to use anchors is

03:09:21
for different resolutions let's say you had an 800x 600 screen let's say somebody's playing with that and you had a progress bar over here let's say you left it at the default anchor let's say you didn't actually modify the anchors this widget is actually going to go outside the player screen however if you change the anchor to the bottom right now this widget is -4 61 and - 137 relative to the bottom right corner so then it will always be inside the screen so that's

03:09:56
another reason to use anchor so I'll go ahead and undo all of that so that should be good now if I go ahead and create this so in our player controller on begin play we are actually creating it now if I go ahead and press play you see we see our progress bar and since we have our anchor over here you see it always stays at the same relative position on the screen the next thing that you obviously want to do is actually bring in the values of Health from the character to the actual widget so it's actually pretty simple to

03:10:29
do that so let's go step by step there are quite a few ways in which you can do it so if we would have created the widget on the character it would have been simple to just pass in the health value to the widget however since we have done it in the player controller there is an extra step but nothing to be worried about about so now let's create an event in the player controller so that we can actually interact with the widget so we can call this one update health for example so type in custom

03:10:59
event and call this one update health and for the new value we can go ahead and add in an input and it's going to be of type float obviously and we'll call this one new health now over here in the progress bar we can go ahead and create another event or we could even directly adjust it here so we could get the HUD and over here we could type in first of all let's check if our progress bar is a variable make sure it set to is variable otherwise you won't be able to access it so if once

03:11:35
that is variable get the health bar and again this is where your blueprint menu is going to help you a lot now you want to set the percentage so typ type in set percent you will go ahead and get this node now in case you guys don't know this percent is going to be a value between 0 and 1 and our health is a value between 0 and 100 so let's just divide this by 100 so do that or you could make your health variable store 0 to one that works too all right so you can do that or you could have a custom event inside

03:12:14
your uh BP HUD that works too so let's head back into a character now and what we can do is we can actually do something so let's say when we actually pick something up let's say we reduce our health for example so we can head into our interaction so when we pick it up let's say we reduce our health by 10 maybe now if it is valid we destroy it and we invalidate the nearby pickup and let's reduce our health by 10 so create a health variable first of all now health is a variable which is dependent

03:12:52
on which character you're in so that's why we are creating it in the character make this private over here make this variable private and we can go ahead and set the health to be equal to whoops we can go ahead and set the health to be equal to health minus 10 and we don't want it to actually go below zero so we can go ahead and clamp the value so we can call this one clamp so clamp float minimum is zero maximum is 100 obviously so you can go ahead and set it now if our health is zero so if our

03:13:39
health is less than or equal to zero if you don't clamp it you can check for less than or equal to so let's do that actually so if our health is less than or equal to zero whoops less than or equal to zero we can go ahead and just kill our player so instead of killing it let's just exit the game instead so we can call a we can execute a console command so type in execute console command and this one we'll simply type in exit it's going to exit the game even quit works now this is something which you might

03:14:16
need multiple times so what we can do instead of this is we can actually make a set Health function because we want to exit the game even if our health is reduced for some other reason so here in this case we picked it up so our health reduced but we want to be able to reuse this so right click collapse this to a function and call this one set Health now let's say you don't want this to be able to call on the other blueprints so let's say you want to only be able to call it in this BP character

03:14:48
you can make it a macro instead and obviously we need the health value so grab in health and head back into your event craft pickup over here we can go ahead and pass in the health so this is going to handle everything for us and let's actually make this a larger value let's say 40 so on our third pickup in theory we should exit our game and if it is not less than or equal to zero uh we can go ahead and update the progress bar first things first and remember we had our player controller reference now we can

03:15:22
go ahead and use that so regardless of what we do we want to update the health bar I mean we'll exit over here so we don't need to update it so we can type in update health and new health is going to be our health variable now some people might show you uh how to do this using a binding so you can actually go into your progress bar and you can type in bind and create a binding however this is very very inefficient and it is going to run on tick so actually don't really bother using that do it the way I'm showing you

03:15:59
guys this is the proper way to do it however there is a good there is a small chance that it might miss it might not update but that's nothing to worry about it's going to be like 1 in a million maybe so it honestly doesn't matter so once that's said we should be good to go and make make sure by default your health is set to 100 and once just update the progress bar once you set the player controller reference because we are not actually setting the health by default uh in the hard you could set it however what if a

03:16:33
player disconnected from a match and is coming back so you don't want it to be 100 because you'll be creating the widget once again right so set it once you get the player controller so in our initialized function once we get the player controller reference we can go ahead and set that and we'll clear the timer at the last order doesn't matter here since this function is already being executed the order honestly doesn't matter but we can do it like this now if I go ahead and press play you would see our health

03:17:05
is set to 100 and if I go closer okay let me just speed that up a bit so if I interact with this nothing happens but if I go ahead and interact with this our health reduces my health reduced and now we exit the game the third time we do that so this is basically how you work with widgets so if you want to update it you would just use one of the functions which are there in one of these widgets and what if you wanted text obviously you would just search accordingly type in text and you should be able to find text so let's

03:17:44
actually type in the actual health value so over here what we can do is we can just give 100 by default or we could leave it a text block and set it normally so over here get back into our play controller and in your update Health function we can go ahead and grab our text I don't know if it's set variable so it is not set to be variable so we can type this one Health text now you should be able to access health text from the player controller once you set that to is variable so grab in our

03:18:22
HUD Health text so get your health text and over here we can go ahead and set the text to be equal to the health value itself now there is a special node which you'll use a lot called format text so this is very simple actually use curly braces and type in health it'll make a pin for you whatever you type in curly braces will be a pin and the first one let's just put a plus over there because it's usually usually health is denoted with a plus before so your current so your text is basically going to be plus

03:19:02
along with a health upended with your health so let me just show show that actually so grab in your new health you can grab in any sort of pin by the way now if I go ahead and press play you see it says plus 100 because it took plus and the actual health value itself now I apologize I do realize that the screen is a little bit black and white so now it should be fine so you have plus and you have your health similarly you could you could do something like maybe hyphens so it's just going to append it as

03:19:40
is you can go ahead and mess around with it a little bit let's say you wanted another parameter you could put curly braces once again and type this one maybe something and over here you can go ahead and make make a little literal string or a text so let's just say hi for example so it's going to print plus 100 space high if I put a hyphen here it's going to take it as is so plus 100 hyphen high so stuff like that which you can do using this format text node and it's really handy in my opinion so now if I

03:20:22
go ahead and press play we have our health bar now we could do a little more of Designing so head back into your HUD and you can actually wrap this around with a border if you right click and type in wrap with you can wrap it with a border and actually have a border color and stuff so I can select this and make sure you set your padding to whatever you want padding is basically the spacing you give so if I change the padding in this case so if I change this to 10 You' see that you're giving more space on all

03:20:57
directions I'll just set it to something like five maybe and I'll make this one black so not content color that's going to be a progress PA color instead go to brush color and change that to something dark maybe and over here as well let's just change the fill color to Green because that's more appropriate for your health with it so change that to something a bit more Greener now if I go ahead and press play you would be able to see we get the appropriate color and our health bar

03:21:27
updates as normal and our text updates as well so that's basically it so that's the basics of widget blueprints we will talk a lot more in depth about this as we move further but now you guys should have a pretty basic idea on how to create stuff now the pallet is something which I want you guys to explore so checkbox is a checkbox and you won't use most of these most often you'll use text slider button image border and image is as it says it's an image and one more which you might use if you want

03:22:02
something like a username password menu is a text box so you can grab in a text box and this will allow the user to enter any text inside stuff like that now I want to cover widgets in a little more detail so let's actually create another level called main menu and let's actually transition to this level using a widget so like you would click the play button in your widget and then you would enter this level let's do that now first we can go ahead and create our map so head into content maps right

03:22:39
click create a new level and we can call this one main menu open it up or rather let's just be a little more descriptive call this one main menu level open it up and this should be blank and that's really none of our concern head into UI create a new folder and we'll call this one main menu over here go to user interface widget blueprint and go ahead and select user widget now we can start making our main menu so we can call this one bpor main menu open the widget and we can just have a canvas panel

03:23:22
again add in a button we can Center it first of all so make it 0.5 and .5 and set the positions to be zero we can increase the size a little bit maybe we could make that something like 350 by 100 maybe maybe 450 again size is your personal preference and we can make the background black so background color change that to something darker maybe something like a dark gray we can go in and add in some text and we can call this one play now can change the font as well by the way under font uh you can actually

03:24:08
import your own custom fonts will not get into that but it's actually pretty simple to do it we'll try to get into that in the later part of the but I'm not really sure if I will so maybe change that to regular increase the font size to 35 let's say this should be good now head into your event craft and let's call this one play button so select the button and then under the details panel rename that now if you select the play button variable you should get a bunch of events including on clicked on pressed on

03:24:42
released all of these are as they stand obviously maybe if you have a sound effect or something you could play it on on hovered or there's another way actually where you can play a sound effect when you hover your mouse so or here if I just type in H I should be able to find Howard sound let's just play uh so maybe let's just play this I mean it doesn't make any sense but anyways and I think there is a click sound or a press sound I guess it's called so we can play a press sound so click on

03:25:22
button and what we can do is on click we can go ahead and open our map uh so we can type in open level and we can do buy object preference so over here let's just select our level beginner course level and that should be good now if I go ahead and press play as you see nothing happens because we haven't created the widget yet now since this is a widget which is the only thing in this level you could simply go ahead and create the widget here on begin play so create widget create widget BP main menu add to

03:26:03
viewport we we don't really need to store it because we not actually calling any functions so if I press play you can see it and when we hover over it you see you get the sound effect however one thing you would notice is if you actually have your focus on the window you can't see your mouse cursor so the way you do that is first of all get your player controller so type in get player controller this is a static function so in inside any actor basically you can get your player controller

03:26:33
reference and from here there's actually a variable called set show mouse cursor so show mouse cursor is the variable set that to true and another thing which you can do actually is change the input mode to UI only so that it only focuses on this widget there is another option called game and UI only we'll use that set input mode to game and UI only grab in the player controller reference and that should be good so we can just reroute it double click on the PIN to reroute it and now if I go ahead and press play

03:27:11
you see even when I focus it I can still see my mouse cursor now if I press play you see we transition to the level now we obviously spawned at 0 comma 0 comma 0 so that's the reason that happened now if you want to uh fix that you can go ahead and add in a player start where your default player will spawn so now if I head back into the main menu play it if I head in we will spawn where our player start was but one thing you'll notice is uh we still haven't actually got rid of the mouse focusing part so

03:27:45
your mouse is behaving like how it should so what we can do is on begin play now we are in our main menu level head into our beginner course level generally you do it on your player controller so BP player controller and what you can do is you can set input mode mode game only and we can get a reference to self and you can also set show mouse cursor to false so set show Mouse cursor make that false now if I go ahead and press play okay I mean that wasn't what I intended now head back into your main

03:28:28
menu go ahead and press play now you see your mouse is going to behave normally so that's basically how you deal with it now you can do your normal gameplay stuff so that's how you would actually create you would actually interact with your actual levels and stuff you would transition levels and stuff you using widget blueprints so head back into UI main menu and if we take a look at our code it's really simple and a widget as well it's really simple so that's about it now let's say we wanted to have more

03:29:00
than one option and let's say we wanted to lay them vertically so if you want to add multiple rows you can go ahead and use something known as a vertical box so if I write click on this type in wrap width and use a vertical box you can go ahead and get this now the vertical box will automatically use the same anchor as we used for the child but nonetheless just something which you can change change the size y to something big maybe and press contr D to duplicate this button now over here I can type in exit

03:29:36
let's say and again on click we can change that so play button one is not appropriate we'll change that to exit button so exit button and on click we can go ahead and execute console command and we can type in exit so that should be good to go and you'll notice one thing it's just taking up a fixed amount of space and it's not actually filling it properly so if you want to do that you can select both of these and select fill now let's say you wanted your play button to occupy more

03:30:13
amount of space than exit so you can increase this uh what text box which is available to you so if I hit two and the exit button has one on this option basically they are occupying space in the ratio 2 is to 1 that's basically what it means so you don't want your players to exit obviously so You' make the play button bigger so this is how you would do it now if I press play now the same logic is copied over the reason why the sound is playing even for the exit button is because we copied

03:30:48
over the code so that's why so all the sound effects as well is copied so as you can see press sound and H sound are actually the same in both of these now if I press play I press exit we are going to quit the game if I press play We load into this level so that's pretty cool so that's about it for this part [Music] now it's time we start talking about another feature which blueprint offers that is blueprint function libraries now let's say you wanted to have some functions which might be used in

03:31:31
multiple places but are not relative to a certain object so in that case you would use a blueprint function Library so let me actually show you guys an example so head into Blueprints and all or maybe we could create another folder let's call this one function libraries open it up and over here right click head into Blueprints and select blueprint function library and we can call this one my or our blueprint function library now inside here you would notice that we actually have functions options

03:32:21
to write functions so for example let's say we have something generic so for example let's say uh we have a vector and let's say we want it to normalize it now obviously there is a normalized function already but I'm just taking an example now normalizing a vector is a general operation it's not relative to any object so we can type in normalize and for the input obviously we are going to take in a vector so take in a vector and we can type this one in maybe and now once we have the vector we

03:32:59
are going to first of all get the magnitude of this Vector the way you get magnitude of a vector in Blueprint is by typing in Vector length so get Vector length now this is this is the magnitude of the vector so we can can divide this vector by the magnitude so that is going to normalize the vector for us and once we actually do that we can go ahead and return it so this is going to be the return value and obviously we'll make it a pure function now let's just call this one normalize underscore hours because I I think there

03:33:42
is another function called normalize so just so that it's understandable for us now head back into any one of your blueprints let's say our level blueprint and over here if we just type in normalize so we already had a normalized function but I just took the example underscore R you see we actually get our function and this is not relative to any object so you can call this pretty much everywhere you wish so this is basically your blueprint function Library you just go on creating functions

03:34:17
[Music] so once that's all settled now what if you wanted to use some code or some assets created by somebody else there is actually a huge Marketplace called the unreal Marketplace and you can access it through the epic games launcher so if I head into my epic games launcher head into market place under the Unreal Engine section you would see that you get a massive library of assets and there are a bunch of free ones as well like I I really mean a lot of free assets so what if you wanted to use them

03:34:55
so that is where using plugins and other content packs comes in handy so how you do it is really simple actually so for example I know one which is very handy it's called low entry I believe oops low entry so I actually have it in my library so so it's by this publisher actually so low entry low entry standard Library this is the one which I'm using this is really useful so once you search it up and you can look it up in the marketplace and there are many Forums on Reddit and stuff talking about which

03:35:35
plugins are good and stuff so you can go ahead and install it according to your need so let's say I wanted some weapon models for prototyping you could just type in weapon and you going to get weapon packs the way you install it is by clicking on this install to engine button I've already done that so that's why it shows that I can't now over here in my plugins panel now I should be able to access it over here under installed or uh if you just search it up you would be able to find it and you can enable it

03:36:06
so low entry extended standard library and I need to restart the editor so let me go ahead and do that now that it's done I can go ahead and use the content in the plug-in now how do I know what content is there there will actually be a documentation and source code and stuff available so you could just look it up so there will be a place where the documentation is given so you have a preview over here then you also have access to the source code and a bunch of stuff you could also take a look at this

03:36:39
over here so maybe let's say we wanted to use uh some function here so for example I type in uh is debug build let's say I wanted to see if I am currently in a debug build so I can type in is debug build whoops debug build and as you can see I can use the function now this was a plugin which has to be installed to the engine however we will also look at other types of plugins such as let's say I type in weapon for example I needed a weapon pack so I actually have some in the library you could find a free one so you

03:37:17
can head under free and you can look for it but again now in my library I actually have some weapon packs if I want to install those it's actually really simple so FPS weapons bundle this is one thing which I have so I can go ahead and add this to a project and it does say none of my projects are compatible but plugins like these actually it doesn't really matter if you're using a later version than what is supported as long as you're using a later version than that it should be

03:37:48
totally good to go so click on show all projects and you can go ahead and select this and you can change the version to the latest available one and you can go ahead and add it now just another thing in case you don't have a plugin uh of this sort so the one which we saw last time so let's search for low entry once again so let's say we have a plugin of this sort which you install to the engine but you actually don't have the appropriate version so the way You' actually go about upgrading your version is actually

03:38:26
really simple people haven't made any tutorials on this I don't see any Forum or anything talking about that either so basically you just come into your uh Unreal Engine installation directory so I go to program files and real engine this is where I have it and over here under engine plugins and the marketplace ones will be in the marketplace and for example I go to low entry extended standard Library I can right click on this up plugin file and I can actually open it with any text editor or I can open it with something

03:39:01
like vs code so I'll open it with Visual Studio inside the up plugin file you should see something a little like this so you don't have to worry about any of these things the only thing is the engine version let's say it was there for 4.27 and you're using five and if you want to make it compatible and let's say you're getting build errors you could just go ahead and change 4.27 to 5.0.0 so let's say it was 4.27 by default so you can go ahead and change it to 5. o.o whoops 5. o.o so stuff like

03:39:39
[Music] that all right so that's about about it there isn't really that much depth to plugins I mean I will talk about creating plugins and stuff integrating third party libraries a bit later on in the advanced part of this course but now let's go ahead and actually talk about a recently released tool and which is quite handy in my opinion and those are the modeling tools first of all in your plugin section make sure your plugin is enabled so make sure modeling tools editor mode plugin is enabled and if you

03:40:15
don't want to separately drag your model in the level and edit it then you can press this as well and now if you check your content browser uh make sure you have some sort of a 3D model make sure you have some sort of a static mesh so you can import that from your 3D software so I just got one in from the engine content so what I did was basically actually I'll just go ahead and delete that and redo it so delete that and delete this folder as well save everything now I just search for smore

03:40:52
usually it's a convention to name it SM smore for static mesh under content I just went ahead and created a new folder so new folder and I called it models open it up and just paste it in uh just using the one from the engine content now you can drag it in the level and start editing it by heading into this tab right here and heading into modeling so we have a bunch of options the first few are for uh creating objects but some of the useful ones are for example moving the pivot so let's

03:41:27
say you didn't want this to rotate along the center can go ahead and type pivot and you can move this point over here now if I rotate it it's going to rotate along this point and these changes are actually applied to this so even if I just drag in another ball these changes will be applied to that so just be careful while using them of course you can undo them at any point so just save that and sculpt is basically to deform the shape so something like this and again you can use shift the

03:41:59
same principle works over here as well as we did with the landscape editing so stuff like that then Des sculpt does a similar thing just works a little bit differently so I can just drag it like this I'm not sure what I did there but yeah so I'm not really here to talk about the tools in detail but just to give you an overview of how to actually use it so you could experiment around with all of these so if you type in accept so now we have this shape obviously this is it just messed up with

03:42:31
the UV map and the materials and stuff but anyways that was not our point now a couple of useful things first of all creating shapes so if I just type in stare over here and if I head into this and I can actually make it a curved staircase I can actually increase the number of stairs I can decrease the step height so I can increase the curve angle for example then I can decrease the step height so I can make it something like 10 maybe place that and type in complete now if I go ahead and press play you would be able to see that I can

03:43:09
actually use my stairs so that works well so stuff like that and now shapes are pretty obvious obviously just create a box do stuff with that and now you might be wondering where these are stored or here just check uh what is selected under this under the new asset location if it is selected to Global in your content folder folder there should be a underscore generated folder in my case it was set to World relative so wherever you have your map or here there you should see a underscore generated

03:43:47
folder and if you open it up you should be able to see your static measures so for example we have this stair which we just created and we can drag this in so this is going to come in really really handy for many people in my opinion now not only that it provides us with several other cool features I'll just showcase one of them actually so if you head into your modeling tools once again so so I'll just close it and open it up again so I'll open up the modeling tools and if I type in poly extrude you

03:44:24
can actually draw a shape so if I just click somewhere drag a point do something like this and if I join them now I would be able to create something like this so let's say wanted to create a castle wall or something you could do that and the good part about this is this is UV map by default you don't have to actually UV map it the UVS are pretty good so you can directly go ahead and apply a texture and it is going to look decent generally if you create a weird shape like this in a 3D modeling software you separately have to

03:45:00
go through the effort of UV mapping it so that the textures don't look distorted but in this case you are good to go so that's about it for the modeling tools so you can mess around with those these are really you know specific to what you're doing so according to what you would need you would use the appropriate tools but it is there now even over here you can change the Pivot Point let's say for example so I'll just show you guys once again so modeling I select pivot and if

03:45:35
I move this over and press as accept you would see that the Pivot Point mov over there so that's about it so let's move on to the next part [Music] so what I'm going to be talking about next is kind of the basics of what we did till now so basically we worked with these models over here basically these are called Static meshes so any and all 3D models which you get in the engine without any sort of animations or anything those will generally be static meshes uh any mesh with some sort of

03:46:15
animation is going to be a skeletal mesh basically so stuff like characters gun models and those are going to be your skeletal meshes anything which simulate pH physics or which does not have animations so for example the staircase maybe a weapon model in a pickup blueprint stuff like that are going to be static meshes so they're recognized by a light blue color in the content browser so if I head into models you see it has a light blue color coding and this indicates that it's a static

03:46:49
mesh now we will dive into skeletal m meeses a little more in depth later on but for now I'll just head into static meeses there are a couple of things which I would like to cover first one is enabling nanite now if I head into wireframe mode so now I can actually see all of the vertices in space [Music] now say I have many of those spars and in this case I have more than 6,000 so 6,480 so the first question over here is how's the performance till this great that is thanks to nanite so if you right

03:47:35
click on your model and enable nanite over here if you right click and click on enable you will enable nanite now if I go ahead and disable this you would see that the performance dips immediately so that's one thing about nanite so as you can see it's really not playable at this point now if I mean obviously this is highly unrealistic and moreover it will depend more on your computer as well so if I go ahead and enable nanite now and if I press play as you can see even with so many spares

03:48:05
right in front of me it's absolutely not affecting performance now we are not here to talk about the actual technology involved in nanite so that's the reason I'm not telling anything else but this is basically it currently in 5.0.3 there are a few limitations for example let's say you wanted to use this on a tree you probably cannot because trees contain leaves and leaves used masked materials and those are not yet supported on nanite and it but they will be supported in 5.1 so very very soon

03:48:36
you would be able to use them so that's about it there are a few material features which you can't use and we will talk about materials so stuff like ethering and stuff you'll have to just disable those notes if you want to use nanite but for most objects so stuff like walls or maybe if you have an insane level something like this nanite is going to come in handy so that's about [Music] nanite by now one thing that you would have probably noticed is that any and all objects in the scene actually have

03:49:13
some sort of a Mater material on them so for example this has some neon blue texture on it and it seems to be glowing and this box right here has some sort of checkerboard and same with the ground so what's up with that so basically those are materials and that's what gives the color and all the other roughness related properties of a given surface now let's actually go about seeing how to create a material and apply it on objects so let's just use a cube for example in order to demonstrate using

03:49:50
materials so let me just grab in a cube and I'll just place it in the scene now this has a material basic shape material you can actually explore this by clicking on this search icon over here so you'll actually go to the directory where the material is stored but in our case let's create a new folder called materials and let's go ahead and open it up right click and create a new material or you can head into materials and create a new material here now the most important ones are just materials and

03:50:24
material instances the rest are just stuff which you might need in specific circumstances so we'll take a look at material and let's call this one our material now applying a material on a surface is actually really simple now we aren't going to be dealing with multiple materials on a single object in this part of the course course we will try to deal with it later on but for now we won't be doing anything so by default you get this Checker material so I'll just drag this in and you can in order

03:50:55
to apply it you just drag it basically on the surface that's how you do it or if you want to apply to uh a static mesh in general so let's say I wanted all of the uh okay whatever this object is so let's say I wanted all of this object to have our material so what I'd do is i' into the static mesh and over here I'm going to select our material so let me go back so all content materials R material you can select that and you can click on this Arrow icon which will use R material so now it's actually using

03:51:32
our material so we haven't seen any change because we don't have anything set up in the material but the way you actually start working with this is by using these node so this pin right here is as the name suggests the base color now how do you define a base color so the most basic node over here is going to be a constant so whoops I press C on the keyboard I'm supposed to press one on the keyboard and left click and you see you get this node here which allows you to enter value now generally you would enter

03:52:08
value between zero and one but in some cases you would enter higher and lower values so in this case if I just plug this in the base color and you can see it's compatible so You' see that our material is fully black now it's just a fully black material what if I increase this a bit now save that again as you can see it became a lighter shade of gray so one is going to be white so this is basically a gradient zero is black and one is white what if you wanted to give a color so You' hold three on your keyboard and

03:52:49
right left click then you'd get something known as a constant three Vector this is basically our r g and B values so red green and blue so you can go ahead if you wanted red you could do one on red and as you can see you get a red color material and it's applied to all the objects which are using our material so that's about it for base color now if you want to bring in any textures I recommend this website called cc0 textures so open it up now it's rename to ambient CG keep forgetting about that

03:53:26
so if you just head in and you can just grab in any texture so just I'll just grab in the lowest resolution one so I can open it up in my folder over there and over here I'll just drag it into images for now I just have it set up like like this so I'm just going to extract it and oh here you see you get a bunch of textures if you want to import it in the engine it's really simple actually to import any asset be textures models or whatever so we'll create a new folder and we'll import it so

03:54:04
textures open it up and if I go ahead and drag this for example so I can just select all of these and and I can go ahead and drag this in my content browser and we can go ahead and save it now if I want to apply this texture to this material now first of all we'll see which one is the base color sometimes these textures are labeled as albo but albo is basically a base color without any sort of uh Shadow related information that's basically what it means without any other sort of detailing it's just the raw color

03:54:45
so if I drag this in the base color I can do that now you could do this as well totally fine so this is how you bring in a texture now if I go ahead and look into my level you see we have this wood texture on our little wall here now what if I wanted to tile this texture a little better now let's say I wanted to make this bigger or smaller you'd use something known as a texture coordinates so you type in text code and you're going to see texture cordinate plug that into the UVS and now let's say I press one your

03:55:25
texture will now be scaled 10 times you and we are basically like your X and Y to be very vague now we zoomed in way too much so let's let's make two now so now you see it's going to be more tiled so now if you would see you would have a more tiled material so if I make this three for example and if I go ahead and save this you would see that it'll be even more tiled so I can make this 3.5 I can increase the value and it's going to be more tiled so I can click apply save and I should be able to see there

03:56:05
are more number of Pricks now I I I'll just set this to one once again and save that and as you can see it's applied to our level now this may be fine but what if you wanted more details let's say you wanted to make this very glossy so in that case you can use the roughness node now the roughness is basically a 0 to one value so you can again use a constant if you want so zero is going to be fully reflective now you could use the specular Channel as well but most of the times you'll only use

03:56:39
roughness it's very rare that you will actually mess with the specular CH Channel so now if I go ahead and apply this you would see that it's very glossy and if that's not really that clear drag in a point light just move this and as you can see it's reflecting everything over there you see the little point over there so that's showing roughness zero now if I change this to one for example and if I hit save You' see that it's not reflecting the light at all so that's that's the

03:57:15
use of the roughness Channel now obviously this is some sort of a wood floor texture so obviously it will be depending on the grains of what's there over there so how you would set it up is by using a roughness map now generally in in websites such as cc0 or ambient CG now as it's called you would get something known as a roughness map basically the brighter parts of the image are where the light is reflected more the darker parts of the image are where light is not reflected so let's

03:57:51
say there is a fully black area here so that's where all the light is going to be reflected so I might have told it the other way around basically the more bright the color the more the roughness now if I drag this in use this in the roughness Channel as you can see this gives us a little more definition now as you can see at the borders over there you can clearly see that the roughness map is doing something so this is about roughness similarly normal is basically uh your depth so as you can

03:58:29
see this texture although it has a bit of roughness it looks completely flat now if I go ahead and add in the normal map so if I just snap this to the left and bring in my unreal editor on the right and if I go ahead and apply my normal map here and if I hit apply as you can see you would see a little bit of a depth over there now if you can't really see it that's probably because this is pretty subtle so you can use something known as a multiply basically it's just going to multiply the value of each pixel in this

03:59:09
texture so multiply this you can use a constant or you can set the value over here itself in the multiply node so if I typee in 100 let's say for example so now you would be able to see a little bit of the depth over there but since this sort of a texture isn't really containing much of depth so you won't really see it there are other ways to increase the depth of a normal map but that's not the point of this tutorial so basically normal map is for your depth if you're into PBR rendering

03:59:42
you'll probably already know all this stuff ambient osion is basically like your uh depth in your crevices and stuff it's kind of hard to explain it there's actually a comment here so simulate the self shadowing that H happens within crevices of a surface basically that's what ambient osion is so in stuff like trees and rocks ambient osion is something which would play a major role and this sort of a texture it's really not going to do much so this is about the basics of materials now obviously

04:00:21
this is completely wrong because we only have a texture coordinate for that one texture so make sure you plug everything in so just plug everything in now if you go ahead and apply and save that now You' be able to see that it's applied properly this had a subtle effect from the start itself so that's the reason you couldn't really see anything wrong with it so we created a basic material here now for any of these you can actually use your constants but most of the time except base color you won't be using

04:00:59
constants you'll be using textures now that's the very basics of materials there are a lot you can do let's say you wanted to make this thing glow so let me just remove all of this stuff let's say I just wanted a glowing neon green color so let me just get a constant 3 Vector so the same right click search menu exists in the material editor as well drag that in the base color and what you want to do is first you can grab in a constant and maybe let's say you have 10 this has to be a value

04:01:34
greater than one so let's say I have two for example so now you'd see that it's completely glowing white in color now if you wanted it to Glow in this color itself what You' do is you would actually get this and You' multiply this by two so you would multiply this by two now if I go ahead and press save you see it's glowing in a sort of green color so this is basically called an emissive material because it emits light and it's pretty cool to look at by adjusting the value you multiply it with

04:02:16
you adjust the intensity now one problem which you might have noticed here is every time we want to change a value so for example we want to make this less bright let's say 1.5 now every time we have to apply and save this what if we could dynamically change this that's where material instances come in it's basically like your derived class in your uh C++ inheritance but to put that in short basically you create another uh asset known as a material instance which is subordinate to this material and you can

04:02:55
edit all the parameters in it so I can right click on our material and create the material instance and let's just keep it as the engine has suggested now instead of applying our material we'll apply our material instance nothing has changed obviously however if if I head into our material instance now I can change the parameters over here the first thing you might notice is there is nothing to change so how do you do that basically you would have to head in here right click and convert it to a

04:03:30
parameter so any constant or any texture which you convert to a parameter will be a value which you can change so this is going to be called brightness let's say brightness and this one is going to we called color so right click convert to parameter and call this one color now apply and save it now if I open up my instance you would see that you get two parameters and now I can edit them so now if I press two you see the changes are live so zero Works 1 2 not. 3 so I can adjust my values just like

04:04:11
this and I can change the color as well and it's updating dynamically so for the most part you'll be using material instances for this purpose itself so these were the basics of materials now you could Tinker around a bit look into the documentation and create something [Music] yourself now we haven't talked too much about the other type of mesh that is the skeletal mesh so let's talk about that now now if I go ahead and press play actually you would see that we have a character over here which is moving

04:04:51
around now the animations aren't actually complete if you were to notice he's just sliding around he's not actually doing anything now how do you define the logic where you know if you're moving above a certain speed maybe let's say you start moving you want to play an animation how do you define that so that is where you use an animation blueprint and that is what I was searching at the start of this course when we actually did the character so head into your character over here one thing that you

04:05:23
would notice is if I just head into mesh and if I just click on the search icon on the animation blueprint it actually takes us to a folder inside the engine directory where there is an animation blueprint which actually does something over here so this is how the animations are actually controlled and we'll create one from scratch we can reuse these animations no problem so head into your content folder uh not the engine so content and for now we can just uh head into our models folder and over here

04:06:00
let's assume we had our character here so let's call that tutorial character cuz I guess that's what it was called tutorial TPP I guess I'll just open it up right click create under animation create an animation blueprint and select the skeleton now now I'm assuming you have a little bit of knowledge of what's a skeleton what bones and stuff so at least that much would be required if you want to understand this basically know that each joint which you have each uh point which can hinge basically is going

04:06:36
to be your uh bone so if I'm not clear about that if I head into the actual skeletal mesh so if I head into this one so I'm not sure what it's called and this one let's leave it at new an MBP so let's TPP I guess so this is the skeletal mesh now if I were to just click on this and if I head into the skeleton view you would see for example this is going to be your index so if I rotate it you can see that we can actually control it index 2 is going to be the further part of the

04:07:15
finger stuff like that I'm not actually applying these changes so that's totally okay and for example if I take the pelvis I can go ahead and rotate the entire thing because that's the root that's the reason it's happening if I take spine it's going to rotate the back stuff like that let's say you want it to rotate it a little something like this so you could make him Bend forward stuff like that so this is a skeletal mesh and output pose or here in the anim graph as soon as you open the animation

04:07:50
blueprint this is what determines what pose you're in by default it'll just take a t pose or whatever pose it was in when you imported the model so let's apply our animation blueprint to our character so head into your character select the mesh and for the animation blueprint let's select new anbp or whatever that was called so new anim blueprint so as you can see we stuck in a t POS right now and let's start applying animations now in order to add an animation the most basic way you could

04:08:24
do it is you can simply drag in this animation and you can play it so this is going to be the idle animation and these are animations which the engine has provided so I haven't really done anything here so if you have your own character you would have your own animations but as you can see there is really no logic that you can Define over here so the way you do that is by first of all we can start by creating a state machine this is the most basic thing you can do in an anim blueprint so basically you can use

04:08:59
your variables over here to determine Logic on how to change between animations let me show you with an example so we'll just leave it at New State machine for now or we can call this one uh walk run maybe idle walk run let's say just name it appropriately and now if I compile I'll be in a t again now entry is where you would start so obviously if nothing's really happening you you would want to idle so head into tutorial idle if you were to notice it just outputs the animation post this is

04:09:39
something like your return node basically head back into your idle walk crun State machine now if I compile as you would see it's playing the idle animation and if I press play actually this is going to work now we want another state so right click add State and this one is going to be called walk/run now this is a shortcut way to do it like I'm not doing a separate Walk and Run phase I will do a separate Walk and Run St state after I do this so we want to be able to transition from idle to walk

04:10:18
run so drag in an arrow and when we stop we actually want to be able to go back as well and I will show you what I mean by that now if I head into walk run and if I drag this animation you would see that he's not actually heading into walk run so what you can do is you can just set this to true for example and you would see that he will be in this walk run state so what this basically is is if this Boolean is true the character will be able to transition from this animation to this basically so how do you do that we can

04:11:01
actually set uh set up some logic here so we can say is moving for example this is not how you do it I'm just showing you guys the basics so if he is moving we want to trans position to the Run phase so idle walk run we have that now in the event graph we'll actually set up the logic to get is moving because remember we only have the variable but we not actually setting the value so every time the animation updates so that's going to be every frame what we can do is we can try get Pawn owner basically that's going to be

04:11:40
our character reference and we can cast it to our uh I don't know what it was called BP character I guess cast it to that don't do a cast on update actually you can actually uh do it on I guess it's called start uh there's an equivalent of begin play actually event blueprint begin play so on this node you can actually cast it and you can store a reference and use that don't cast to it every frame it's not efficient I so you can promote that to a variable and call this one

04:12:17
character reference so character reference and once we have that stored what we can do is we can use that if this is valid of course so convert to validated get if our character reference is valid uh what we'll do is we will get the speed so how you get the speed is by getting the velocity so velocity get velocity and we are going to get the vector length and if this Vector length is greater than zero it means we are moving so now if I compile you see he's idle but now if I press play if I start

04:13:05
moving you see the animation triggers but now he's not going back and that is where the transition comes in we have set set up the logic to go from idle to walk run but the engine doesn't know when to come back so a very simple thing you can do is put this back and if he is not moving so you can type in an exclamation so if he is not moving then we can go ahead and transition back now if I press play as you can see it's working just fine now there are only two animations here but what if you wanted to blend between them

04:13:42
what if you wanted a walk phase let's say so the way you do it is by using a blend space so what a blend space is is basically transitioning between two animations and I'll just show that I'm not really going to talk too much in depth about animations and stuff but I I guess you you guys kind of get the basic idea let's say you had like a jumping animation so what you do is you wouldd have another Boolean for uh the jump State and in this state machine here you would create a new state and call this

04:14:14
one jumping and then you would transition from this and you would go back stuff like that that's basically how you do it uh now if we wanted to set up our blend space as I told you guys so head into your models TP tutorial TPP and let's just right click animation and let's create a blend space so now we can select a skeleton and we'll call this one walkround for example so walk run if you have a separate walking animation you can inject it in but for now we won't now in the access settings here

04:14:56
this is what you'll actually be using so your vertical axis is like your speed basically I mean it's a convention you can interchangeably use this but you can use the vertical axis as speed so basically you see the value is 0 to 100 so that's what it is so we can type in speed because we can use this name later on and for the horizontal axis we can call this One Direction and it's going to be from - 180 to + 180 over here for Speed we can go zero to whatever maximum speed by default at

04:15:33
600 so we'll go go with that and we don't have sideways animations otherwise on the left here you can place your sideways animations I'll just show you with these ones so obviously when your speed and direction is zero you would be idling and walk forward is going to be over here now if I hold down shift and if I walk through this so whoops so I going just leave that over there so add Zer and zero and hold control actually hold control and if you would notice you're transitioning between the animation so

04:16:19
if I play as you see now if you're walking slowly so let's say I leave it at here so when my speed is 373 and my direction is whatever that is this is how the animation is going to play now if you want this to change a little bit you can actually uh increase or decrease the values over here and smoothing time is basically for your transition time so how long it'll take to transition from one animation to the other generally I just leave it at zero I've had no issues honestly now in our animation blueprint

04:16:56
instead of this we can use our walk around blend space all right you can connect this blend space to the output now we would see that you have to provide the direction and speed and doing that is actually pretty simple so head into your event craft and what you basically do is you grab your character reference over here and from this we can actually get the velocity so velocity get velocity and then from here we can get the vector length so basically the magnitude of the vector all right uh once we get that for

04:17:38
the direction actually uh we have a node called calculate Direction which requires uh the velocity and I will tell you what to do next so we need direction and speed so we can promote these two variable so promote to variable we can call this One Direction and we can call this one speed and if the character is valid we can set the direction and speed over here in the direction for the velocity we can just directly grab in this pin over here and then what we can do is we can get actor rotation now if I hit compile and if I

04:18:40
go ahead and plug these in or here in my blend space player then in my transition over here so walk run to idle instead of not moving what we can do is we can get the speed and if it is less than a certain value so if it is less than let's say about 10 so then we'll enter this transition similarly if the speed is greater than 10 we'll enter this transition so so if the speed is greater than 10 so then we can go ahead and transition into the walk run state so once we change that we should have our

04:19:23
logic working so now if I go ahead and press play as you can see the work run animations are working so that's about it now we have finished animating the character with some basic animation blueprints so that's all there is to it obviously there are many more things you can do with this animation blueprint of course you can you can have sprinting as well so if you would have Sprint uh you would you know have another state called Sprint and then you would plug it in according to what logic you want

04:20:00
basically all you have to take care of is when your character can transition into States and make sure it's not going to be in two states at the same time that's about it and in the event graph uh anything that has to update so for example the speed of the character those can be done over here on blueprint update animation event so now I I think this is more than enough for blueprints and I I think with this much of blueprint knowledge you would be able to make an entire game assuming of

04:20:38
course you would be ready to look into the documentation a bit uh and look into what the various functions do if you actually play around with whatever we did plus look at a few extra functions you can create an entire game and now for the more keen ones out of you here uh we are going to head into C++ now we'll be taking a deep dive into the more advanced features of the engine now not to worry for those people who don't know C++ I will also be brushing through some of the prerequisites that you need

04:21:13
in C++ in order to get started honestly there's not much to do with the language most of it would just be function calls and stuff like that so anyways without any more further delay let's actually start learning C++ for unreal now I will be going through the basics [Music] now now let's just talk a little bit about the prerequisite knowledge of C++ which you'll need to actually understand the further part of the course I do still recommend you learn C++ separately but I will get get you guys what you

04:21:51
need for unreal because it's really not that important to know the language more so you need to know the features which we actually will make use of in unreal so I'll just create an empty console application here so this is going to be a blank application with uh in the terminal now I won't even use this I'll just use an empty project template so I'll just search for empty in Visual Studio of course I mean we have it right here so just go click next and doesn't really matter I'll just look for a

04:22:24
folder so I'm just going to create it there and click create so just leave all the settings at default none of these would matter for now now once I've created this I'll just go ahead and set up the basic stuff which you need for C++ so first of all you need a C++ file with a main function in it so just to uh just for my reference I'm going to name it main. CPP and we need a main function we'll not get into that now so int Main and we just going to return zero now I'll not get into this but the

04:23:03
feature which first of all we'll need is to include code from other files now if you want to do that you would do hash includ and inside angular brackets or inside double quotes depending on the situation you would include the actual header file so let's say I have a header file so I'll create one so go ahead and call this I don't know header. let's just leave it as this and pragma ones basically means uh it this header file will only be included once so you won't have circular

04:23:39
dependencies and stuff basically but anyways let's go ahead and type some code so in order to create variables that's the first thing you'll need apart from including so including this header file is simple so in double codes you can put header. or you could even use angular brackets you know generally you would use that only for like standard C++ stuff but both of them will work so if you want to include header. HED through this you might have to add it in the include parts so we'll not do that we'll

04:24:12
stick with this so let's say something standard C++ such as IO Stream So I misspelled that IO stream I can go ahead and do this or if I have something standard C for example Windows do H so I can do that so for standard C++ libraries you would uh not use H for standard c1s you'll use so for example if you want cmath that's going to be without a h or you could do math.h this is the cmath library so stuff like this for now we'll include header so whoops so header. now this should work and later

04:25:00
on I will be showing you guys how to include unreal headers that's not an issue so this main function I just like to go over basically our program is going to start from here but again as I told you guys when you're developing in a game in unreal You' really not worry about the main function that is handled in the engine so if you actually go through the engine Source you will find somewhere where you have int Main and there is there will be a while loop while loop which actually runs the game

04:25:28
so we'll not talk about that so let's write some code so first of all creating variables and before we do that one thing to note is that these are just text files honestly you can put the same code in a header and a C+ plus file it it really doesn't matter by putting do hedge you just indicate that you want to include it as a header so that's the only reason both of these are technically just text files and can be opened with any text editor such as notepad notepad++ Visual Studio or

04:26:00
Visual Studio code honestly doesn't matter so if you want to create a variable you can first of all head into CPP reference to know the basic types but if you want to create an integer for example you type in int space your variable name so for example we'll have my integer and if you type in equals you can assign an initial value to it you actually don't need to do that you can do this a bit later as well but you have to do it inside of a function or something so if I just put my integer

04:26:37
equal 12 and make sure you end everything with a semicolon this is not going to work work because even though you have this line here you're not executing this at all so remember I told you guys uh the program starts from the main function so over here if I put my integer equals 12 this is going to work why this works is because we have included header. head so it's as if it just copied over all of this content and pasted it in instead of this hashing clude now similarly you can have other

04:27:10
types which we discussed so you can have float float X for example and you can have many other types so for example if you wanted a string you would put in STD string in unreal you use F string but again now you're getting an error that's simply because you have to include string so these are the few additional complexities which come with C++ so STD string my string equals let's say test string and you can go ahead and set the value again test string so not sure what we call that so

04:27:53
okay my string is what we called it so my string equals and you can assign any value to it or you could even use the Constructor for this anyways this is how you create variables like this data type variable name equals value value need not be defined initialized as soon as you create the variable you can do it later as well but it's always a good practice to do it now one more thing is that these variables can be printed out which you will not use in unreal you'll use the print string function to print

04:28:36
it on the viewport but in in a console application you do something like STD C out and you would go ahead and print my string for example again we not using this in unreal so that's the reason I'm not really covering this so the error is because we haven't included the header which contains this function so you can go ahead and include iio stream and if you go ahead and run a debugger here as you see we get 232 printed because that was our string again if we just delete this part you

04:29:14
would see we will get test string and we can also print my integer like this so we get 12 so this is how we would go about printing stuff and what if you wanted to write your own function so what if you have like 10 lines of code and you wanted it to be in uh be called once so basically you can create a function with this syntax X so if you want to create a function what you do is You' put the return type let's say we create an addition function so our result is going to be an integer so the return type is

04:29:56
int space your function name so in our case let's just descriptively name it add and in the bracket you would put the Val put the variables which you know which you take from outside so in order to add two numbers we will need two numbers first of all so we are going to pass two integers so the same way in which you created a variable and in the same way in which you know you'd handle anything else you would just do int a comma int B so you separate arguments through a comma so what this basically

04:30:32
means is when I call add so when I say add and I put my parenthesis so this is how you call a function so if you want to execute add this is how you do it and you would end it with a semicolon now inside the bracket you would put the values of A and B so in my case if I just put in 12 and 43 or I'll just take some some random numbers now the result of this is going to be returned here and in fact instead of you can set it inside the variable so if I do my integer equals add of 1342 comma 43 so whatever value will be

04:31:12
returned Le here that will be set inside my integer now if you want to actually write the logic for this so you simply do return a plus P something like this so this is how you do a function but honestly you don't need the syntax since we'll we'll we actually have a simpler way to actually write functions we'll be using classes mostly so you shouldn't really bother too much about all this and with that being said let me just show you guys how to create a class so I'll do it in my header so for

04:31:47
example I'll just do a class called student and I'll open up my curly braces just follow along with the syntax it's just a matter of getting used to it so under private so these were the private variables which we talked about in Blueprint as well so I can say we have a name and let's say we have his marks so in marks something simple like that and under the public section we can have some methods so we can say STD string oops and we can call this one get name and instead of writing the

04:32:34
definition over here like this so this is similar to what we did here it's just that it is inside the class now what we can do is we can only have the Declaration here like this so only the name is given here but we can actually have it defined outside this class itself so I can do this and I can go ahead and actually make another function so I can say in get marks so now you can also go ahead and Define this outside the class how you do that is you would use this syntax I'm not talking in depth about this mostly

04:33:18
because there's a shortcut to do it which I will talk about so STD string and what what was a class called student followed by two colons you do get name and you can write your function definition over here so you can go ahead and return I guess it was called name so name and similarly you can provide a definition for the marks as well so int student get marks and you can go ahead and write the definition for it return marks so basically you are going to get the marks from this now if you want to

04:34:02
instantiate a student so let's say you wanted to create a student object from this remember we talked about classes and objects so you just do student let's just call him S1 for example and you can do S1 doget name now dot is what you would use to refer to the members inside a class in unreal though when you create objects you generally have a pointer to it so basically the memory address of it is a pointer nothing much to worry really so I'll just show you guys a way to create it so if I type in student pointer instead

04:34:48
equals new S1 basically we are Dynamic new student so new student basically we are dynamically creating this and instead of the actual variable name we have a pointer to it pretty much now nothing much to worry about you would just put a star instead of just referring to student and if you want to refer to something through a pointer you do S1 instead of putting a DOT now if you were to do dot you see it just got replaced with an arrow so You' refer it with an arrow so something like this so if we actually

04:35:29
just create a method to set the marks so I'll just do void set marks and it's going to be int the parameter which we need so int marks so we'll take this value from outside and we can say marks okay we we are using this again so we can type in marks with a lower case so marks equals marks so what we can do is we can say S1 dot set set marks or rather with the arrow set marks and we can just say 56 for example just a random number and we can print it by typing in stdc out and we can print this so run a

04:36:17
debugger and as you can see we got 56 printed so we successfully set the marks so this is how you would call functions which are defined inside a class and you will need to call them through an object because you need to instantiate them first of all this is something which you will not do in unreal you would use the functions such as spawn actor and stuff in order to actually create objects but anyways this was just something I showed you guys now with this much you can pretty much do it if there's anything else such as for

04:36:49
loops and stuff you can just follow along and look at the syntax that's pretty much it and if statements are also easy so you just do if and you would have the condition in the bracket so let's say the marks is greater than 56 so I can do S1 get marks S1 get marks greater than let's say 35 then we can go ahead and print that the student has passed so stdc out and I can say passed so if I do this as you would see we get 56 and passed obviously this is not in a new line but that's pretty easy

04:37:29
to do so you can do STD NL and now You' see 56 pass so with this much basic C++ you can actually follow along but again I do recommend you separately learn a bit of C++ before you come in the upcoming sections of this course is going to be for intermediate and advanced users so before you actually get started I recommend you guys do a few things first of all spend maybe a few days actually exploring the engine a little bit more maybe creating a tiny game or something and secondly make sure you do know the basics of objectoriented

04:38:11
programming in C++ so stuff like your classes and you know uh stuff like structs functions and variables and the the basic stuff basically if you guys are familiar with that much of C++ and you have used the engine a little bit you would be able to follow along with the further part of the course [Music] so in order to start coding in C++ for unreal head into tools and open your Visual Studio project by clicking on that button over there and you should be in some sort of a file over here now you may have

04:38:59
something blank so we'll just close that now under your games folder you should see your project name here and this is where you actually start working with stuff now we don't have anything actually under this we are going to be having our source files so you don't actually create it here in unreal in unreal you actually have the option to just generate all the boiler plate code for you you can do that by heading into tools and by typing in new C++ class now over here you get various options now if

04:39:38
you have something really simple if you have some pure C++ l iic you could just create an empty class and you could just Tinker around it's just going to create a Constructor Destructor and it's going to write the class definition for you along with no macros just the standard C++ one but the most basic useful thing that you'll use in unreal is going to be your object so under all classes if you select object this is going to be equivalent to your object in blueprints however when you actually create it so

04:40:10
if I just create it it uh just select public and this is just uh to determine where your CPP file will be whether it'll be in the public folder or the private folder now over here we can just call this CPP object uh so let's not confuse ourself let's just call it CPP uncore yeah object is fine so this is not an object this is the class which is named CPP object please don't get confused with that so create a class and now as you can see you have some really basic code and one thing you might not have noticed

04:40:51
is okay live coding is on that's a different story but what you might notice is it already has several things such as it has included some header files here these are just unreal standard header files and you will need them and you might have seen a few extra mac as well so this is a uclass macro and inside these these actually taken arguments too now these are useful for the unreal header tool basically when you compile this it happens in two phases basically your unreal header tool sets up stuff which are specific to your

04:41:32
objects for unreal called U objects and in order to implement those features it does certain extra steps so so when you get a compiler error it could be either from that or from your standard C++ compiler anyways that shouldn't be much of a problem to you guys now if you might have noticed even though we called it CPP object it's prefixed with a u and we have inherited it from U object now why is it like this now basically any object that you create that is a derived class of youu object must have the prefix U

04:42:13
and even object has the prefix u in Blueprint it is just shown as object however in theory it is actually U object and similarly for actors so let's actually create an actor as well so we can head back into the editor tools new C++ class and as you can see you see pretty much the same stuff over here but these are the two important ones object and actor now obviously character Pawn and stuff like that are important but they don't have any specific prefixes so I I'll be talking about them a bit later

04:42:49
and obviously we'll talk in depth about the inheritance hierarchy so I'll select actor and let's call this one cpor actor create that and live coding if works properly it should in theory compile it for us uh now if we actually open it up and reload this you would see you find something which looks a little bit overwhelming if you're looking at it from the first time but if you ignore this macro and if you ignore this comment here I don't even know why this uh comment exists because

04:43:27
if you come to an extent where you can write or interpret this code I don't think you need to know that a Constructor sets the default value so we'll just delete that comment and begin play is basically your event begin in Blueprint same thing uh tick is again your tick in Blueprint you can delete the comment now this code looks a lot more cleaner now this is a virtual function and if you were to notice it's not called CPP actor it's called a CPP actor basically every actor is prefixed with an A and the actor

04:44:02
class itself as [Music] well all right now that we have EST estblished a basic understanding on creating uh blueprint equivalent actors and objects let's look at the inheritance hierarchy in unreal in a little more detail now I'm not covering everything over here now I have left a few things such as interfaces and I'm not going into each class I'm just talking about the ones that you'll use in almost every project so that should cover things for you if you need anything in specific the documentation

04:44:38
should help you if you understand this much so at the base level you have U object of course you have your typical basic C++ class but we are not getting into that now under that I can categorize uh these into three main other classes which you'll use now there are many others but you won't really use them the first one and which you probably expected is a actor now an actor or a actor as it's called in C++ is something which can be placed in the scene so if you want to place something

04:45:15
in the scene and write the code in C++ you would create an a actor or in the menu or in the unreal editor it's referred to as actor everywhere now similar to pawn you have a pawn which is basically something which can be possessed by a controller so basically you can control it and it need not be you it could be an AI as well so maybe you could write some code for Bots or something so you would use Pawn in that case and if you have something specific like a humanoid character or something generally for

04:45:53
most of the things which will be Pawn you generally use character so if you need a movement component and stuff like that you would use character some functionality is already set up in your character which is not set up in Pawn so something things such as adding your controller pitch and your input and you know uh many other functions which we will talk about as we use them so that's where you use character this might be clear now a controller is basically an actor which takes in input now you cannot place a controller in a

04:46:32
level obviously it sounds a bit stupid to place a controller in a level but basically uh each player will have his own controller and to be specific he will have a player controller if it's an AI or something you have something known as an AI controller but again we are not getting into that we it's really not that common to use it a controller will basically take your input now although you can set up your input bindings in other actor blueprints controller is the right one to actually hard code bindings and stuff

04:47:06
like that generally when you create widgets which are not associated with your character you would create them inside your player controller blueprint generally you create a player controller you don't create a controller and that's about it for what you'll use for the most part and if we actually head into more gameplay oriented classes you have a info the reason I put this is because this was this was just a wrapper for you know these classes which you'll use you'll never create an a info actor so

04:47:38
ignore this this is just for your reference over here you would see a game mode base as the name suggests game mode base it's basically your game mode so anything any code logic regarding your game mode will be there in this and obviously it's really simple for me to just tell it like this but once I take a couple of examples it's going to be crystal clear for you guys and there is also an aame mode class which is inherited from this and it has some additional functionality for the most part we will stick with

04:48:14
aame mode base but again you can feel free to use aame mode similarly a game State base and a game State now you might ask what's the difference between these two the main difference is that game mode exists only on the server in multiplayer games whereas game State exists both on the server and client so things like match timers which you would want all the players to be able to see as well you would have them stored in the game State and maybe some other variables which you only want to use as

04:48:50
a means of calculating something in game so stuff which will only be there on the server in multiplayer games or something which is core to your fundamental game play so something like maybe you know switching to another level when you enter place or something I mean depends on the game honestly can't just tell what you do with it just like that but basically basically game mode game State work together hand in hand now there's one more actually called the player State now the player state is really

04:49:22
special because this is replic this is replicated by default to all the clients in multiplayer we more in detail about multiplayer later on but for now just know that player state is going to be kind of the class which you'll use for anything that all the play players must know at all points of time and generally you would store info common to a given player which other players need to know uh stuff like your player name would be there in your player State because all other players need to be able to access

04:49:55
your player name at any point of time so I just give you an example you could be creative with it and do whatever you want now one thing you might have noticed over here for the last one which I'll talk about under U object is uh or actually two more uh game instan is as the name suggests your game instance so this is talking about your game as a whole and not anything inside the game so instead of begin play actually you have something known as event in it here so let's say you call something off of event in it

04:50:31
that actually runs well before your level actually loads so we'll look into examples again if you have anything part paining to the game which has to sustain between level transitions let's say you move from your main menu to your actual game playay level if you want stuff to sustain between them let's say you wanted a variable to sustain in that case you would use the game instance because the game instance will not be destroyed between levels but when you transition from one level to the other

04:51:03
all the actors and all the widgets everything else that you could possibly think of are going to be destroyed now speaking of widgets we have multiple classes here which you'll probably never even touch even widget to be honest you'll never touch in C++ it's very rare that you you would require a C++ class for a widget so you use a widget is the class which you'll use of course in the editor it's going to be referred to as user widget so this is how You' create widgets but honestly it's too much of a

04:51:33
pain to work with widgets and C++ for something that's just you know very simple you could just work with other Blueprints and just have a blueprint widget which you would interact with stuff like that so that's about it actually now the way you would practically use this is you would have one C++ Base Class so for example we can have for a character we can have one character and we can go ahead and derive one so let's say we call this one R character so let's say it is a we'll just call it CPP as a convention

04:52:09
a CPP uncore r R character I'll just call it R care for now now what you do is you would have core functionality written inside this class so for example your movement maybe maybe if you have a first person shooter game your firing logic basically stuff that is Mission critical for the game and stuff which would break if they don't execute so for that you would write it in C++ but other cosmetic things which you don't really require and it's fine if it executes a bit late stuff like you know

04:52:43
uh creating widget maybe uh let's say you have a Crosshair on the screen maybe updating its position uh if you have a dynamic Crosshair that is or maybe you know stuff which is not essential like effects spawning effects so if you have stuff like that which is not really Mission critical it's fine uh if it's a bit slow and maybe if you don't have too many Loops so if you have many Loops in your code blueprint generally runs slower I will talk about why that is and stuff so what you do is You' have the

04:53:17
core functionality in your base class and then uh you would create a blueprint class which I'm marking in yellow and we you'll call this one bpor rare now this is just a convention I use you could call it anything you could simply call this one rare so this is going to be your blueprint class and this is what you'll spawn in the level so since this is inherited from this B P rare will have all the properties of acpp rare similarly you do that for all the other classes and that's how you would work

04:53:50
hand inand with blueprint and C++ blueprint is going to make your coding a lot easier so it's basically your visual scripting language so it's going to be very simple to write game logic but when it comes to fin a control and when it comes to using other libraries when it comes to doing machine critical stuff you would use C++ so that's basically how you use blueprint and C++ hand inand of course this is a very in-depth topic and we are going to be talking about this in the future now let's actually go

04:54:23
ahead and work a little bit more on whatever we learned till [Music] now so now that we know about the basic inheritance hierarchy let's actually start creating stuff on our own now the first thing which you might want to create are variables now for oure just for reference we'll be using our CPP object. H but anyways you don't have to use this you can you can do this inside the actor as well so stuff like that will remain the same most of the time you will not have anything in the global scope you will create everything

04:55:04
inside of your class itself so the rest of your file maybe if you are creating a new struct or something you would use it but most of the times you will be doing stuff inside the class so let's create a variable now you could do your normal C++ syntax thing so for example let me just create an integer so by using int let's say our integer variable all right you could initialize it here or in the Constructor now one thing that you might know is that since this is private are derived classes hence any blueprint

04:55:44
class which we create out of this cannot access our variable so in order to actually access it there are two ways I'll be showing you guys both the ways so I'll I'll type in our private integer variable because we made it private this is how you would ideally do it I'm just uh explaining you guys each thing but you could uh you could you know brush through if you are already aware of objectoriented programming but anyways it will give you a learning experience nonetheless now another way you could do

04:56:15
it is you could create a variable in the public section so we'll call this one R public integer variable now this is good if you want to access it everywhere however it's really not you know appropriate to do it this way because if you have it in public any other class can just St straight up modify this variable which is not good for us let's say you have something like your uh character speed or something it's very easy to misinterpret that maybe accidentally change the value so

04:56:53
it's better to have Getters and Setters instead now this is how you would work with a public variable I know you guys are still waiting for the unreal reflection system so all these macros which is see U class UST struct U property I'll tell you about all those don't not to worry [Music] now another thing is that since this is private in order for other classes to access it we actually need to define a method so we can call this one int get our private int we called it integer order there so

04:57:36
let's call it like this now we also probably need a Setter so set our private integer now we don't have a function definition so if the reason I told you guys at the beginning that you don't really need to know too much C++ is that once you know how to write the Declaration you could just right click quick actions and you could just create a definition like this same way with our Setter function oh and this has to be void because we aren't actually returning anything you could make it

04:58:11
bull so let's say you have a condition where you can't set it so let's say for a health variable you can't set it to 101 so then you would do those checkings and stuff but in our case we'll just use void head into the file here and instead of this we will return this variable so not public we'll return our private integer variable now this is how you would set it up for the private variable and this is is the proper way to do it also uh currently none of these use unreal

04:58:47
reflection system now if I just run a debugger so it's going to launch the editor make sure it's set to development editor in the configuration so wait for that to build and once it's done building it should start the [Music] editor now in order to actually use this over here and actually check stuff uh in Blueprint so what you do is you right click go to blueprint class and type in CPP object but you see that it's not visible now the reason it's not visible but our actor was visible because by

04:59:28
default All actors if you were to go into this file by default All actors are going to be marked as blueprint table so if I actually head into uh the actor over here and if I actually look into this uclass macro you see it says blueprint table so what we need to do is in our object if we want to use this in Blueprint that is inside this uclass macro type in blueprint table now this is how you expose your U objects to blueprint so let's say anything is not accessible in this menu over here under

05:00:04
all classes it probably means you haven't marked it as blueprint so let's stop the debugger and run it again so wait for it to compile then once the editor loads up we should be able to use our cpor object class so give it a second for it to load and now if I head back into blueprints right click blueprint class cpor object you see that it's usable and this one we'll call it bpor object now if I just write click and if I want to access the function so we have get our private integer so get our and

05:00:48
as you can see there is really nothing the reason is unreal doesn't really know that you want this to come in the editor basically you're not utilizing uh the unreal standard macros which enable you to do it so how you do it is for variables what you do for a public variable here we are going to type in U property and in the arguments we'll use uh a parameter known as blueprint read write now when you put this in the arguments basically what you're saying is you want this to be readable and

05:01:30
writable in Blueprint let's say you only want it to be able to read it you do blueprint read only now how do I know how to do this basically you can just head into your browser and type in U property ue4 or UI oops not properties so yep you property so basically have to go to the documentation page and as you can see there should be a list of specifi somewhere over here there is so all of these are the specifiers so let's say you wanted a function to be blueprint callable you do that there is

05:02:15
blueprint pure as well I'll be showing you guys the common ones but you can have a look at all of these the documentation is King now for a private variable actually we don't need to make this a U property however you could choose to make it now if you want to use these Getters and Setters which will technically you know enable us to use our private variable our get function will be pure of course so we are going to use a u function now now U function is another macro again you could have a look at it so here if I

05:02:51
head into U function over here you see again there is documentation which talks in depth about this we will be looking at the common ones anyways this one will be blueprint pure blueprint pure means those green nodes which we saw without any execution pins so if I actually head into any blueprint these types of notes basically without this execution pin that's going to be our Pure function and I talked a lot in depth about it when I talked about Blueprints and stuff now this one will be a u

05:03:26
function as well and this one will just be blueprint callable all right now we can go ahead and run a debugger now we should be able to to access this now live coding is a bit finicky that's the reason I'm not using it otherwise I would have chose to use it now let me just create that I didn't actually save it so CPP uncore object we'll call this one BP uncore object save that this time if I open it up now and if I type in get our private integer you see we get this function which gives us access to

05:04:17
the value similarly set our private integer also works but it's kind of useless we actually didn't set up any functionality so let's just taking a parameter parameters are pretty simple except references everything else are is going to be the same for parameters like how you do in standard C++ so you could type in int new value and over here as well we could just head into the definition and change that and then we could do our private or our public it should be no it should be private so our private integer variable

05:04:53
equals new value now that should fix things so we should have our logic corrected over there but that's not really Our concern right now now what if you wanted to take a value by reference now this this is pass by value and it will work you could try it out not really going to waste my time to show it if you actually want your value to be passed by reference you use this macro known as upam so upam ref and then you use an Amper sand over here so copy this do the same thing in your CPP and now if I go ahead and actually

05:05:37
build this once again and and in my object if I go ahead and type set r private integer you see it's taking in by reference if you hover over it it says new value integer by reference so this is how you do pass by reference I just showed that this is one thing which is a little different from C++ you can't just uh use an Amper sand however if you use an Amper sand it is going to take it as a second return value in Blueprint basically like your out parameters so let me show you guys what I mean by that so if I do this now

05:06:12
this is wrong logically this is wrong I know that but anyways I'm just showing you guys what's going to happen so if I go ahead and run a debugger once again this time it's going to take it as an output rather than an input if I open my BP object again and if I type in let's say set r private integer you see the new value goes out basically this is how you handle multiple return values as well you could just do pass by reference and in Blueprint it's going to interpret it as an out parameter in our case uh you

05:06:55
param ref was the correct choice so we are going to do that undo this over here as well so that's about it oops just correct that also if you guys want to access access your public variable you can just directly use R public variable so R public integer variable so it's directly accessible to us but one thing you might notice is that unlike these variables here it does not let you edit the default value and stuff now there is uh one reason for that that's because you again need to set a flag in order to do

05:07:34
it uh remember the U property macro or here you have to type in edit anywhere in order to be able to do it so edit anywhere if I can spell that correctly if I actually do this and uh run a debugger once again I should be able to use our public integer variable and set its default value now if you were to see under the class defaults we have an option to set the default value or when we even get our public integer variable you see that we can set our default value so this is basically how you expose that to

05:08:11
[Music] blueprint I suggest that you guys now try it with a few more functions of yourself and maybe you know check how they work in the editor and stuff once that's done let's talk about the next type that is UST struct so basically if you want to create structs for the Unreal Engine you need to use the macroon known as UST struct now generally I prefer doing it inside this H file for your project so you will have a file like this but you really don't need to you could do it in any file so

05:08:53
for example let me just do it in our CPP object. H file it could be really anywhere unreal is going to recognize it for you so I'll just do it above our U class so I'll just type in struct and if you guys don't know what struct is uh well you got to learn that before it's basically like a class but uh by default all its members are public but remember when you're working with uh Unreal Engine you don't really work with struct methods you only work with variables and any methods you'll have

05:09:29
you'll have it in another class as static functions so that's how you work with it anyways I will show you guys what I mean by that real soon so for example example let's just create a struct known as let's say book this is obviously highly impractical but just as a basic example and for the variables we could have maybe a string now remember in Unreal Engine the variable you use is not STD string so you don't use STD string actually what you use is called F string which is unreal string type obviously

05:10:08
most of uh the string types are just interconvertible at any point of time so if you're using a third party library or something you can convert it so F string is the string type in unreal so if I type in F string let's say name and maybe we can have an integer for number of pages and we can have a float for rating all right we have a really basic struct over here now if I go ahead and build this actually so I'll close my edit if I go ahead and build this you would see that it would build

05:10:46
successfully however obviously uh as you would expect you cannot access the struct in the editor because we haven't used the unreal macros so in order to use this in the editor you you call UST struct and inside the parameters what you do is you would make this blueprint type so this is what you use to expose truck to blueprints now if I actually run a debugger right here so you would find that there are a few build errors so what this is is this is not your C++ compiler eror basically there

05:11:29
are a few rules in order to use structs in unreal similar to how you have a u prefix for all structs you need to have an F prefix so now if I go ahead and run this this in the editor it's going to be visible as book you see that we get another error now it says expected a generated body now if you notice our class here it has a generated body similarly for our struct as well for all UST structs you're supposed to be having a generated UST struct body so it's going to set stuff up for

05:12:06
the editor for us basically so now if I go ahead and build this you should see that we compil successfully and we open up the editor right now but you will soon notice one problem again which you probably would have guessed if you would have seen these so the so if I just head into my object for example and if I if I type in let's say I I create a new variable and call this one book one and I get the type book you see I can access this there's no issue but if I right click I can't actually split the struct pins now if

05:12:48
you actually hover over this cannot split the struct pin it may be missing blueprint exposed properties so what it it basically tells us is we actually need to Mark these as U property as well so the same macro can be used here as well so U property and there's a little bit of an issue with the indentation there don't mind so you property again again make this one A U property depending on what you want let's say we don't want to be able to change the name so let's make that blueprint read only

05:13:25
so then we won't be able to change it now if I stop debugging and open the editor once again now if I go ahead and take a look and if I drag this in right click and split R pin I am able to split it now if you drag this in and if you want to edit the members you would use the set members function and obviously you can have number of pages and rating as a parameter and we set name as not being editable since we did blueprint read only as you can see we don't have that available as a pin so this is basically

05:14:03
how you use structs in C++ now the way you use it in C++ is pretty much the same like how you would by the way if you want struct methods you can use them but you cannot write U functions inside struct that's the thing so if I actually go ahead and try it basically I'll show it to you guys so if I head in here type in let's say void test function and I'll just give it a simple body here and I won't do anything now you would see that it will build successfully there won't be any

05:14:34
issues so as you can see it builds but if I actually make this a u function I won't I won't even give any parameters if I just make this a u function as you would see it says U structs cannot contain u functions so how do you actually do stuff with it so how do you actually operate on structs basically what you would do is instead of having the U function here you would have it inside either a function Library class or you would have it inside some other object and make it a static function Maybe so let me actually show

05:15:11
that so let's create a test function so for example let's create a u function here so U function and what we can do is we can make this blueprint callable and over here instead of just declaring a regular function let's do a static function static void test and now we want to operate on this struct so if you want to operate it similar to your objects what you could do is you could simply create your own Target pin so the way you do it is fbook Target and obviously you would make that a reference

05:15:57
so you param and in the brackets you would have ref so you would pass this as a reference and then you could work with it inside so I can write the definition here as well but just to be a bit cleaner so quick actions so whoops quick actions and I can create the definition and now now that we've actually come this far I'll just show you guys how to print strings so it's not like blueprint where you directly just call you know print string and this is not going to work so I can't just do

05:16:38
this so so let's just say test function called for example I actually cannot do this uh the very simple reason being [Music] that in Blueprint unreal actually Imports or rather includes all your headers for you as per necessity but basically that doesn't happen here so so it's not exactly headers but you get the point so in order to use print string so how you would go about searching for functions is you do something like this so you do print string unreal C++ this is how you just search it up and you

05:17:26
would look for the one which says docs. unrealengine.com and you would head in here and it says it tells you the include file so copy this path paste this in not not path rather the include and now you would see you have all the various parameters some of which are optional there are only two parameters which you actually need but anyways now what we can do is now you notice that you're not able to call it but that's because this is actually a static function once again so what you do is you do UK kism MIT system

05:18:06
library and followed by scope resolution print string and now you would see that it still shows an error that's because you actually need to pass in a world context object because it doesn't really know you know where to Output the string like how to show it on the screen so in order for it to know that you actually need to pass in an object if this wasn't a static function you would just use this so if if this were inside an actor and it's not static you would use this but it says this may only be used inside

05:18:43
a non-static member function so what we can do is we can just pass in a u object pointer over here or rather we'll just pass in an actor pointer so a actor pointer now remember when you work in C++ any object any actor anything that you have which is enclosed in a class basically any class if you want to use them you would use a pointer to it you will never refer to it as a actor it'll always be a pointer just remember that so an actor is just to give you know some context to it so we can just

05:19:23
type in context for example it could be an object as well I assume so if I type in context here now we would see that the error is gone but obviously we change the function signature you could make this a u object pointer I believe and now what we can do is we can copy this over head back into our function declaration and put that in so now our error should go now if I go ahead and actually run this now if I head in to Blueprints and BP object or here if I call test for example I think it's called test as you

05:20:10
can see now we can operate on this struct and for the context we can what we can do is simply we can plug any you know outer object in so I'll just actually do that so I'll open up the level blueprint so for the context what we can do is we can go ahead and get a reference to self and for the Target what we would do is we would go ahead and actually get a struct so instead of this I'll just create a struct so I'll just call this struct for example and it's going to be of type

05:20:49
book so we can use that and now this function is going to operate on this struct so this is just a basic way you can do it now if I go ahead and press play after 3 seconds you should see something being printed test function called as you can see that works so that's pretty much how you would handle struct [Music] methods so that pretty much covers the basics of using structs in unreal uh C++ now the next thing is obviously enumerations and that should be about it and then we can start you know working

05:21:28
with a little more complicated things at the base level enumerations in Blueprint and C++ work the same but in order to create them in C+ plus you can do the same thing actually you can do enum this one doesn't really need to have a prefix by the way so for example let's just say fruit uh fruit list let's just call it and inside that we can have our list items so let's say we have apple let's say we have our mango and let's say we have a banana stuff like that make sure you

05:22:08
just end everything with a comma Now again the same thing this is not exactly exposed to blueprint but in order to actually expose this you you use the same specifier as your used struct but instead you type in U enum if you use the U enum macro and if you add in the parameter blueprint type now this would be usable in Blueprint but if you wanted to give it a different you know name for it in Blueprint so if you wanted to give a display name to this basically what you do is You' use another macro known as um meta and over

05:22:49
here you would change display name equals and you would put in the string so in our case uh let's just call this one apple uncore uncore one maybe so just for you just for me to demonstrate that it works now if I actually run the editor and I can just go ahead into any blueprint and I can operate on that so I can say switch on whatever we call that fruit list as you can see instead of Apple it actually shows apple one and mango and banana is just shown as is generally what you would do is you would

05:23:32
simply have the display name to just display exactly what this list item was so you would simply have this and you would have mango over here generally you would just leave it like this banana so this is how you would go about doing [Music] it now we have brushed through the basics of Unreal Engine C++ of course if you want to know what function calls to use for your game playay specific needs you could refer the documentation and later on when we actually take an example we will look into some of the

05:24:13
common ones so it's not really that you have to refer the docks for everything I will be going through many of them now over here let's actually do a quick exercise let's try to translate this into C++ now if you were to notice this entire thing is actually purely in Blueprint and let's say we wanted our code to run faster or for whatever reason we needed it to be in C+ Plus+ so let's actually go ahead and translate that so it's really simple uh let's start step by step so we

05:24:48
have our get player camera manager function let's see which uh header file we need so it says Target is game play Statics right so this tells us that we need gameplay Statics so if I head into Chrome and if I type in game play Statics ue4 or ue5 you see you actually get the documentation page so over here we can get access to which header file we need so Kismet gameplay Statics started so stuff like that let's actually go about doing it now for the cast node we we need a C++ class because all our C++ classes will

05:25:27
not have access to the blueprint classes but all our blueprint classes will have access to the C++ ones so you cannot access a blueprint class from C++ so that's one disadvantage AG now let's go about doing this so I'm just showing you guys one example obviously we will talk about a few of the common ones such as spawning actors and stuff which are really common now let's start in the editor so let's go ahead and actually create the classes that we need so first of all we need a base class for our BP character

05:26:05
so go head into tools new C++ class character and call this one CPP character of course you can name it descriptively if you wanted create the class head back in and we need a couple more things actually so one thing that we need is the pickup class itself so type in actor and call this one CPP pickup all right create the class now what I want you guys to do is head into BP pickup and over here under class settings for the parent class I want you guys to select CPP pickup and over here as well I want you

05:26:55
guys to select BP uh CPP character so CPP uncore character I want you guys to select that now what this basically means is that you are inheriting this BP character class from CPP character so everything that's there in CPP character will also be there in BP character basically this is your inheritance now let's head back in let's just reload this and I think we can close the editor for now or actually we might need that for reference so let's actually open up the character so we need a player camera

05:27:28
manager and from our header file we uh from our documentation we know that we need this header file so inside our character. H because that's where we wrote it always when you're including header files you need to do it above the generated doed so over here Kismet gameplay Statics do and let's just uh do this in the public section and let's have a look so when we press our left Mouse button we get the player camera manager so let's try calling that static function so go ahead uh let's actually create the

05:28:05
function let's call this one I don't know what do we call this so we just tracing and destroying so let's call this one remove pickup or something so void remove pickup all right we don't really require any parameters now let's go ahead and create a definition for it so oops let's just head in and it has created the definition for us so let's go ahead and get that that's a static function so U gamep playay Statics get player camera manager and over here what we can do is

05:28:47
for the world context object since this is an actor characters are actors so you can just use this generally you just use this and player index is zero since we have only one controller per screen so we got the camera manager and from this we need the actor location as well as the forward Vector so what we do is let's actually just store it in a temporary variable so we can type Auto Temp equals and we can store this in a variable and what we can do is we can go ahead and get the actor location so this is a pointer again so

05:29:24
temp with the pointer operator we can get the actor location we have forward Vector here let's do that as well and temp get actor location now this might actually warn us right now uh to use the get camera location function so as you can see use get camera location instead so get camera location just spell that correctly and now we have access to these locations and what we are doing is we basically plugging this into the line Trace what we can do right now over here to simplify things is we have a for

05:30:07
forward vector we grab that in and we multiply it by a float so the operator is already overloaded so we multiply that by 50,000 in our case so let's just do that and if we head back into a blueprint so we add that to our camera location so plus our camera location so you could just do a plus again so plus our camera location we can put these in parenthesis is just to be a little more clear on what we're actually doing so we can delete this line we have that next what do we have is our line Trace so if

05:30:48
you just hover over this you see it says Target is Kismet system library and I know this header file so I'll just do it for you guys anyways uh what we are doing is going to be correct so let's close this up so it's going to be Kismet Kismet system Library you could have a look at the documentation as well so Kismet Kismet system library and if we include that our error should go and if I open up the CPP file once again now we should be able to call the line Trace function so you Kizmit

05:31:26
system Library line Trace if I do that I should find line Trace single and for the parameters we have a bunch of them so first one is the world cont text object which is going to be this again and next we have the start and the end location we look into all of that so this and our start location is going to be our camera location so what we can do is we can actually store this in a variable right now so what we can do is we can type in Auto camera location equals get camera location now for the start we can go ahead and

05:32:12
type in camera location and then we have our end so again we can store this in another variable so Auto end lo location or let's just call this one end equals whatever calculation we just did right there so end and is what we called it then the next parameter we have is a trace type query which is the Trace channel so this is what you see over here now over here uh this is a little bit peculiar in C++ so if I just do eace type query so erce type query and if I take a look you get something like 1 2 3 so on basically

05:32:59
these are what you define in the project settings so if I actually head into my project settings and just type in Trace you would be a able to see that you get Trace channels by default we actually get two uh that is visibility and camera so if we just do uh Trace type query 1 that is going to be your visibility and then if we take a look we have a Boolean for Trace complex we don't really want to trace for complex collisions here so let's just do zero or that is false and over here we have a parameter

05:33:33
which we actually don't need and we also have a few more I guess we'll just use the ones which we absolutely need so actors to ignore we can just create an empty array and we can just pass that in so t a actor pointer and I will get to TRS don't worry basically this is like your STD Vector in uh standard C++ uh instead of that the one used in unreal is called T so all the same functions exist inside this as well instead of dot size you have you know do num uh there are a few names which have

05:34:13
changed but it this is pretty much like your STD vector and let's just call this one ignore and we'll just pass that in so ignore and the next parameter is uh e draw Deb uh debug Trace so basically whether you want to see the line trace or not so e Draw d buug Trace whoops and over here we have for duration for one frame persistent uh let's keep that for duration for now all right once that is done we have our hit result which we are going to Output so we'll just create another variable so F hit

05:35:05
result and we'll call this one uh hit or out hit or whatever and what we can do is we can just pass hit over here and once we have our hit result we have B ignore self yeah we want to ignore ourself and don't really need the trace color because this has a default value so that's about it basically so we can go ahead and close this so I feel these parameters should be enough and once this function is completed we should would have access to everything that we can possibly think of so the first thing

05:35:43
uh that we we are going to do is we're going to cast it to the pickup now in order for us to work with this first of all we need to include the header file so hash include because we don't know what CPP pickup is so we'll just do CPP pickup. so this should compile because it is in the same folder and once we actually include the what we can do is we can simply cast it now you won't use a dynamic cast here unreal actually has some things built in for us so we can get our hit so if

05:36:22
hit dot actor. get actor if this is valid now at this point if we haven't actually hit any actor with our line Trace basically this if is going to be false and we are not going to execute this code however if we have hit the actor we can go ahead and cast it to our pickup so if can go ahead and cast it so this going to be acpp pickup this is how you cast in uh unreal C++ basically you have a cast function and over here we can just pass in the actor so if this actor is valid so again the pointer is going to be pointing to

05:37:03
an actor if it is actually valid in that case what we can do is we can go ahead and and destroy this actor so hit. get actor and we can call the destroy function that's about it and just to make sure what we can do is we can just print it so UK is M system Library print string and over here we can just pass in this instead for the world context object and we can print destroyed a pickup and we can go ahead and terminate that so so now in order for us to actually be able to call this from blueprint uh we'll set up input and

05:37:43
stuff a bit later in Blueprint it has a couple of extra steps uh so in order to expose this to blueprint we'll again use a u function and make this one blueprint callable uh make sure I get the case right and just indent that and now if I go ahead and close my editor and run a debugger now the editor should load up and if we open up our character we can get rid of all this code and I don't know what we call this so we called it remove pickup I don't even know why we call this but we can call remove pickup

05:38:19
remove pickup now if I go ahead and press play and if I left click as you can see our logic actually works and okay this is not a pickup this was just a cube so that's the reason it didn't work but anyways the line Trace works now the reason it's working is because BP pickup is also a CPP pickup because we inherited from it so that's the reason what's happening is when we actually cast it over here uh we are actually successfully casting to our CPP pickup as well even though that was a BP

05:38:56
pickup so that's basically how we translate it now we can go ahead and clear out some stuff this was just for clarity so instead of using the camera location as a separate variable we can go ahead and copy this over similarly for end we could just do the same and if we have anything else we could do that as well so we don't have anything else we can go ahead and close this up we'll we'll leave this temp variable because having such a long line everywhere is going to be a little bit

05:39:33
weird but again you could you could do this so you could just place this instead of temp wherever temp is going to be there you could go ahead and get the player camera manager and do that but in this case actually using temp would be a better solution so we'll just stick with using [Music] temp so we have brushed through quite a bit regarding C++ and as we create stuff we will go through more things now what if apart from a pickup we also needed to cast to some other thing so let's say

05:40:12
let's actually create another actor so let's do it with our interaction actor itself so let's go ahead and open it up not sure where we've used it so let's just hit crlf to find and let's just find interaction so so we are basically nudging it so what we're basically doing is we are again casting so I have to just check where it is so if we are overlapping so that's what we are doing so let's actually remove this logic and let's actually have the destroy logic itself

05:40:51
so remove this and remove this or actually we could keep this now if you wanted to do it with your cast so what you would have to do is you have to cast to interaction actor if this fails uh and then destroy it and this for the most part will work so let me just go ahead and drag that in forget about the C++ logic and as you can see this works and even this works however one thing you might notice is let's say in an actual game obviously you will have many such actors not just an interaction and a

05:41:31
pickup actor so in that case you'll have to perform many Cs and casting is expensive for your computer's performance so the way you get around this is instead of casting multiple times you could cast to an interface and in unreal blueprint there's actually a very elegant system implemented we'll be talking about both the blueprint and C++ versions of interfaces now so in order to handle this problem what we can do is we can actually create an interface so I'll show you guys step by step to implement

05:42:09
this exact logic uh using an interface and we can actually have separate logic as well for both the interaction and the pickup actor so head into your blueprints right click blueprints blueprint interface and let's just call this one I don't know destruct I guess uh generally I have a Convention of calling it BPI uncore and we can call this one destruct pickup maybe all right and we don't need anything for the input but anyways now the way you actually use this is for whichever actor

05:42:53
that needs to be casted to so for example we casting to our pickup and our interaction actor so we would head into both of these and under your class settings under implemented interfaces we can go ahead and Implement BPI destruct and do the same thing for the interaction actor head into class settings BPI destruct basically at at the fundamental level what this is doing is it is inheriting this interface along with actor so basically your interface is also class internally in C++ I will show you guys the C+ plus version which will

05:43:34
make things a little more clear but in instead of doing all this what we can do is we can call destruct or I guess I called it pickup so let's just call it destruct in general to compile and save that so we call this destruct uh now if I actually go ahead and press play I mean nothing's going to happen because although we have destruct as you can see we can't really Define the logic here the way you define the logic is for example we can head into pickup under interfaces right click Implement

05:44:11
event and if I go ahead and just print a string and I can type in destructing pickup and if I go ahead and destroy it so destroy actor and Target will be self and I'll do the same for the interaction actor so implement this event oops paste this in and we can do destructing whatever this is interaction actor so now you should be able to see that both of these different implementations are actually called so if I press play you see our pickup is destroyed and if I actually click on this side our

05:44:55
interaction actor is also destroyed so this is how you basically use interfaces instead of casting basically what it's doing internally even though this looks like we got rid of cast in is instead of casting to our interaction actor it casts to the interface because interaction actor implements that interface the cast is going to succeed and the function will be executed the situation where the cast fails is automatically handled in the engine now how do you do the same exact thing in C++ you may ask it's pretty

05:45:31
simple actually you just use the concept of multiple inheritance in C++ so [Music] tools create a new C++ class and over here what you have to do is Select unreal interface and we can just call this my interface for example and create the class it should load up visual studio for you so just reload that and over here you should be able to see my interface. H and my interface . CPP basically this is where you would write the function definitions and you can go ahead and Define it in your various classes so

05:46:17
what you do is for example let's just have uh this function work for uh both the pickup and you know our uh whatever that was interaction actor so let's say we want this function to work for both of them so let's go ahead and do that using an interface we'll actually get rid of the C++ logic so we'll get rid of that and what we got to do is first of all uh since we are actually casting to the interface here we can go ahead and include the header for that so hash include over here uh we can go okay we

05:46:59
are including pickup already so what we can go ahead and do is we can go ahead and include this interface in the pickup so not after the generated before the generated. H and this is going to be my interface. and over here where you see public a actor put in a comma and type in public I my interface I is basically the prefix which is used for interfaces just remember that so my interface in the editor is going going to correspond to IM my interface in C++ so let's actually write our function

05:47:43
so let's call this void distru maybe and we can go ahead and add in our implementations so we can right click first of all and make this one virtual right click quick actions create a definition for it this is just going to be like your uh default implementation so now let's say we wanted to implement this function in another class it's really simple to do it now that we have a virtual function here we can head into our pickup. H and over here along with this we can type in Virtual void

05:48:37
and I don't know what the function was so I'll just copy this over do the same thing in the pickup and since we are actually overriding a base class method what we can do is we can use the keyword override and now if I go ahead and right click quick actions create a definition head in here and now let's say we do the same thing so let's say we do UK Kismet system Library print string this and let's just say destroyed pickup from C++ and we need to include Kismet of course so let's just do that real quick

05:49:22
so let me just copy this over I just do this in the file so now we can go ahead and actually destroy it so we can say this D destroy or rather you can just call destroy all right so we can go ahead and test this logic but remember it's not going to work for our interaction actor because we again don't have another C++ class for it so let's actually create that too so new C++ class actor let's just call it for example I don't know uh CPP uncore interaction actor okay so we'll create the

05:50:11
class and what we can do is we can again implement this so in order to implement the interface so I'll just stop the editor there so in order to implement the interface we'll do the same thing what we did for pickup so if you head into the header here copy this over head into your interaction actor implement the interface and again we need the header file so what we can do is we can do hash include uh whatever this is so we have my interface. and then we can go ahead and implement this event by using virtual

05:50:48
void distruct which was a function name and we are overriding a base class method so override and now we can go ahead and create the definition for it and over here we can go ahead and print the string again we can do that by simply including kmit again so let me just copy it over oops I copied that so head back into your pickup where we had included it copy that paste that back in and let's just copy over the code from our pickup you can have different code as well I'm just showing you guys

05:51:26
as an example on how to use it so we'll change what we print so destroyed interaction actor from CPP and this should work work also just head back into your CPP file your CPP character and where we cast it to the pickup what you basically do is instead of casting to the pickup you cast to the interface since we inherited the interface so it's going to be I my interface and make sure you actually include the header file I've already done that so somewhere over here we have included pickup. H already and

05:52:02
pickup. H already implements the interface and we have included the the header so we don't really need it so we can cast to this interface and instead of destroying and printing what we can do is we can utilize this so we can have this separately so we'll just do Auto Temp equals I'm I'm doing uppercase temp because we've already used lowercase temp here and temp is going to be valid because the cast has succeeded so what we can do is we can call distruct from here all right now we can go ahead and

05:52:45
run a debugger now if I head back into my character connect this up uh hit play and you should see that we say destroyed pickup from CPP but the interaction actor doesn't work that's because we haven't actually set up the parent class over here so go ahead and change that to cpor interaction actor and we could rename this as well BP interaction actor all right so if I go ahead and press play the pickup works and as you can see destroyed interaction actor from CPP so that's pretty much it that's how

05:53:28
you use interfaces and later on we will also be seeing more practical examples this was probably a good one but still we actually implement this in our actual [Music] game now let's look at another case where you know you want to call blueprint functions from C++ now this almost seems impossible because your C++ classes aren't actually aware of what blueprint classes exists but actually it is it's really simple to so what you do you could use it in any actor any object even in the interface

05:54:11
if you want but I'll just show you guys in the character by just printing something so the way you actually call blueprint from C++ is like this so you just write a normal function so let's just call this void test BP Funk let's say and now what you got to do is you have to use the U function uh macro and you can make this blueprint callable or not but the specifier that you need is called blueprint implementable event so now you can have the function declaration over here you can actually

05:54:53
have parameters too so we can test that if you want so int X let's say so now if I actually run this you won't actually get a compiler error because unreal automatic Ally generates the definition for you and you can Define it in Blueprint so if I open up my BP character and under functions under overridable if you just have a look you will have test BP Funk and as you can see I can actually implement this over here and we also got our input parameter so we can just go ahead and print a string we can either call this

05:55:30
through blueprint or we could even call this through C++ let me show you guys by calling it through C++ so I'll do it on begin play so what was a function called again test BP Funk and you would see that this is actually implemented so let's type in 100 for example and this will work and in the meantime now I would like to show you guys one more thing that you can do I just wanted to show you guys that yes you can actually do this you can actually implement it in Blueprint [Music] but there is a possibility that you have

05:56:09
some C++ code but then you also have some blueprint code which you want to be executed so in that case what you would do is you would use another type known as blueprint native event so we'll just copy over this function and let's call this one test BP native Funk and let's just have something else for example let's say we'll have a float and for this actually what you need to do is you need to have another function called The implementation of this function so that is going to be

05:56:47
what you define in C++ and this is going to be your uh function name in Blueprint so in order to explain what I mean instead of implementable type in Native now if you compile this you'll actually get an error so what you're supposed to do is not create a definition however you are supposed to create an implementation for this so the way you do it is you just copy all the signature and instead of the same function name you type in underscore implementation whoops implementation so what you can do now is

05:57:24
for the implementation you can go ahead and create the definition head into your definition and we can go ahead and print something so let's say we go ahead and print for examp example let's just say C++ implementation called and we can close that in and for a blueprint implementation we can set that up in Blueprint no issues so that should be it now you can go ahead and actually compile this once again so apologies I just made a few typos over here so so let me just just copy Implement

05:58:08
over here so implementation and do the same in the CPP file as well so underscore implementation and now you should have no problems so if we head into a BP character and we can go ahead and override both of them so test BP Funk we can go ahead and print it actually uh this this is our blueprint implementation and we called it from C++ so okay we'll just go ahead and print it we are calling it from C++ so what should be expected is 100 is going to be printed even the native event you can call it from C++ I'll just do it over

05:58:52
here so first of all let me Implement that in Blueprint so Implement that go ahead and just print that that shouldn't be that hard and just grab in our begin play here and instead of okay let's just spawn this let's keep all of this logic and we can go ahead and since we made it blueprint callable whatever this was and we'll just take in some random value now if I compile and if I go ahead and press play as you can see we get 100 as well as our 423 43 printed now your obvious question is why didn't the C++

05:59:37
implementation get called so if we if I actually go ahead and delete this and if I were to press play now we would see our C++ implementation is called but that's not really that useful isn't it unless you just have some sort of a default implementation so what you actually need to do in order to get the C++ version called is right click on the Node and type in add call to parent function now it is going to call the C++ version now if I go ahead and press play as you can see it calls the C+ uh C++

06:00:14
implementation the blueprint implementation as well along with it so that is basically how it works now if I if you were to do this as you can see we call the C++ function along with the parameters of course as well as the blueprint function what you are calling here is actually the blueprint function if it does not find an implementation it is is going to use the parent class version of the function remember [Music] that so until now we actually discussed everything which was foundational in order to actually start developing in C+

06:00:52
plus however we do lack a little bit of knowledge regarding you know the implementation of various data structures in unreal now apart from just using normal variables you would use arrays and Maps there are others such as has sets link list and stuff but for games you would honestly just use arrays and uh Maps most of the time so in order to implement arrays in unreal so you don't use a static array I mean well you could but you don't use static arrays uh you don't really use the STD Vector as

06:01:27
well you could use STD Vector but you can't expose them to blueprint and stuff or you would have to write your own rapper class now if you guys don't know what I'm talking about I'm basically referring to the standard template library in C++ but in unreal instead of STD Vector we actually have another type known as template array or t array so the way you create that so let's create a variable in C++ let's do that in the public section we're just doing it for demonstration so I'll just make a U

06:02:00
property and make this one blueprint read right and and edit anywhere so edit anywhere and over here what we can do is instead of let's say we have an array of integers so the way you do it is you type in t array and as a template argument you would give the type as integer and let's just call this R in Array all right now template array is actually internally something like your STD Vector so if I actually control click on this this is actually a class which implements it and the methods which are

06:02:41
associated with this are pretty simple we will go ahead and check all of these so similar to the STD vector class in standard C++ Tay has a bunch of functions which gives us info about various things so let's actually set some stuff up so in order to initialize this array so what we do basically we can do it in The Constructor or right here we'll do it in the Constructor just to keep things clean so we'll call R in Array equals and within curly braces we can just give some values so I'll just

06:03:18
initialize it with some random values all right so now let's go ahead and look at how to add stuff to this so similar to add and impl we have methods for that over here as well so we can type in R int array Dot add and now we can go ahead and add an item so let's say for example I want to add 12 so our fifth element here that is at index 4 is going to become 12 and this array is going to be resized since it is similar to an STD Vector now similarly also have M place so constructing an element in place

06:04:02
basically do M place this is like a your M Place back function in uh STD Vector so I'll just add in some random element over there now our array is going to be 23 6 43 64 12 and 4 now what if I wanted to remove something so I can type in r in Array and I can remove either at index so do remove I can either remove an element by using the remove function so let's say I wanted to remove 23 I'm want to remove 23 and R in Array whoops R in Array dot remove at is going to let us remove something at a given index so

06:04:51
let's say I choose zero so now it's going to remove six because we already removed 22 so six is our first index so six is going to be removed all right so we did all of these but now what if we wanted to reserve some memory for our array so what if you didn't want it to resize and search for memory so even those functions are available so let's call The Reserve function before all of this so R in Array do Reserve whoops reserve and we can as we can see we have four elements five

06:05:29
six uh and we remove two so we have two so we can reserve four but at Max we have six six elements so let's Reserve six so we can call that and stuff so these are the most common ones that you'll use uh you won't really use all the other methods but again you can just refer the documentation if you really need it now we can go ahead and iterate through this array through a range based for Loop just like how you can with any of the STL data structures so we can go ahead and do a for Loop

06:06:07
Auto we can just call this one element and we can pass in the array just like how you would pass an STD Vector so R in Array and what we can do is we can go ahead and print it out by calling the print string function so UK Kismet system Library print string you know the drill by now so now in order to print an integer you actually use this function which is a static member of the F string class so F string from int is what you use and you can go ahead and type in Ellie here now remember if you wanted to

06:06:48
print a float you would use this function known as sanitize float now it's going to cast it implicitly anyway so even float works for this and you also have other functions for converting between various uh data types you could again have a look at either the the F string class or you could go ahead and just search it up on the documentation so if I actually head in over here so we have our sanitized float here we have to hex blob from hex blob we have we have various functions basically so we have from int as you can

06:07:25
see you can go through this class see the return type and look at what the function does and then you can go ahead and implement it accordingly so now I'm in the editor if I open up my BP character and if I actually head back over here we had made this blueprint read right so we should be able to access our int array so if I just type in our int array so as you can see uh we get it just like any other blueprint variable and since we initialized it in our Constructor we already have certain values now in begin play if we go ahead

06:08:02
and iterate through this so I'll just do that with we'll uh not call this function anymore now we have an idea of what that is so we have already set it up actually so we we've done it over here so we're printing stuff in our begin play in C++ so we don't have to set it up actually so if I go ahead and press play as you can see we have 4 12 64 43 in reverse order that is 43 64 12 and four and let's actually walk through the logic so we have 23 6 43 64 and we went ahead and added 12 and 4

06:08:41
so 12 and 4 should be our last elements and we removed 23 and we removed 6 so our AR should be 43 64 12 and 4 and if we go ahead and look at our logic here and our output so we see that we get 43 64 12 and 4 so this is basically how you use the T array class functions so this is exact exactly the same as your STD Vector but there are a couple differences in the function names and most importantly from a readability perspective all of these functions use Pascal case so it's readable compared to

06:09:20
the standard C++ stuff which uses underscores which is not really that readable so this is how you would iterate through an array obviously you could use a full length iterator but there is no actual purpose to do it as per my experience anyways let's head into the next part now and take a look at how else we can iterate through this through your standard C style for Loop so I won't be actually showing you guys the output since it's obvious that it's going to work so you would just do something like

06:09:51
for INT I equal 0 I less than where now this is where we talk about another method in this class so we do I less than rint array. num this is similar to the size function in the standard template libraries STD vector and we can do i++ so we can just increment I could do I ++ or i+ equals 1 now instead of ell since this is not a range based for Loop we can get R array and we can get the I element now this is going to work exactly the [Music] same apart from array the other data structure that you would use in a game

06:10:40
is going to be Maps well there are link lists and other data structures which you really won't use that very much in games even maps to be honest you just use it maybe a couple of times in your entire project but anyways in order to create a map in unreal basically you you use the type T map so if I just copy out the U property macro and in the next line we can go ahead and create a map and if you guys know about Maps basically it's just a key value pair so for example you can have two strings as

06:11:14
key and value and you could have something like a username password key value pair something like that so let's just create a simple one let's say we map a string to a float so it's case sensitive obviously and we can call this one R map now you can't just initialize a map like how you would initialize an array so you would have to call the add or the Imp Place function multiple times that's just how you would do it so R in Array or rather R map do add and what we can do is we can pass in

06:11:53
the string and the float so let's say pi and 3.14 then we can go ahead and call add once again so we'll just go ahead and do all of this in our begin play so let's just find some other number let's say num one for example let's just grab in a random value now once that's done you have other methods but you aren't really going to be using them for anything but I'll just show you guys how to iterate through this and how to retrieve the key and the value so that's what you'll be

06:12:35
using this most for now let's say you wanted to access an element though you could do something like this so let's just print out uh what the index num one will contain so copy this over and instead of R in Array of I what we can do is we can get our map R map of num one basically num one is the key here and basically by doing this you're getting the value of it so in our case we mapped num one to 43. 4543 and if you want to iterate through this we can use a range based for Loop here as

06:13:21
well so we could just say Auto element and we can pass in our map and what we can do is we can get the element so we'll print this so we'll copy the code over once again so we'll print both the key and the value so let's just create a string variable temporarily and the way you get the key of this so each element in this map is going to be a key value pair so Le is going to be a key value pair what we can do is we can do dot key in order to get the key and if we want the value we can go

06:14:03
ahead and do le. value the way we'll do that here is we'll just append the string so basically we'll concatenate the two strings so what we can do is temp. append and let's just put a colon just for visual purposes and we can do temp. aend and since our uh value is going to be a float we can do F string sanitize float and we can go ahead and get our value so Le do value that is going to be a float now we can go ahead and rather than printing this we can go ahead and print in temp so we also learned how to

06:14:43
concatenate strings on the way so this is how you would iterate through this this is how you would get a key of a given element in the map and this is how You' get the value now remember you cannot have two keys of the same value so let's say I actually create another uh element with the key num one it's going to throw an exception you can't actually do that so now we'll actually stop printing our array now that we're done with that so if I go ahead and run a debugger now since everything is set up now if I

06:15:18
go ahead and press play you would see that we get Pi 3.14 and num1 43. 4543 and as you can see we also get our 43. 4543 uh that printed first because we had printed our map of num one so basically the key here is num one and we basically asked for the corresponding value it is just as if you asked for R in Array of one it's pretty much something like that so basically instead of the index you would pass in the key that's basically how you use this operator here now this is basically basically how you iterate through it now

06:16:07
you could you know do many other things with a map but for the most part You' just be using it to store key value pairs generally it's useful for having a track of you know game users and stuff like that they're really very odd odd use cases for maps you wouldn't really use it that often so I'll leave this over here [Music] now when it comes to designing your game once you're actually aware about all the things that we just discussed over here up until maps in order to actually

06:16:47
Implement them in an appropriate and efficient manner you would use the classes which the engine provides us so we'll be going through some of the most important ones which will be used in all of the games and there are other derived classes of it the ones which I showed you guys in the flowchart previously when I showed the inheritance hierarchy those are the ones that we will be discussing in detail there are other classes we'll just be brushing through few which whichever are important but if

06:17:21
they're not we are going to be just skipping through them but if we ever use them in the last part of the course we'll be having a look at them in depth once again so now let's start talking about actors now at this big beginning of this video I actually talked a little bit about actors basically anything that can be placed in the level is an actor so that definition still holds good but it is incomplete there is another thing which an actor can do and that is it can tick now you guys have probably seen the

06:17:55
tick function so let's open up an actor actually let's create one because all of these have their own base classes so let's create a pure actor in Blueprint we'll do one and see ++ as well pretty soon or actually we probably have it so let's call this one bpor a let's say I just created this for the sake of it now if I were to actually have a look over here you would see that you have three tabs and the event graph is where you worked on for the most part but we haven't actually gone in depth into all

06:18:30
of these little details so first let's actually go from the top so what we have here is the class settings and most of the times you'll just use it to implement an interface or change its base class but other than that you aren't going to be using it now under class defaults you have a bunch of things which actually Define what an actor actually can do now if you were to look at actor tick you have several options start with tick enabled tick interval and you also have several other

06:19:04
things now we did talk about this one so I'll I'll not be talking about that but anyways all of these are self-explanatory and one thing which you won't see in any other type of blueprint other than actors is the replication tab basically if you check this replicate stab this actor will be eligible to be used in multiplayer what I mean by that is that when you spawn this on the server which we will get to when we talk about multiplayer basically all your other clients can see too by clients I'm

06:19:37
referring to players in this Con context and we have settings regarding that now these are just the flags these are pretty self-explanatory hidden in game and visible stuff like that and under the Collision tab these are things which we again talked about but there are a couple more things which an actor provides us the first one uh is your damage now if let's say you have you wanted this actor to be destroyed so let's actually do that let's go ahead and create an object so let's add in a

06:20:14
model here so let's say we add in a sphere I don't know uh maybe simulate physics on this or let's let's leave it as is what we can do is unreal actually provides us with default logic to apply damage to this so if I type in event damage you see we get three of these nodes Point damage radial damage and any damage so any damage is going to refer to all types of Damages Point damage is going to be your damage through a line trace or something generally radial damage is going to be something where

06:20:53
you know you damage this actor through a grenade or something like that so you would have you know a distance and stuff like that so if I just press this so you have your origin so that's going to be where your grenade landed for example so it need not be a grenade could be anything else just give an example so from that point uh if as you go further away your damage is going to decrease stuff like that so let's just do event any any damage so any damage what we can do is over here we can go ahead and simply print this out

06:21:31
rather just to demonstrate that that this actually works now by default unreal does not give you any health variable you got to do that yourself and one thing you might have noticed is this little icon over here at the top right hand side of any damage basically that property is called blueprint Authority only what it means is that you can only call this on the server so you cannot call this on the clients obviously you don't want your players to be handling the damage and stuff but anyways let's

06:22:04
actually go ahead ahead and work on this logic so when we left click we do the line Trace thingy so let's bring up the line Trace logic once again so what we can do is we can line Trace by Channel and we get our camera manager get player camera manager get the actor location this is some stuff which we've already done then we get the forward vector and we multiply this by a certain value so let's just convert this to a float and let's multiply this by let's say 50,000 we are going to add

06:22:49
this together and we can plug that into end and the start and from our out hit we can go ahead and call apply damage so there are multiple nodes apply damage apply Point damage and apply radial damage we do apply Point damage you could just do apply damage and base damage let's just give it a value of 30 or just to keep things a little more interesting so Random float in range so let's just say anything between 20 and 50 maybe so it's just going to select a random number and damage actor

06:23:28
is going to be the hit actor obviously and damage causer is going to be self damage type is something we won't be talking about and hit info we could just pass in this whole hit result so what we can do is instead of doing this we can recombine this pass this in here and we can go ahead and break this separately so type in break and pass the hit actor once again to the damage actor and we can collapse this as is hit from Direction basically uh that is going to be something which isn't really going to

06:24:06
affect your damage but once you know the damage doctor's location you can actually find the direction towards it basically so what we can do is you can do something like this so basically use this node called find unit Direction so unit Direction so get unit Direction so it's going to be from our start to our location and this is going to be our hit from Direction so basically uh this is a position vector and this is a position Vector as well so we can subtract it to get uh a vector joining those two points

06:24:49
basically and now it should compile if you really don't want to use this you can go ahead and split this and this is going to work as well it's just going to construct a vector in place so we'll recombine that and use that and and if I go ahead and press play nothing's going to happen but if I actually drag our BPA here and if I go ahead and press play so as you can see we are applying some random amount of damage so not sure why the lag exists but anyways now once that's done the next

06:25:31
thing that an actor provides us and also just one one more note here so now we're talking about the blueprint version of this we'll also look at C++ stuff a bit bit later there are a few things that I would like to go over in C++ as well so the next thing is hit events now remember we had done the overlap for a character so somewhere over here so similar to that you also have hit events so you just type in event hit and this is how you set up hit events you also have hit events for each

06:26:05
individual component so if I click on the sphere if I scroll down I can actually do on component hit as well that works too now other is going to be the actor which actually hit this and other component is basically the component of the other actor which hit it my component is going to be the component in this actor which actually hit the other actor and hit location is the hit location of course and we also get a hit result so way too much for what you need so that's generally the reason why when I actually

06:26:42
work on these things I I just create an interface myself because generally you really don't require all of these things in order for your damage logic to work anyways I'll show you guys how this is going to work so if I just go ahead and print this and one handy node here is you can actually get this and if you can type in get display name and you're going to get the display name of the object basically if my character bumps into this so let me do that real quick okay I can't it's too high so

06:27:16
let's bring that down so if I actually bump into this as you can see you get BP character the reason it's printing it so many times is because we are in contact with it for quite some time so when we are in contact and we are sliding on it each each frame it counts a new hit basically that's the reason it's happening all right so the next thing that I would like to touch upon when it comes to actors is the construction script so this is similar to your default Constructor in C++ now there is a way to

06:27:50
actually uh get an equivalent of a parameterized Constructor I will get to that both in Blueprint and C++ but first let's work with this so let's say I drag this in now every time I update this actor the construction script is actually called so let me just show you guys so if I just go ahead and print string and if I go ahead and move this actually so first let me compile that save it and now if I head back as you can see every time I move it it actually prints hello basically every time you

06:28:25
spawn this actor or you update this actor in the level this construction script is called at runtime it's only going to be called when you actually spawn it but over here in the editor whenever you move it it's going to be called each time there's actually an option somewhere in the class settings so run construction script on drag so you can disable that if you don't want that to happen so it's it's only going to call it once you finish placing it I'll just leave it as this now if you

06:28:58
want a parameterized Constructor basically let's say you wanted to set a variable so let's call this uh I don't know maybe some float variable and we'll make this of type float now if you want to actually set the value of this outside like a parameterized Constructor first select this variable and head into this option right there select instance editable and expose on spawn now what you essentially done is you basically exposed this when you actually call the spawn actor function

06:29:35
so if I just head into my character and spawn this on begin play so I'll just leave this BP pickup and let me just do this actor instead so bpor a now Health points is not a parameter so you can alt click that to delete the pin now as you can see we can select some float so I can set this to whatever I want now this is something which we touched upon however there is an equivalent of this in C++ as well but it is a little more complicated than this so if we actually head into our Visual Studio

06:30:17
solution all right so now that we are in C++ now let's actually test it out with our CPP uncore actor so let's go ahead and spawn this from our character or if we have anything else we could try that as well so interaction actor maybe yep we could try that so we can spawn our interaction actor now if we go ahead and head in here inside our characters header file so we can go ahead and include that as well so hash include and we can go ahead and include CPP interaction actor. now let's actually create a

06:31:02
function or we can do it on begin play so head into begin play now after we are done with this or we can actually just remove this logic we aren't really using this the way you spawn actors in C++ is by calling the spawn actor function from world so in order to get your world you call this function known as get world and from here you can go ahead and call spawn actor and this actually takes in a template argument and this is going to be the type which this spawn actor function will return so

06:31:41
this going to be a CPP interaction actor and we could just spawn it like that it's going to take in all the default parameters you can actually set up sub classes and stuff so let's say instead of CPP interaction actor you wanted to spawn some derived class of it which is there in Blueprint you could do that totally so let's say I wanted to spawn BP interaction actor and not CPP interaction actor so we can actually test that theory actually so BP interaction actors spawn I mean the spelling doesn't really

06:32:17
matter here so let's delete whatever it's there in the level so BP interaction actor so interaction actor so I'll just go ahead and delete that now if I press play I'm not really getting that so what we can do this is going to spawn your CPP interaction actor but if we actually have a variable here which stores the exact class which we are spawning so we can do that right there so U property make this one edit anywhere and make this one blueprint read right as well now what we can do is we can go

06:33:01
ahead and pass this in so the type which you use is T subass of and obviously we are looking for a derived class of acpp interaction actor so we'll just copy that over so this is going to be prefixed with the name and we'll call this one class to spawn or rather we can call it actor to spawn now this will be available to us in our blueprint now one thing to remember you have to make make sure it is actually valid so if our reference is valid here so our subass basically so if this class

06:33:45
reference so if actor to spawn is valid only then we are actually going to be spawning this actor and over here in the arguments list you can go ahead and pass this in and paste this in and you can also pass in a transform optionally but I won't be doing that now let's actually pass in some parameters so if you want to pass in a parameter using your deferred spawn actor as I would call it as the function is called so we can actually do that with the same thing so let's create a variable here which we would want to

06:34:25
edit so under the public section we can go ahead and create a U property we don't need this to be blueprint read write or anything so we can call this one in some variable and the way you would set default values for this is if I go ahead and write the function again so this is how you spawn an actor here you would have uh what's going to be returned so if I actually do Auto Temp equals spawn actor interaction actor basically this temp will be of type acpp interaction actor pointer so a pointer

06:35:07
to this Pond actor will be uh returned now what what we can do is we can spawn another one actually so we'll just do Auto Temp one equals we can just go ahead and copy this and instead of this we can do spawn actor deferred and just make sure you get the spelling right so spawn Factor deferred so for this one we have to pass in the transform so we can just uh write a Constructor over here so F transform and that should compile but once you call this function the actor is actually not spawned now since we have a

06:35:56
pointer to our actor we can go ahead and call this function known as finished spawning so if I type in Finish spawning this is going to actually complete the spawning process now you can just again pass in the default transform so once this is done our spawning would actually be complete and in between this is where you can actually set your variables so you don't have a parameterized Constructor but now we can go ahead and set our some variable so some variable equals 100 obviously temp one and now what we can do is in our

06:36:40
interaction actor we can go ahead and just print it on begin play so you Kismet system Library print string and we can go ahead and continue with this and go ahead and print in F string from int and we can pass in our value Val here so some variable is what we want and that should be about it now if we go ahead and run a debugger here everything should work as expected just make sure you close the editor before you actually build it so so now if we go ahead and press play we shouldn't see any print strings and

06:37:34
this proves that our if check here is actually working if we would have uh removed this if check our engine would have crashed since this actor to spawn class reference would be invalid anyways we can set that since we have exposed it to blueprint so in our character I assume so this is in CPP character so it's going to be inherited into BP character and under your class defaults over here you should be able to find your variable so CPP character under the third section here actor to spawn and we

06:38:12
can select our BP interaction actor if I go ahead and press play now as you can see we get two prints along with one Z and 100 for our spawned actors now the first one says zero because in our first spawn actor function we actually didn't set any of the values so this was our classic spawn actor and in the second one we actually used the Deferred spawn actor which let us set the default values before calling the construction script so this is basically how you would simulate a parameterized Constructor in Unreal

06:38:50
Engine in both blueprint as well as [Music] C++ now the next class that I would like to mention here is going to be the character class and we have used that quite a bit so if we just open up our BP character for example which is a character class so we have inherited it from CPP character just to keep things clean I'll just create a new character here and let let this just be call new character maybe now open it up now if I were to just look at the parent class it says character and character is actually a

06:39:33
derived class CL of Pawn so basically every character is a pawn and pawn is a derived class of actors so when I'm talking about characters I am collectively me referring to both pawns and characters basically every character is going to be a pawn now the reason why I especially wanted to mention this even though this is technically just a derived class of actor and probably probably many other classes which I'll mention further are derived class of factors is due to this character movement component now this

06:40:09
allows you to do various things now if you were to just go ahead and look into these parameters you can actually have a pretty basic idea on what you can do at the beginning of the course if you remember I had mentioned that you can actually use functions to modify almost any of these values not all but most of these values at runtime so for example now let's just take our BP character for example and let's go ahead and press play and we know that we're using this so we're walking forward but what

06:40:44
if this feels a little bit too fast for you now this is where our character movement component is going to help us so the maximum speed of this character is actually set by a variable inside here so if I just drag this in and if I type in set max walks speed as you can see we are able to set some value over here so I'll just do this on begin play you could do it somewhere else as well but let's say we wanted him to go only at 500 default is 600 by the way now if I go ahead and press play you

06:41:20
see that he moves a little bit more slowly now if you feel this is a now one more thing is that the animation will also slow down along with his speed so that's not something which you should really be seeing in this example so we are moving slower let's say we wanted him to move a little more fast so let's say we have 1,000 we can go ahead and set the speed and now we walk much much faster so stuff like this and one more useful thing which the character movement component provides us is movement modes

06:41:53
so if I just type in movement mode and get movement mode you can actually see this is an enumeration we can just do a switch to see what are the enumerators here as you can see we have walking nav mesh walking which is for AI basically falling swimming flying and custom now there are various things you could even do with this uh apart from switching between them you can actually set the movement mode so for example if I just change this to Flying for example and if I go ahead and press play now you'll notice that this behaves

06:42:33
a little little bit differently now if the movement mode is flying if I go further as you would see he's actually floating in the air so when you actually set this movement mode to Flying basically it also allows you to take vertical movement input so apart from your move forward and backward you could also do up and down so let me actually do that so where we have our add movement input instead of forward if I do up vectors so get actor up Vector if I just do something like this and if I go ahead and hit W as you can

06:43:12
see we can actually go up and down as well so this is something cool which you could do and there are a few functions which I would specifically like to talk about right now and one of them is launch character launch character so let's say I wanted to implement a jump pad or something so let's just do it after a delay so delay of about 2 seconds and we can go ahead and give something for the launch velocity let's just give 10,000 maybe now if I go ahead and press play as you can see we were launched in

06:43:50
the air I mean I just gave a really high value for the launch velocity uh let's say we give something like 3,000 maybe if I go ahead and press play as you can see we are launched in the air so if you had something like a jump pad or something which you wanted to implement this is a really cool way to do this and the best part about all this is this is actually networked by default most of this logic if you just run on the server is just going to run well for multiplayer as well so that's one thing

06:44:24
so launch character and stuff like that there are actually many other functions which you would have access to one way to actually take a advantage of the context sensitive menu is if you just drag off of self and if you can just head into character you can actually look into various functions over here this is what I find useful you can apart from launch character few more functions which I would like to go over are Crouch so if you set your movement mode to crouch and make sure you have you can

06:45:01
Crouch so there should be an option somewhere here so Crouch should be under character movement can Crouch make sure that is true otherwise it's not going to work make sure this is true and if you go ahead and hit Crouch and one thing that I would like to show you guys is by setting this hidden in game to false so let this be visible in the game now if I go ahead and take a look at this as you can see everything seems normal here let's actually just disable some of this logic all right so I'll go ahead and

06:45:42
Crouch so if I go ahead and Crouch as you can see our capsule whatever we had is actually shrunk this is basically our Collision now so let's say you couldn't pass under some things now you can actually so I'll just drag this a little bit B below average character height so let's say about this much and now our walking speed is also very less even though we set it to 1,000 manually now as you can see our Collision is only up to the capsule you can change the height by the way so if I

06:46:20
just type in Crouch I should find Crouch half height you can actually increase that no issues with that and as you can see now this has a separate Max walk speed so stuff like this is already implemented for you in the end engine now all you have to do if you really want to learn more is just browse through this list just look at something which might be useful so let's say you're doing multiplier you could have a look at this now this is not something which would would really be that helpful

06:46:49
to be honest but there may be a few settings which you might actually find helpful now there are many many more things which you can do and if you aren't able to actually write a certain mechanic using these 9 out of 10 times you're just doing it wrong it's just one out of maybe 10 20 times that the engine is actually deficient of features so just like this you could go ahead and explore this for yourself all of those parameters which we saw in Blueprint are also accessible in C++ there is nothing

06:47:29
special really so for example let's say I wanted to crouch so I can just typee in Crouch as you can see the method Crouch exists here as well and not only that if I want to access my character movement based functionality there is actually a get function for it so get character movement is the function name so this is going to return a U character movement component pointer so once we actually have access to that so let's say Auto Temp 2 equals okay it's in a different scope so we can reuse temp so

06:48:05
Auto Temp equals get character movement and now we can use this variable in order to just call our regular functions so for example if we want to change a movement mode so we can type in whatever the function was over here so movement mode so set movement mode was the function name set movement mode now clearly it's not happy with us using this type but fix for this poter to incomplete class type so the simple fix for this is to just look up the documentation for the header here we don't have the character movement

06:48:51
component header file so we'll just paste that in our do H and now if you go ahead and look at this this should work and now we get the options for the parameters so for this let's actually type in E movement mode and we have move flying for example and then new custom mode we can just set this to zero so like this you can set the movement mode in C++ so stuff like this is going to be analogous to both blueprint as well as C++ however note that some of these headers aren't actually included by default so

06:49:38
make sure you just go ahead and include them before you start working with [Music] them so we are inside the BP player controller class and we have dealt with this before but going a little bit more deeper player controllers or controllers in general are designed to handle input so if we actually bring in an input binding so for example I just type in w on the keyboard so what's going to happen is this input will actually be taken over our input bindings which we set up in our character so if I just print a

06:50:20
string we'll actually not move instead we'll be printing hello so that's one thing to note other than that the mouse interface has several important functions such as show Mouse CER enable click events enable mouse over events and stuff like that all these are self-explanatory one thing to note is that your Pawn or your character obviously is going to be possessed by a player controller and without a player controller you can not actually control your character and all of these are actually set inside your game mode so

06:50:57
which player controller class you use is decided by your game mode class which we will talk about soon game mode game State player State and player controller all of these work in conjunction a player controller is going to possess a pawn which you can control now once that's said there are a few of the functions which are important here such as set input mode game only which will take your game input basically and when you have set input mode game and UI only so in that case you are going to be able to interact

06:51:30
with widgets as well as take player input in the game similarly UI only is going to disable your keyboard input entirely so stuff like that functionality regarding input is available in your player [Music] controller despite using all of the above mentioned classes it is technically impossible to set up a well playable game so we have a few more classes which actually set up the whole framework to actually start developing the game logic itself and those are game mode game State and the player State now

06:52:15
the player State isn't that important but the game mode and game state will provide you with all the functionality that you need in order for your gameplay logic to work so we have already created a game mode know that every level will have one game mode and you have to set that and the important part here is these classes these can be set over here in the world settings and pawn class is as as expected BP character however this can be changed at runtime in the sense you can possess a different Pawn the default

06:52:51
is going to remain the same but you can call the possess function on your player controller so let me actually show that so let's say I'm on new character right now so now I can't move or do anything however if I head into my game mode and let's say after begin play I just give a delay of few seconds so delay and I give let's say 3 seconds or 2 seconds and I get my player controller now note this is a single player game so this works otherwise anything that you do will be with respect to the the

06:53:33
server game mode in a multiplayer game will only exist on the server that's one thing to note so from here we can type in process and what we can do is we can just spawn a character so where our player start is we can just copy this over let's say or we can have a Target Point instead so just type in Target Point drag this in and get the location so we have something like 10 11,420 so head into the game mode class spawn actor select BP character for example so bpor character and for the

06:54:29
transform 11,420 and we'll do 350 for the Z and for the pawn this is going to be the pawn which we will possess now if I go ahead and press play wait for 2 seconds and as you can see we have possessed our BP character so stuff like this you can easily set up in your game mode so anything such as this which is handled on the server is done in the game mode but the game mode isn't really limited to this the game mode has several functions such as post login and you also have other things such

06:55:21
as on log out so this is basically when you join the game in a multiplayer game this is basically when you leave the game or you disconnect so you'll still have all the references available to you so that's where you'll use the game [Music] mode so basically you'll use this for stuff which is Court your game logic however let's say you wanted to store something like a timer now the timer has to be in sync with everyone so obviously it has to be on the server but all your other players must be able to read it at

06:56:11
least so in that case you use a class known as game state which does the exact same thing so if I just type in game state I'm going to use Game State base game state is basically game State base with a few extra functions so let's call this one dpor game state oops BP game State open it up and ignore the viewport and stuff doesn't really matter and once you have this over here we can have something like a match timer so I'll create a new variable and call this one timer so I'll make this of type

06:56:53
integer or here we can go ahead and start the timer so set timer by function name we can go ahead and create a simple custom event here so custom event and we can go ahead and call this one for example timer increment and we can copy the name paste that in we want it to run every 1 second we want it to be looping and it has to run till the end of the game so we can do timer Plus+ now this uh value of timer over here can be read by your widgets and stuff like that so there's actually a function which you

06:57:36
can use for this so let's do that in our widget head into your UI HUD BP HUD and where we have our stuff set up so let's actually revert our character uh settings so change the character to BP character and here for the spawn actor as well we'll remove that for now for now we'll forget about it oh here where we actually create our HUD this is where we have our reference so what we can do is we can actually create some more text here so we can type in timer so whoops can type in text drag in some text here maybe just

06:58:24
increase the font a bit and we can go ahead and have this to be light anchor it to the top right hand side and instead of this we can go ahead and set this to be whatever the timer is so in our game state every time this happens we have to update it so what we can do is we can get our player controller here we don't have a reference to it currently so get player controller we have to cast it to our BP player controller cast to BP player controller now we can do this on begin play and we can store a reference in a

06:59:10
multiplayer again this is not going to work obviously so promote this to variable and type in PC ref maybe for play controller ref we can go ahead and update okay we have a update Health function we can create an update timer function so custom event update timer and this should work as is so give the timer value to this so type in timer get a reference to your HUD make sure this is variable and we'll call this one timer text make sure you compile this so timer text set text and we can set this to be whatever

07:00:03
this timer reads obviously you can use format text and you can make this show minutes seconds and stuff like that so we have our timer so we can do format text so format text we can have minutes colon seconds something like this so make this in curly braces and our timer by 60 is going to be our minutes and our timer mod 60 is going to be seconds however we also have one more parameter which we need to take care of is if this value is less than 10 we want to append a zero at the start so divide

07:01:03
so rather convert this to a string first so two string and once we have the string we can check if this is actually less than 10 and if it is less than 10 we can use a select instead so select so if if it is true and if it's false we need separate things so if this is going to be greater than 10 which means this is going to be false so we directly want to print that out but let's say this is less than 10 we want to upend a zero here so upend type in zero and then we want to print the seconds so some simple logic

07:02:00
like this now we you can go ahead and test this out and if you were to look at the top right hand corner it does not update because we have to set the game State as well so if I just select bpor game State over here and if I go ahead and press play this should technically work but it's not so let's have a look under our BP game State we have our player controller and we're actually not calling the update function so update timer now this function should work as normal so the timer is going to be the

07:02:37
value which we get over here and on begin play we can just set the timer to zero so we'll just call the update timer function once I go ahead and press play as you can see our timer works and it increments every second and if we just give it a little bit of time so we have a runtime error here we'll take care of that so it says assist n trying to read proper property HUD this so this error is in our player controller the reason is uh when the game state is actually created the player controller isn't actually yet

07:03:13
created so that's the reason why or rather the player controller is created too but the HUD is not yet created so once this begin place called our HUD is created so a simple fix for this is to get a validated get and if it is valid we are going to set this text and we shouldn't get any errors now anyways as soon as we create this HUD we can go ahead and update the timer whoops update timer and we can set it to zero for a timer variable we can actually set it to some higher value right now so that we

07:03:53
go ahead and test out the minutes part of it so let's say set this to something like 65 it should start at 1 minute and 5 Seconds so 1 minute and 6 seconds 7 8 9 10 and our logic works properly so for stuff like this you would use the game State now the game mode is going to drive the actual logic itself behind your game functionality but let's say you wanted to access all the players information you would do that through the player State class so I'll just be vague about it and if you right click in your game State

07:04:30
and type get player array you can actually get an array of player States so you can actually Loop through this in fact and we can get stuff like the player name so get player name and for multiplayer games you can get the unique net ID so for these things basically any details which all players need to have access of at all points of time those are the things which your player state will hold so that's about it basically and one last class that we have left to talk about which is important is going to be

07:05:10
our game instance then we can head into more advanced stuff and we can have an example project [Music] created unlike all the other classes which we spoke about till now the game instance is kind of special the game instance behaves very differently compared to all of these classes so if I actually just open up my game mode for example so we'll open up the main menu first things first maps and our main menu level and now in my uh game mode I'll just go ahead and print stuff so I'll just print post

07:05:52
login and I'll just type in log out maybe so log out and we can also have event destroyed event end play so we'll just go ahead and print stuff over here as well so destroyed I'm just doing this in the game mode but this could be in any other class and this is going to be end play all right so if I go ahead and press play right now and if I go ahead and press play as you can see our post log was called and as soon as I close it or rather I should switch levels because if I close the game the logic isn't

07:06:41
really going to be executed so I'll just type in open main menu level as you can see our log out function was called so what I'm trying to say here is that this game mode class will not persist between levels so once you log out this game mode reference whatever we have is not going to persist now forget about the game mode reference you can't even access it from anywhere else so let me actually show you guys using the game instance the special thing about the game instance is that when you switch

07:07:20
levels your game instance will still remain the same when you open up the game an instance of the game instance is created so basically an object of type game instan is instantiated and that is going to remain the same so go to blueprint Class Type in game instance and over here we can name this our game instance or rgi anything you want you could put a BP underscore you can have a C++ class as well but I don't really find the point in having a base class for this one now instead of begin play you'll actually

07:07:58
find event such as event in it so this is when your game actually starts so if I go ahead and print this out if I type in in it and if I head into my project settings type in game instance I can actually change this to BPR rgi if I press play and if I press play again or rather I'll head into the level and do it if I press play you would know notice that in it isn't even printed here in the console but it was printed way before everything else that's why it's way down at the bottom over there the reason is

07:08:44
even before the viewport was properly spawned and even before it started logging stuff the event in it was actually called so the event in it basically refers to when you start the game not when you open up a level or not when you create something else now one thing which I want to show you guys is I'll head into blueprints head into our game instance I'm going to go ahead and call the get game mode function and I'll go ahead and promote this to variable and let's not name it it's

07:09:18
fine and then what I want to do is after a while so let's say I switch from one level to the other now I'm going to go from this level to the main menu level so I'll head into main menu level and in the level blueprint here I'll just access the game instance get game instance and we can cast it to BPR rgi this can always be a pure cast because it will never fail and over here get whatever the variable was called I think it was called new variable zero and we can go ahead and right click and

07:10:00
convert this to a validated get we can go ahead and print it and we can say not valid and this is going to be if it is valid so valid so if I go ahead and I'll actually leave a bit of a delay here oops delay let's say about a second not more than that so if I go ahead and head into my level again and if I press play as you can see everything works normally but I'm going to go ahead and type in open main menu level and as you can see I get not valid so what this exactly means is that our

07:10:49
game mode object which was created when we loaded the level because game mode objects are specific to a given level as soon as we change the level our our BP game mode object was destroyed and whatever game mode we had over here in our main menu level so this is none so it's just going to take game mode base so that object was created however our game instance was still the same so if I actually store a reference to the game instance somewhere else that is still going to be completely valid throughout our game so

07:11:26
anything that is persistent between levels you would have it set in the game instance generally you would handle save games and stuff like that through the game instance because even if a player exits a level your save game logic and stuff should be able to work and stuff like settings and all those things are what you would put inside the game instance anything related to file handling will also be put in the game instance and many other things regarding networking uh in general outside the game is going to be

07:12:01
in the game instance for example a database you could handle it through the other classes as well but this is going to be the safest way since this class is going to have itself instantiated throughout the program in in our case the game and even when you actually exit the game we have event shut down rather than event destroyed or event end play so if I just type in print string and if I just exit nothing's really going to happen because the viewport is already destroyed by the time the shutdown is

07:12:36
called so stuff like that let's say you had to close out some connections or something you could do that through your event shutdown let's say you have a database or something like that just give give an example anything that's persistent between levels you would use the game instance and one thing which should be obvious by now but I wanted to mention is each player in a multiplayer game will have his own game instance and you cannot put in-game networking code in this you can put networking code but

07:13:09
whatever is outside the game if you have any in-game networking code you there is absolutely no reason to use the game instance there is no use of calling uh rpcs through the game instance since one player's game instance is in no way related to the other players game instance so if I actually start two instances of the game Let's let's say I have two players even though they may be connected your game instances will be different so this player will have a different game instance unlike the game State or the

07:13:46
game mode where it's going to be common for one game so let's say two players are connected both of them will have one game mode and game ST in common which will be created on the server but in a game like this game instances will not be the same so I should have done listen server or client so stand alone even in Standalone even game mode game State and classes like that will be different because in stand alone you are not actually connected but in any case your game instances are never associated with each

07:14:20
[Music] other so with all the knowledge that you have now you should be able to create an entirely complete single player game in Unreal Engine 5 of course you will need to refer the documentation at times at times you will need to mess around with stuff but this much of knowledge should be enough for you to create a complete Game completely functional game using all of unreal score features however I am aware that I didn't touch upon particle effects and audio that is sounds uh we will take a look at that

07:14:58
when we actually create a practical game I am not a VFX art nor I'm a sound design person personally so that's the reason I didn't touch over them but we will go over some resources which you can use and I I'll just talk about what I do to actually get hands on those resources now that's done we can go ahead and start talking about plugins until now we just implemented plugins which were there in the marketplace or if you have a plugin from GitHub or something you would download it and

07:15:30
maybe just paste it inside your project so if I had in here you just create a plugins folder and paste that in there that's simple but what if you wanted to create your own plug-in if you wanted to do that and this topic is very less discussed so not many people actually talk about this stuff so you're in luck because we are talking about this in detail now so head into plugins click on ADD and you see many options now we won't be worrying about the editor plugins those are for more advanced users and if

07:16:06
you're in a state where you're creating editor plugins I really don't know what is the reason for you to watch this course so we won't be touching upon this we'll be looking at third party libraries later on we'll be looking at blank content only and blueprint library now blueprint library is self-explanatory it'll just contain a blueprint function Library let's say you wanted some functions for a vector or something maybe you implementing another data structure for which you want

07:16:33
functions you could have a blueprint library and content only is basically the type of plugin where you know you would have models and stuff like that without any code basically but the one which we'll be doing is blank and just give an author name in my case I'll give gamium and description this is my first plugin well it's not but just for the sake of giving a description and let's call this one test plugin and go ahead and create it so the plugin has been created and we have Visual Studio open however before

07:17:11
we actually start working on it I want to touch upon one topic that is the build. Cs file basically everything you have in the engine is divided into modules so the core functionality of the engine is like core core U object and engine so now that you have actually created your plugin your plugin as well will have a build. CS file if I actually open the folder over there so plugins test plugin uh and if I head into Source test plugin I have a build. CS file here and I have content binary stuff like that so what this

07:17:50
basically is is this plugin itself is actually a module in itself so if I want to use this plugin in C++ let's say I should go ahead and include that module so I can do that by typing in comma and we can type in test plug-in this concept will be more clear once we actually Implement a third party librar uh when we Implement a third party Library you actually have a separate module for the library as well as your plugin as a whole basically your plugin acts as a wrapper so that it can interface with Unreal

07:18:27
Engine because unreal standard API does differ a little bit compared to your standard C++ what you do generally so you'd use the plugin as sort of a wrapper to you know interconvert type so let's say you wanted to convert all the STD strings into s f strings which is there in unreal so stuff like that so you would have the plug-in as a wrapper and you would interface that uh through the plug-in inside the engine so let's actually take a look at our plug-in now now that we have a basic

07:18:58
idea of build. Cs in our editor we already have our test plug-in content folder open we can work with this normally but anything we created uh inside here will be actually packaged inside our plug-in so for example let's create an actor class so let's just call it some actor and whoops and we can make it do something let's say so for example let's say we have some logic so let's say every frame it just prints out something obviously you would have some more practical logic in here so let

07:19:41
me go ahead and type something so let's say our actor is sticking something like that and we could go ahead and have C++ classes as well so over here under Tools you can create new C++ class I'm just showing you guys how to do it because we did go over the blueprint itself so you know how to work with blueprint it's just that you're creating it inside this directory and I'll show you guys how to reuse it in another project so head into tools new C++ class just like how you would let's say you

07:20:23
wanted to create an interface so I just took an example and instead of my interface we can call this one one uh our plug-in interface and instead of beginner course you can type in test plug-in because this is a separate module in itself and now if I go ahead and create the class You' see that under our source or rather under our plugins folder so I'll just reload the solution under a plugins folder under the source folder now you should be able to see our interface so now you can work with this just like how

07:21:04
you would with another file so this is how you would actually go about doing it so now if I just go ahead and close this and rather I'll just close the editor and remember guys make sure your plug-in is enabled here if you're are not able to see it in the editor make sure you enable this so what you can do is first of all let's see if it actually buildt successfully so we'll just create a u function so it's going to be a virtual function because we want to override it so virtual

07:21:44
void test function and we can go ahead and leave it as is we don't really require a default implementation but we'll have one anyways so right click quick actions and create a default implementation and now we should be able to implement this interface so let's make this a u function so U function U function and just to make our job a little bit easier we'll just make it a blueprint implementable event so that we can actually just give the logic in Blueprint itself so this works and now if I just go ahead and

07:22:29
build this you should see that both this plugin as well as our whole project will be actually built so it says blueprint implementable events in interfaces must not be declared virtual let's just fix that and now it should build as is just make sure you don't have a definition here because it will look for the definition in Blueprint now let's say I wanted to use this in another project this is how you would go about doing this so open up your editor head into the plugin section again and

07:23:11
where you have your plug-in over here under project other click on package just select a random folder I'll just select my documents for example and go ahead and package the plugin it will take a little bit of time but once that's done you should be able to to implement that in another project so meanwhile while this is actually compiling we can go ahead and create another project so open up your epic games launcher so our packaging is actually complete before the launcher loaded up so you can actually check it in our

07:23:48
documents folder so head into test test plugin and you should be able to use this in your projects and I'll show you guys how to do that so just ignore that head into Library let's actually just launch the engine as is and over here we can go ahead and just create a new project so we'll just create a blank project blank with nothing I'll just create blueprint and for the project name uh okay we do have a C++ class so it might actually want to rebuild stuff once again so anyways what we'll do is we can

07:24:27
create a C++ project call this one plug-in test and we can go ahead and create it so I'll show you guys how to implement it both in Blueprint and C++ anyways now that we are actually in the process of creating it so it should take a while but eventually once the project is opened up we should be able to import the plugin just like that and I'll show you guys what steps you need to take in order to actually get this in the plugins list now our project has been created so we are in a blank level just we'll just go

07:25:07
ahead and create a new map and let's just call this one some level open it up save it and make this the default project settings maps and modes make this the default so that should be good and if you open up your Visual Studio which we will open later we'll close this up and close the editor as well and beginner course will just minimize that for now if I head into my file explorer what I can do is I can copy this over and where I have my other project so I believe I created it under unreal

07:25:48
project so plugin test and what you want to do is you want to create a new folder called plugins and paste this over there now what I want you guys to do is right click generate Visual Studio project files so this is actually going to integrate it and once you're done with that if you want to use the plug-in content in C++ all you have to do is head into Source plugin test and under plugin test build. CS we don't actually need to come here actually this is for the plugin what's the plug-in using so what you have to do

07:26:28
is head into your plug-in test rather and I mean the project head into Source plugin test build. Cs and over here so I meant I meant to come here so over here what I want you guys to do is where we have our modules I want you guys to add test plug-in uh just don't get confused plugin test is our unreal project name and test plugin is our plug-in name and now I'll show you guys how to implement it so we can go ahead and build this once again so we'll close everything up and we'll just generate the visual studio

07:27:11
project files once again and we'll close our beginner course we'll open it up and we'll just create one C++ class and maybe a blueprint class so we'll do blueprint first since we are opening the editor anyways so we have some level and if we actually go ahead and and create something so let me just create uh an actor if I head into all classes and if I type in so I'm not sure what I called it so we can head into plugins and check test plugin content Su actor so Su actor as you can see we get

07:27:47
some actor now if you're not getting this it simply means that you haven't enabled it in your plugins so under installed other you should have test plug-in and you should have your author name and stuff like that so make sure you have this enabled over here and now if I go ahead and drag this in the world and if I press play as you can see our code which we had in our actor is now working in the other project similarly we can use the interface as well so over here under class settings implemented

07:28:21
interfaces we can go ahead and look for our interface I think we called it our plug-in interface and we have our test function which we can Implement and we can go ahead and tell something so you could just say test function called in order to implement this however we would require C++ since we actually didn't make this blueprint callable however we can still choose to edit it in the source over there so if I just head into our source and if I actually go ahead and edit the CPP file we can actually rather uh in the plugins

07:29:07
folder test plugin if I head into the source folder and edit the CPP file or rather the H file and add the blueprint callable specifier I would still be able to you know use this over here but anyways we will implement it in some class which we create here so I'll just go ahead and close Visual Studio here and I'll go ahead and create something so we can create a new C++ class of type actor we are able to implement this but we can't call it that's the reason we are actually doing

07:29:43
it so we'll just call it my actor for now and go go ahead and create it so live coding should do its thing so our file should in fact open up in a new window window right now and go ahead and just don't mind it opened up in a separate window and now we can feel free to go ahead and include our interface just goone ahead and reopen the solution file here uh now inside my actor. H since we included the module in the build. Cs file we should simply be able to include R plugin interface. h now you should be simply able to inherit

07:30:33
the interface by using public I are my R plug-in interface and now we have successfully inherited the interface now the since this was a blueprint implementable event you can just go ahead and use it in Blueprint itself and just to make things a bit convenient for us we can head into our R plugin interface. H file under the plugins folder and we can add in the blueprint callable flag so now we can go ahead and actually call it from the blueprint so we can go ahead and run a debugger now so this is how you implement it in

07:31:09
C++ my main intention here was to show how to include the header file rather than using the interface that is something which we already covered so wait for the editor to load and once the editor loaded in what we can do is we can go ahead and create a new blueprint class and we can remove this actor first of all otherwise it'll keep printing our actor is sticking so go ahead select actor we'll leave this at new blueprint one add this and under the parent class or we could have done it over there itself we'll select my

07:31:46
actor and now again we have our test function and we can again go ahead and Implement our event so we can go ahead and print something let's say test function called or we could have gone ahead and inherited uh my actor instead of some actor here but then again you would have to change some other stuff so we'll just redo this and now if I go ahead and press play nothing's going to happen head into your level blueprint and for example just go ahead and get a reference to it and now if I just call

07:32:23
in test function test function message this is what we want and now now if I go ahead and press play you see we get test function called so this is basically how you do it guys so this is basically how you would use a plug-in which you made and implement it in another project and as you guys saw you can absolutely feel free to edit the plug-in contents once you have pasted it in this plug-in [Music] folder now let's move on to third party libraries now there is one thing to understand before we actually head into

07:33:05
implementing them and that is that there are differences between your standard C++ API and the unreal C++ API a very simple example would be the difference between STD string and F string so in unreal you would use F string whereas in standard C++ you would generally use STD string no interconverting between them is really easy easy so if you want to implement a third party Library the way you would do it is you would build your third party library inside of a plug-in so basically you would put it in a

07:33:42
separate folder and I will show you guys the procedure so nothing to worry about that and the the unreal plugin which you will create will act as a wrapper to kind of you know interface between the standard C++ and unreal C++ API so the way you do it is again create create a new plugin first select this third party Library template because it has most of the important things that you would need in order to actually set it up so again I'll just put gamium for the author and I'll just call it some third party

07:34:20
library library plugin and over here we can just call this one tlore Plugin or something like that that so third party Library plugin so go ahead and create it so now this dialog box should appear over here or rather message box and we'll just click open or okay so basically that was just some code which was written in the example library now over here we shall not be using their Library so they have actually provided us with a library which we can use as a reference so if I add into plugins TPL plugin Source you

07:35:06
see there are two folders here now third party is the folder where you'll have your third party library and TPL plug-in is the folder where you would you know have your plug-in content and anything uh under this folder would be edited in your project solution file and I'll show you guys what I mean so right now head into third party third party plug-in Li plug-in Library so what we can do is over here as you can see there is an example library now whichever file says example Library dot something that is basically

07:35:49
our actual third party Library so in order to implement our own third party Library we can go ahead and delete whatever they have put over here so we don't need any of this so this is just an example and what they have done is they've used a dll but I'll be showing you guys how to implement a static library and a dll separately so we'll do a static one first so I'll just go ahead and delete all of this now what we left with is a blank uh folder with just the build. Cs file so what do you

07:36:23
want to do now is open up visual studio and over here you can go ahead and create a new project of type static library and click next and we'll just call this I don't know test third party library or something so test third party Library so we'll create it under a g repositories or rather we'll just select our solution folder so we'll go ahead and select our beginner course head into the plugins folder TPL plug-in Source third party third part TPL plug-in Library select this folder and

07:37:14
what we can do here is we can check Place solution and project in the same directory so we would have all those project files as they appeared in the example so go ahead and press create now you should see that our library is actually created so if I go ahead and open up this folder over here as you see this folder has been created it's not necessary that you have it over here so you can just go ahead cut this and paste this over here and you can go ahead and delete this folder so it's open in visual studio so

07:37:58
I'll just close everything so I'll just save it so we can just cut this and paste it over here so we shouldn't have opened that so we'll just replace it as of now nothing should happen now once we're done with this we can open up our build. CS file and over here you would notice that we have a bunch of stuff which you seriously which I seriously don't expect you to understand uh basically these are for Linux and Mac so you can just go ahead and delete these I'm not going to

07:38:34
be showing how to work witho files and stuff so I'm not really a Linux guy so we'll just be working with our Windows Library so we'll not do the dll now so I'll just comment this out we'll do the dll a bit later and what this is is this is basically our uh uh Library directory and the library file itself now example library. lib was the file which they had created so whatever example Library they had that file was named example library. Li but ours isn't yet here so we can just go ahead and add

07:39:18
in some sample code so that we can actually create it so head in here change the configuration to release first things first and head into source files add a new item and over here you can go ahead and create a do hedge file because we will need some sort of a header to include it so we can just type in test class we'll just create a class so test class. maybe we can create some static method inside and over here uh we can actually move this over to the header file section right click on source file add

07:39:59
new item head of uh Source CPP file and we can call this one test class. CPP and once both of these files are open over here we can just start writing a class so we can call this test class and under the public section we can simply have a method so under public and under private we can have a string variable so STD string and we need to include string obviously so hash include string so we have our STD string we'll just create a variable called maybe test string and we can write a Constructor

07:40:50
here to just initialize it so what we can do is we can go ahead and create uh test class and write the definition for the Constructor the reason I'm not doing it in line over here is because I want to show you guys that the lib file is actually doing something so if we have the definition right here so we wouldn't really need the library file now I can go ahead and create the definition for it and what we can do now is under this we can go ahead and just initialize our string so we can say test string

07:41:36
equals this is some test string doesn't really matter what you put in there and we can just have a method so we can have STD string get name maybe now this is going to return that string basically so we can go ahead and test that so we can go ahead and return test string now this should be about it for this so before you go ahead and build it just set up this pc. hedge file and stuff so go ahead over here instead of test class. H just include this pc. H and what you would want to do is you would want to come here and just include

07:42:22
your test class. over here so now this should compile so if I go ahead and press build make sure it's in release configuration and it should work so now if you were to head into your TPL plug-in Library folder now under this x64 folder which has been created you should find your lib file don't worry about all these other files just go ahead and copy this file name which will be the same as your library files name I mean your library's name so test thirdparty library. Li that is the file

07:42:56
which we want to include so so now that we are done with this now we should in theory be able to wrap this using our TPL plugin now this is actually the code for our unreal plug-in now inside this we'll actually be writing some code in order to just wrap this class whatever we wrote over there so go ahead and head into your beginner course solution that is your main project solution and now if you head into your test Plugin or rather the one which you created now so TPL plug-in Source TPL plugin and we should be able to actually

07:43:47
work with this so we'll just do it inside this header file uh as I I showed you for the previous plugin if you want to add in more files and stuff you can do it through the project or we can actually do that since we have our solution open anyways I mean our unreal project so over here we can go ahead into tools add a new C++ class we don't really require an actor so we'll create an object so object create it and we'll call this one wrapper object and this will just be under my TPL plugin so we can close our solution

07:44:27
since it'll open it up once again and and create the class now if you were to open up your solution you should see a wrapper object. CPP and stuff and one more thing uh this is something which you really don't need so now you can just feel free to head into this function here and just delete all this code and over here as well you can go ahead and just delete this make sure you just have the functions and for this one basically we don't have our example library. we instead have our test class. H so this

07:45:02
will work we don't need it here so we aren't going to use it so we can just leave the rest of it as this and now if we were to continue now but now if I were to go ahead and build this so if I just go ahead and hit build now wait for it and now you'll notice you actually get errors even though you didn't have any code uh the reason is well we don't actually have our U object module if you get any errors like this cannot open include file and it something like this basically it's the same thing you

07:45:39
haven't included the module so what you have to do is head into your uh TPL plugin under Source you should find your TPL plugin build. CS file and if you were to recall your main build. CS file that is your projects build. CS file so if I head into source course beginner course beginner course build. CS you see there is a module known as coreu object and this isn't there in uh the TPL plug-in build. CS so I'll just go ahead and include that and now it should build successfully so if I

07:46:13
just click on build now this should build with absolutely no problems so now we can go about implementing a wrapper object basically we are trying to get our test class to work with our actual code here so I'll just do it under the public section so whenever this uh U object that is U rapper object will be instantiated I want our actual third party Library object to be instantiated as well so we can go ahead and type in test class class obj equals we had a default Constructor so we'll just call that and the reason

07:46:52
we get errors is because we haven't included the header so we can get TPL plug-in Library so library and we call it test class. now we shouldn't get that error now we should be able to create our object and now we can go about writing our functions for it so the only difference in the main with the standard C++ API and unre API in our example is that we used STD string over there but we want to use F string so we can write a u function for it so so youu function we can just call it get name and the return type is going to be

07:47:34
F string of course and we can create a definition for it create a definition open it up and inside the F string Constructor we can get our object obj doget name do cstr so C St strr so this is how we can just convert it now this is is something related to the conversion you can just look into the documentation or the Forum so this is how you would go about converting it and we'll make this one blueprint callable as well just so that we can test it in Blueprint and now successfully we have translated our

07:48:15
standard C++ function in our third party library and this is now usable in unreal so if I just go ahead and run a debugger here inside a project now we we can ignore this and we can head into content and we'll just do it under blueprints go ahead create a new blueprint class and this will be of type wrapper object so we don't find it and we forgot to make this blueprint table once again no issues we can make this blueprint table and you can make it blueprint type as well if you wish so we can go ahead

07:48:55
and restart the editor now and now under content blueprints if I right click create a blueprint class and type in rapper object we should get a rapper object and we can go ahead and just call it bpor rapper so this is our rapper class basically now if I were to actually go ahead and call the function we can actually do that so we'll instantiate the object and call it so our function was called get name oops get name call function get name Target is rapper object and we get a string so we can go

07:49:38
ahead and test this method out so in our level blueprint we'll just construct an object so we can ignore this we can go ahead and construct object from class and we can construct our rapper object so BP rapper we didn't really need it to be honest but anyways we can go ahead and call the function get name once it successfully constructed and we can print strings so that we can check if it works so now if I go ahead and press play as you would see I get this is some test string and this is exactly what we

07:50:21
put in our third party Library so if I head into third party test class. CPP as you can see we had our STD string and we actually called this method through our rapper class so this is basically how you implement a third party static [Music] Library so now let's get to DS now working with dlls is going to be a little more tedious and if you were to take my opinion in on real engine at least it's it's really not worth the hassle to work with dlls I always prefer just working with you know static

07:51:05
libraries or any unreal native plugins but anyways I'll just show you guys with the example itself the procedure is the same head into to plugins click on ADD third party library and we'll just call this gamium and plug-in name let's just call it dll test so we're going to create the plugin and it should take us into visual studio so we get this message box here so which is from uh the functions given in the dll so just head into your solution Explorer and under your uh plugins you should

07:51:49
find your dll test plugin and if you open up your third party folder you should be able to see the code now we'll just be be modifying it in here so we'll just call a function so example Library function let's just head into the definition they're just creating a message box similarly we could just have our own function the important bit over here is the export part so basically you have this macro which is going to export the function now the usage of classes isn't really covered here so I'm just going to

07:52:27
do that instead of WR wrting my own function obviously you can implement the same thing with your own dll but remember uh the changes to the build. Cs files which you have to make so under plugins dll test Source dll test or rather third party dll test library and in this build. CS file again you will probably have to change a few parts you can remove this if you're working on on windows so this is over here just change the file name to whatever your dll is and over here for the lib file as

07:53:07
well just make sure you change it to whatever your file name is even here as well just do those changes and you should be good to go and the addition of modules will still remain the same so you will still have to include core you object and stuff we'll do that so not to worry so if you want to actually export a class you would have to do it right here in the H file you can have the definition separately in the CPP file but I'll show you guys how to actually do it so the way you do it for classes is a bit

07:53:42
different for functions you can follow this example and move on but over here let's say I want a class so I can do example Library export now I am assuming we are developing for Windows so I'll just go ahead and delete all these ell so I won't be having any of that so I'll only have the uh macro declared even over here as well so I I'll just go ahead and remove all of this and I'm just assuming that everything is for Windows so with that assumption let's continue now if you want a class we can

07:54:21
go ahead and declare it and one more thing in your H file as well make sure you just have this macro if you want to work with class if you're working only with functions you don't really require so now what you want to do is let's just call this one test class and over here we can go ahead and have some methods so let's say int get num or something and we can have a variable as well so under private we can have int num and for this we can go ahead and provide a definition for it and one more thing

07:55:05
for each definitions so for your class definition here make sure you put in export for methods you would put in import here and export in the definition but since your class definition is here itself make sure you have example Library export or whatever your library name is and we can just go ahead and return num so what we can do is we can write uh we can just say we can just set this to some value uh what we can do here is we can write a Constructor actually so this class is called test class and we'll just write it in line

07:55:46
over here what we can do is num equals can grab in a random number between 0 and 99 so this should work as expected and then our get num function should work as well now once you're done with this our dlls example Library should work so what we can do is we can go ahead and before building actually we can create a new file so head into your editor and we can close the solution for now we can build it and close it so we have live coding enabled just ignore that so build it so this should build

07:56:35
successfully now if I just head back into my project beginner course and if I head into my U project file here once it loads up you would see the message box as is if you don't want that I'll just show you guys how to disable that if you don't want the message box head into your dll test third party third party library or whatever or rather uh Source dll test private dll test.cpp this is the file where it's actually uh given the function definition so just go ahead open that and edit the file to remove the function

07:57:15
definition so let it open up and over here what you would want to do is you would want to remove this function definition so you can remove this and then the message box isn't going to pop up can remove this as well but that's not going to be called unless it fails so not to worry and even this path as well so if you do require to change it you will have to change it if you're implementing your own make sure you account for all of these so heading back go to tools new C++ class all classes

07:57:53
object we'll go ahead and just or we can do actor just to keep things a little more interesting so we can go ahead and create an actor click on next my actor make it uh under dll test and we can go ahead and create the class so this should open up our solution file and don't mind if live coding fails we'll just close and reopen that not to worry we can go ahead and open the solution file once again so we'll go ahead and close this and once the solution is open we should be able to go ahead and find our file

07:58:34
here so under dll test private dll test.cpp or rather my actor. CPP and we should find all our function definitions and not to worry if you get so many errors it's just to do with the build. Cs file once again it's kind of dumb but that's something which you have to deal with so over here make sure you include Eng and make sure you include core U object make sure you have these two modules if you want to access Kismet and stuff like that you'll need engine if you want to access your U object type you'll need

07:59:12
core you object so if you don't have an idea of what contains what you can go ahead and have a look at the engine module in the documentation everything is given over there otherwise you could just follow along so head into now it will build uh intell sense isn't uh refreshed yet so head into your my actor. and we can go ahead and include a header so we can go hash include dlore test library and our header is called example library. of course if you have your own header that's going to replace this and

07:59:51
we shouldn't get any sort of errors here and over here we can just write a function we'll just do it in line so U function make this one blueprint callable to make things simple so blueprint callable and we can call this one void run dll function so I'm not really bothered about the name too much and now what I can do is I can go ahead and write a definition for it we'll just do it over here so from our dll we can go ahead and grab it so the function which we had was called get num so we can go ahead and

08:00:34
instantiate an object to that class so our class was called test class just call it obj and we can go ahead and call the function we'll do it in the next line and obj do getn we can go ahead and print this by typing in UK Kismet system Library print string and we can just pass in a disp pointer and we can do F string so it's an integer so from int and this should be good to go now what we can do is we can include Kismet because we don't have the print string function here so hash include

08:01:22
Kismet Kismet system library. now now this should build successfully assuming we haven't made any mistakes here now it's giving us an error it says test class class type redefinition a simple fix would be just to do pragma once so pragma once and this should build now with no problems now we can go ahead and open up the editor so once we open it up we won't get the message box now because we had disabled that and over here if we just head into a level blueprint for example and make sure under the play mode just

08:02:03
change this to Standalone because we had it set to multiply we can go ahead and construct an object from class or rather we can do spawn actor since it's an actor so my actor my actor is what it was called and we can just have a default transform it doesn't really have anything and from this we can go ahead and I'm not sure what the function was called so let me just have a look so our function in my actor was called run dll function so we can go ahead and call that so run dll function So in theory we should get

08:02:44
stuff printed over here but this will probably not work now because we haven't actually compiled our library itself which is kind of stupid so head into dll test so third party DL test Library example Library dos solution uh now just click okay and now what you would want to do over here is go ahead and select your release configuration and go ahead and build it oh and yeah make sure you close the editor when doing it that was the error which we got right there now if you were to go ahead and open up your beginner

08:03:25
course U project once that's loaded in now we should be able to call the function and it should work as expected so in your level blueprint where you called it run dll function and we can go ahead and click on selected viewport and as you can see we got 95 if I go ahead and play we get 66 and we keep getting random numbers every time so our dll actually worked but if you do want to imp Implement your own it is going to be a little more complicated than this even with just including the one which was provided to

08:04:06
us with unreal it was a big hassle so make sure you guys uh avoid using dlls I prefer using static libraries or I restrict myself to those for unreal at least so that's it I guess about third party libraries we can go ahead and talk about multiplayer now it's going to get fun guys [Music] now let's talk about networking in Unreal Engine so networking basically in unreal revolves around start topology basically your server client model so basically you have one player or a dedicated machine which acts as a host

08:04:54
which we call the server and you have all the other players which are clients now there are two types of servers in Unreal Engine one is a listen server and another one is a dedicated server in a listen server the server itself acts as a client as well as the server that is the host whereas in a dedicated server the server only acts as a host and does not have a player controller so these are the two types of servers and basically any data that has to be passed through through Network as you can see

08:05:29
in this diagram here there is no connection there is no direct connection between two clients always if data has to be passed from client 1 to client 2 or vice versa it has to be routed through the server so that is one thing to note when it comes to networking in Unreal Engine now there are many questions which might might arise regarding the efficiency of this and stuff but most games these days work based on this principle and it is in fact very robustly implemented and we will be talking about all the features

08:06:03
of unreal networking [Music] soon I have brought up my main menu level here and I just want to demonstrate how you're going to join two Standalone games that is two games on separate computers into one so if you aren't familiar net mode will basically let you choose between the type of servers which I talked about play as client is your dedicated server basically and play as listen server is going to be a server which is also a player along with the other clients play Stand Alone will basically mean two

08:06:41
separate games and that's what we will be doing now what if you wanted to connect between these two so we'll be using the game instance for it so open up your BP game instance now I am recording this a little bit later so that's the reason you may see a few things with which you haven't seen so BPR rgi and we can just set up a couple of custom events we'll first of all delete all of these we don't need this so I'm not sure we may have broken some reference doesn't matter so we'll just

08:07:14
go ahead and fix that so we'll just delete that and now if I head into rgi and I'll create a custom event now basically connecting to a single game is hand handled by something known as a session so every time your players are connected unreal actually has something known as a session stored internally we aren't going to be diving into the C++ part of this we'll just be doing this in Blueprint but please note that if you want finer control over these properties you would want to work with

08:07:50
C++ so session is basically what is going to allow your players to connect so let's go ahead and create a session so so what we can do is we can do something like create Lobby would be inappropriate I'll just call this one create session and we'll go ahead and type in create session and as you see there is an async task over here and if you guys aren't familiar with this clock symbol and a node like this this is an async task and public connections we'll just set that to two for example so two

08:08:24
players and player controller this is for listen servers if you have a dedicated server you don't have to pass in the player controller but in our case we are passing it in so we are going to use the function get player controller and then use Lan is set to false you could do it if you wish and upon success what you can do is you can go ahead and load a level so open level and we can go ahead and open our beginner course level all right right and then what we can do is we can go ahead and create a function to join join

08:09:06
session or I I would call this one create match so that it sounds a little more familiar join match so what we can do is we can first of all find sessions so type in find sessions these are the only few functions which are there in this Library so that's the reason I'm not really going over them that much so we can get the player controller and what we can do is Max results you can just set it to something like 100 and we're going to check if it's a failure or if it's a success so what we

08:09:44
can do is first of all we can get the length so if it's a failure we're just going to print something so we could say failed to join a match and what we can do is we can get the length and if it is greater than zero we'll go ahead and just join the first session obviously you can have your own logic here so each session is going to be one hosted game basically so let's say there are three uh uh three members in this array or three uh elements in this array what it basically means is there are

08:10:30
three people hosting a match right now that's what it means so now what I can do is I can grab the results and I can get a copy of the first one if the length is greater than zero and I can go ahead and type in join session all right and here we'll again need to pass in the player controller and note whoops and note that you can only run these session functions either on the player controller or in the game instance you cannot run them on other blueprints it is simply going to fail now once that's done let's say we

08:11:11
have no sessions we can go ahead and create a match so create match and on success we don't need to do anything engine will handle it for us over here you can have something like a progress bar or something until on success is called you could probably have some throbber or something like that to show that it's loading same over here so this should be good and something very simple which you could do is inside the main menu so on clicked what I can do is instead of opening it I can grab a

08:11:48
reference to my game instance so I can type in get game instance which is a static function and I can cast it to BPR rgi this will always succeed I'll just cast it over here I'm not going to bother storing a reference to it as of now and I can go ahead and or actually I'll just do it the right way so I'll just call this one main GI you could call it anything it's just a reference to our game instance and once we have that we can go ahead and use it and we can go ahead and join match so join

08:12:23
match now that that's done if I go ahead and press play if I go ahead and just play here as you can see nothing is really happening but after a while we go ahead and join this session basically we load up the map now now that we have actually created a session and if I press play on the other game here and if I just wait for a while so you would want to disable the input during this time but anyways for now we'll just not do anything you would see that you actually don't join the session session the reason is you

08:13:00
actually need to be listening for incoming Connections in order to actually be able to join the game and I'll show you guys how to do that over here where you have open level make sure you just put in listen under the options so make sure you do that before you actually do it and one more thing plain editor is crashing my game for some reason so I'm just going to go ahead and I'm going to uh run this Standalone so Standalone game and Standalone so play Standalone and I'll play this as a

08:13:35
standalone game so I'm not really sure why the issue is happening but this is one way I can test it so if I press play on one of them and if I go ahead and wait so we should land inside a session as expected we are in the level and we are able to do stuff now I'll just go ahead and click on play here in theory if everything is set we should in theory land in the same map so as you can see post login was called on the server and if I were to notice my client has successfully connected over here so as

08:14:13
you can see I'm able to play the game like this so this is basically how you connect to clients now let's actually talk about how to set up stuff in multiplayer guys [Music] okay then so if we want to work with multiplayer what we can go ahead and do is we'll start with a new level because if I go ahead and press play with two players here and if I actually close the game you see we'll get a few runtime errors now this is mostly because our code isn't really set up for multiplayer and

08:14:50
you will soon understand why so basically now what I want you guys to do is head into your Maps folder create a new level and we'll call this one multiplayer testing so go ahead and open it up so this should be a blank level so I'll just grab in a sky and grab in a directional light here and we should have everything set up and maybe if we want we could have fog and we can just create a simple landscape so head into your mode selection landscape and we can go ahead and create it so I'll just do a little bit of noise

08:15:44
so that we have a starting point so that we have some sort of a workable landscape so increase the brush size so the strength is a little too much 05 should be fine so let me just go back okay that should be good for us now what we can do is we can go ahead and talk about multiplayer so the main aspects of multiplayer in unreal are replication and remote procedural calls if you are clear with how to use these two concepts it's pretty simple to code a multiplayer game in Unreal Engine it's

08:16:36
much more difficult to do it with general knowledge of networking but with unreal framework it's really very simple to set up multiplayer we'll discuss both blueprint and C++ aspects but first the basics now I want you guys to head into blueprints and under here I want you guys to just SE select your character and your BPA so I guess this one is where we had physics enabled so if we do yep we have physics enabled so I want you guys to just show the problem with just running multiplayer in general so I'll just go

08:17:18
ahead and drag this in and what I can do now is I can go ahead and grab a few players starts here so I'll grab one here grab another here and make sure they're all facing the same direction so what I can do is I can make this one 1990 so they're all facing towards this ball right there and now what I'm going to do is I'm going to change the world settings to use our BP game mode and for the player controller we can ignore that we'll still get the runtime errors so what we can do is we can

08:17:57
remove this logic so we'll forget about the HUD for now and if I go ahead and press play now you see the ball has fallen down and it's rolling down the hill over there and as you can see I kicked the ball but if you were to notice the ball is in a completely different position so the ball is over there for me and if I actually head near the ball here you'll see that I'm not actually going near the ball on my other screen so if I actually turn around my character is somewhere there and my ball is somewhere

08:18:38
over there so as you can see both of these are not in sync now this is something related to the widget nothing much to worry about so basically what I'm trying to say is that these two games which are running on separate windows are not in sync but you notice one thing that your characters are in sync so for example if I go ahead and run forward and if I go ahead and run forward over there and if I actually look up you would see that my characters are in sync it's just that the physics object over there is not in

08:19:19
sync so the reason this is happening is because in our character if you head into your class defaults and head into the replication tab you see that these two flags called replicate movement and replicates are enabled basically this is unreal's way of telling us that or rather asking us whether we want this particular class to be in sync with all players when instantiated so let's say we instantiate a BP character it will always be in sync obviously there are conditions you have to instance it on the server we'll talk

08:19:59
about servers and clients soon so let's head into our actor and try to fix it so head into your class defaults and let's try enabling replicate movement and replicates if I compile and if I go ahead and press play as you can see now the ball's rolling down it's near me and as you can see this seems to be in sync if I go ahead and and block this as you can see this is almost completely in sync now uh one of my characters flying is due to the movement mode just ignore that but as far as I can see everything

08:20:42
is in sync so this is basically how you get stuff to go in sync in a network game in unreal this is the most basic aspect of it you might see that there are a few more Flags here such as always relevant call pre-replication Net load on client most of these aren't really important we'll just talk a little bit about net C distance squared and net dorcy and stuff but most of the times nine out of 10 times you'll only mess with replicates and replicate movement sometimes you may need your actor to be

08:21:18
always relevant let's say it's something important to your gamep play you'll have always relevant enabled so once that said uh let's also talk about priority basically the higher the value the more priority is given for this to be updated so let's say you have thousands of actors and your bandwidth is insufficient to actually update all the actors the ones with higher priorities will be updated first basically so now that we know the basics of [Music] replication let's start syncing up some

08:21:55
variables so if I head into my actor and if I go ahead and create a variable so we have some float already and what we'll do is on begin play we'll go ahead and set this to some random value so we'll get random So Random float and what we can also do is we can go ahead and print this string all right so let's look at what happens so let's actually delete some of our other methods here so I guess we had some stuff in our character so we'll just stop calling this function and we'll ignore this spawn

08:22:42
actor and I'm not sure if anything else is printing something so we'll ignore the left Mouse Button as well now if I press play as you can see we only get our post login and we have 809 and we have 43 now clearly this is not what you want you want them to be in sync so if you want variables to be in sync the first thing you would want to do is you would want to set this replication tab to replicate it now let's go ahead and try that actually so if I press play we still get different

08:23:21
values the reason is even though we set the value we need to set it on the server and we also need to wait for the replication cycle to take place basically your value doesn't immediately get replicated instead your value gets replicated in the next replication cycle so every once in a while so in our case if you head into class defaults you see this net update frequency parameter it's set to 100 let's say we set it to something like 10 now this variable will be updated after approximately .1 seconds obviously it

08:24:02
can be less than that but up to 0.1 seconds if I make it 100 it's going to be up to 0.01 second so it's not instantaneous remember that these two players what we play here they are not running on the same machine so you cannot expect the variable to update immediately so what we can do is we can actually set some logic to update this the principle which actually goes into this is the fact that all your replicated variables need to be set on the server so let's go ahead and do that now just a quick note here the event

08:24:40
begin play which is there since this actor is replicated each time one computer out of all the players will spawn the actor so for each computer this begin play will be called so if you didn't get what I mean if I actually simply go ahead and print a string so if I go ahead and type in print and if I print hello and if I press play you would notice that the server and the client print hello what that basically means is as soon as the client logged in that is when the client entered the game

08:25:14
this actor was spawned on the client and begin play was called both on the server as well as the client so what we can do is we can check if we are on the server so we can type in is server and we can do a simple if check if we are the server we can go ahead and set this value so we can go ahead and do that and if we are not the server we can go ahead and print it so one more thing we can do is okay this is going to work let's just do it so we can go ahead and print some float and go ahead and press

08:25:55
play as you can can see the values are the same in case you guys have any doubts regarding that you can go ahead and plug this in directly like this if I press play you see 718 718 the value is the same so basically all your replicated variables need to be set on the server that's the first thing now what if you wanted a client to set the value so your client cannot actually set the value however oh and just just another thing this logic is going to work for three players as well so if I go ahead and do this for

08:26:31
three players so as you can see all three players have the same value initialized so that's going to work as well okay anyways getting back so let's say now instead of this we wanted a client to actually set the value for us for all the players so the way you do that is through a remote procedural call [Music] so replicating variables this is about it there's really nothing much to it so this is basically how we would replicate variables I will get to rep notify so let's say you wanted to call a

08:27:11
function when uh a variable has been replicated instead of replicated you can check this rep notify option so then what's going to happen is when the value of the variable is set this function will actually be called on all the clients so if I go ahead and play you see we get a Hello as well along with that so we can just type in rep notify so we get whatever string we put over there so basically that basically shows that our replication logic is working that's pretty much it we can have any other functionality for example

08:27:48
let's say you have rep notify on a health variable you can update the health bar so something simple like that now let's let's go ahead and run this logic from the client so let's say we set this on the client and we already saw that that does not really work that well so what you have to do is you have to use a concept known as remote procedural calls basically they're just custom events meant for multiplayer in Blueprint so type in custom event and we'll call this one set some

08:28:20
float suf float is the variable name so we just made a setup for it under this replicat stab set this to run on server now what this is going to do is this is going to ensure that this runs on the server so if you call this from an owning client now we will get to the problem with it and if we run it from an owning client we are going to be able to call this on the server so reliable basically means you want it to run in order so let's say you ran two rpcs so it's going to run in the same order if

08:29:01
it's reliable if it's not reliable the order may change since it's networked it's not instantaneous so stuff like that can happen so now I'll just make this reliable I'll just go ahead and print a string and I'll call this one server RPC so now what we can do is we can go ahead and we'll not do this set with notify we can go ahead and instead of that we can call our set some float and let's see if we get anything printed now something weird happens as you can

08:29:42
see we are not able to actually call this RPC if I were to actually play this and if I open up the output log here as you see it says warning unit driver process remote function no owning connection for actor BPA C1 this is basically the display name of the actor function sum float set sum float will not be processed what has basically happened here is that unreal basically does not know which client actually owns this actor now this actor isn't owned by anyone and if you are to notice this RPC

08:30:25
call it says rely will replicate to server if owning client now this if owning Cent client section which is there that is what is causing our server RPC to fail now let's do a similar drill but inside a character so if I were to just uh create an RPC here so I'll just go ahead and create a custom event oops custom event and I'll just call this one svore test something like that and make this one a Ser RPC reliable go ahead and we'll just print out a string and we can say RPC called RPC called from character

08:31:06
now we want to be able to call this from the client instead of begin play since we are in the character anyway so we can use a more elegant solution maybe on a key press so maybe K on the keyboard cuz we don't have any other things so okay on the keyboard so find it over there so there is K so when we press it this will obviously run on the client which presses the key we can call SV test so go ahead and play this and if I go ahead and press K it works on the server and if I were to press K on the

08:31:45
client it works on the server too I mean obviously it's a server RPC so the function will run on the server but the point is our RPC worked and our client was able to make the server RPC now what if we wanted to be able to call this so from a client so for this you'll basically need to have an owner for this the way you do it is through the spawn actor function so if you have just placed it in the level like that you will have to use the set owner method which again I mean if you were to place

08:32:18
something in the level it's pretty obvious you wouldn't have an owner for it but let's just uh see an example where we use the owner so what we can do is okay we already have a spawn actor function and for the owner here this is something which I did a bit later so for the owner here go ahead and plug in self so spawn an actor doesn't matter the location and stuff doesn't matter we aren't worried about the actual actor itself we are worried about the RPC so make owner self and now what I want to

08:32:50
guys to do is run this only on the client so let's say for examp example we'll again do it on key press so then that's going to be easy for us to manage so we can manually call it so on key press what we can do uh and we want to spawn this on the server obviously we don't want to spawn this on the client because it is replicated remember so you have to spawn it on the server itself even spawning cannot be on the client so make sure you spawn it on the server so is server only if it is the

08:33:24
server we are going to spawn it and obviously this will run multiple times because for each player which will be spawned this will run so there's no way for us to actually ensure that it happens only once but nothing to worry so we can just grab a reference to this and we'll need to make this replicated if we want access to it from the client so we'll go ahead and promote this to a variable and we'll call this one obj for example and make this replicated so that we can access it from the client and now when

08:34:01
we press the K key we can just check if it is valid I mean it will be but just for a safety check if it is valid we can go ahead and call our RPC I don't know what we called it so we called it set some float so we called it set some float go ahead and run this now if I were to press play and if I press K on the keyboard as you see we get server RPC printed so if I were to check this we have server RPC over here and let's just test it on the client as well so go ahead and press K as you can see Server

08:34:39
RPC is getting printed so we are able to call it on the client basically the ownership is important generally it's a good thing actually that you wouldn't really require to call any rpcs from actors like this generally you would have rpcs in your character game mode game State stuff like that not in the game mode game mode everything is going to run on the server but for the most commonly used classes networking is already set up for you and in case you wanted to use it for an actor like this

08:35:11
I've shown you guys how to do it so this is how you do it make sure you just set the owner so let's say I don't actually set the owner and if I go ahead and press play this will still work actually so if I press K this is going to work but if I do it on the client it's not going to work so that's one thing to note from the client the reason this won't work is because now that we do this so let me just set the owner when I set the owner over here now when I press play I have two characters

08:35:43
so one is on the server and the other one is on the client and for both of these characters the begin play is going to run so this is going to run both for the server as well as the client so for the first version everything is going to run fine but when this begin play occurs on the client's version of the character even this character will have a begin play on both the server and the client because since this is networked this character will be spawned both on the server and the client so when the RPC

08:36:18
takes when the begin play is called on the server for this one that is when the owner property starts mattering to us or here if we don't set self in in in which case it it will refer to this particular character in the game our logic is not going to work so that was pretty elaborate in my opinion this is probably something which you wouldn't even require that much but this is basically how you do RPC calls now there's one more type of RPC which I want to hint upon and that is multicast

08:36:53
what if now we are now that you're on the server what if you wanted to print this for all the players in which case it's really simple type in custom event and we'll just call this one mcore print I mean we actually didn't set the float here which is kind of ironic but we'll just do svore print so SV print so we'll print this and we'll just duplicate this over here and make this a multicast RPC now I generally don't prefer make making these reliable generally you would use multicast for

08:37:29
things such as particle effects so you wouldn't really need reliable but anyways I'll just do it for this example and we'll call this one multicast so we'll just call MC print and remember multicast rpcs have to be called on the server if they're not called on the server it will only run on that client so it's not going to run on all the others so if I were to press play as you can see we get multicast RPC so this is basically how we would go about doing this now this worked on the

08:38:07
servers instance uh obviously because we spawned it over here otherwise it wouldn't work so if I were to just go ahead and press play you would see it works and if we had more players it's going to work again if I had three players it's going going to print it multiple times so it's going to print it on the server client one and client 2 so we have server RPC multicast RPC and stuff works like that so this is basically how you would go about calling rpcs so you have S print which is routed

08:38:47
to the server and we can actually test that out rather than doing it on begin play that is kind of an incorrect way obviously I showed you guys the right way to do it so this is some sort of logic which you would never use so we'll just ignore all of this go ahead and Press Play If I press K on the keyboard you see we are calling the RPC if I press K on the client it works as well if I press K on the other client it works as well and all of the players can see the printed string now you can also have the logic

08:39:21
the other way around so let's say you are the server and then let's say for example I'm just taking an example here let's say when the game starts you want it to show a countdown and the widget obviously will be spawned on the individual clients because obviously it's a widget so it has to be spawned on the particular client's computer so for that you'll again use a client RPC so I'll just do it over here so let's say when I press the K key we uh we'll test

08:39:50
this on the server itself client rpcs can only be run from that owning client or the server if you run a client RPC from another client it's not really going to work so in order to do that we'll just create an RPC so we'll make this one Clore test and make this run on owning client and what I can do now is I can go ahead and print a string and let let this just be there so if I do Clore test and if I were to press play if I actually press K here RPC called from character runs on the server over here

08:40:31
as well this runs on the client and over here as well this runs on the client so this is basically how you do it it'll just run on the client but what if you wanted to run this from the server so if you do this through a server RPC it is going to be routed through the server so I'll just do that and show you guys so what we'll just do is we'll just uh DIY it ourselves so we can say SV test and this will run on the server we can have another print string and we'll call This One SV for server and over

08:41:07
here instead of that we'll call the server RPC and now what we can do is once this is printed we can go ahead and call the client RPC so CL test now if you were to notice if I go ahead and Press Play If I press K as you can see now both are called on the the server so the server RPC worked and the client RPC worked but if I do this on a client as you can see the server printed SV and the server again called a function on this client so this is basically how you would go about using client rpcs so for any multiplier logic

08:41:44
this is exactly how you would go about doing this in C++ this logic is pretty straightforward there just a few additional steps for rep notif and uh replicating variables but other than that even the C++ part is pretty straightforward so generally you would use blueprint itself for core multiplayer logic unless it's something uh you know fundamental to your game and you want it to work properly like let's say you had like a firing mechanic or something and you don't want any sort of performance

08:42:22
issues or any overheads you then you would use C++ otherwise you would really just use blueprint for most of the things because it makes things so simple as you can see you don't have to do stuff like opening ports and stuff so all of that is handled by unreal and now let's go ahead and see how to run rpcs in [Music] C++ now I've gone ahead and opened up visual studio now we'll just ignore the plugins part right now and we'll head into our source folder beginner course public and we'll head into first of all

08:43:05
we'll head into a character now what I want you guys to do here is first of all before you actually use any networking feature just make sure you include net SL unreal network. make sure you include this header if you do not not include this header you'll get all sorts of weird errors so make sure you do that now first things first let's talk about variable replication so if you want a variable to be replicated uh you basically have to make it a U property first things first and this one we'll give the

08:43:46
specifier blueprint read right as usual to make things simple for us and one more thing which you have to give is you have to give the specifier replicated and we'll make this let's say a float float replicated CPP variable maybe now one more thing which you have to do this is additional this is not something you have to do in Blueprint but one thing you have to do for the replication logic to work is you have to actually write one function in the CPP file of our character we'll go ahead and

08:44:22
do that and then we should be able to make this work directly so I've gone ahead and opened up the documentation so this is the function which we actually need so we can go ahead and copy this and paste it inside our character. CPP file so I've opened that up and I've just made written a comment called replicating variables go ahead and paste it and we can go ahead and have a definition for it so over here this is going to be acore character just put your CL last name followed by the scope resolution

08:44:58
operator then can go ahead and just move everything to one line to keep things clean and over here you would want to run this macro called do rep Lifetime and this takes in two parameters one is the class which is going to be our current class and the variable name the variable name is going to be this oh it's going to be replicated CPP variable now I'm recording this a bitat later but one thing that I forgot to mention is make sure you call uh super of this function otherwise you'll get

08:45:32
weird classes when you use the D weird uh artifacts when you use the derived classes and for the parameter you can just pass this in so make sure you just do that otherwise your movement variables and stuff will not be replicated if you use your BP character so that's one thing to note and now if I were to go ahead and run a debugger we should be able to do it just make make sure you close the editor and then run a debugger so as you can see the build succeeded and now we should be in theory

08:46:04
able to use this variable as a normal replicated variable in Blueprint so I'll just show you guys replicated variables are shown with those two balls on the top so BP character is inherited from CPP character so we should have it so if I just type in CPP get replicated CPP variable and as you can see this variable is replicated if I were to actually go ahead and check this variable over here it says cpf net this basically means it's replicated so now this should work like a normal replicated variable now I'll show you

08:46:42
guys how to handle rpcs as well so rpcs are simple I'll show you guys how to handle server and multicast rpcs I won't really go over client rpcs they work pretty much the same so I'll go ahead and stop this now and for the for rpcs in C++ you need to basically have a u function first of all so create a u function and you cannot make rpcs in C++ blueprint callable however you can wrap them inside another function and then make them blueprint callable or whatever so what I'm going to do is I'm going to

08:47:27
make call uh put the specifier server and one more thing I'm going to make this either reliable or unreliable so this is where you specify it so reliable or you can make it unreliable now I can go ahead and actually write something here so let's say void test server RPC core CPP just to indicate that this is in C++ now what you need to do is you need to Define it over there but also uh rather than defining this you're supposed to Define uh another function known as the implementation for

08:48:15
this so what we are going to do is we are going to just copy this over into the next line This need not be a u function and type in underscore implement okay just ignore the parenthesis there implementation and now what we can do is we can create a definition for this instead so I've already done that so I have the definition for this and we can do something simple such as a print string so UK ISM system Library print string uh and we can go ahead and print in this is a server RPC from C++ now this should in theory work and

08:48:57
if we want to call this RPC what we would do is you can you can just go ahead and call this we don't have to call the implementation we have to call this in order for the implementation to get called on the server or we could just uh do something else such as wrapping it in another function so I'll show you guys both the approaches actually so I'll just do it on begin play so on begin play what we'll do is we'll go ahead and we'll actually delete some of this code so we'll delete this and what we

08:49:31
can do is over here we can go ahead and check so if we are on the server in fact or if we are not on the server we are going to do it so if is server so I guess it's called G is server I think it's a variable not a method so if this is not a server we are going to call this RPC over here we'll call test server RPC CPP and this will work as expected and we can go ahead and wrap this in a a blueprint U function so we'll create a u function make this one blueprint callable and from here what we can do is

08:50:21
we can just type in void wrapper for CPP RPC and this one we can just write it like any other function and the RPC will run now what you can do over here is you can go ahead and run this function inside of that so we'll go ahead and call This And since this is blueprint callable we can go ahead and just call this from blueprint also realize that just because of the way the function call works this is not going to run at all no matter what you do it is going [Music] to come outside the if so if it comes

08:51:05
inside the if it's again not going to the condition is again not going to be valid so you're not going to run this function so anyways we'll just run it as is and then we can go ahead and run a debugger so now if I were to actually go ahead and wait for it so once it loads in and I go ahead and Press Play If I press play right now you would notice that you get this is a server RPC from C++ so we got two server RPC calls one from the client and one from the server now I'll also set up some logic

08:51:49
so that we run this during game play so under your BP character what we can do is we can run the rapper so type in rapper for CPP RPC now if I go ahead and press play and press K on the keyboard as you can see it runs on the server and if I do it on the client that works as well totally as expected now one extra feature which I want to cover in C++ rpcs is the validation so if I just type in a comma and type in withd okay I have my caps lock on withd validation now what I can do is I can write a function which returns a Boolean

08:52:32
and instead of underscore implementation if I type in underscore validate you can make it so that this function will only run under a certain condition this is especially useful for something like cheat detection so if I were to just create a definition for it and what I can do is if this returns false basically this client which is calling the RPC will get disconnected immediately so I can just do return true for now and this RPC is going to run so if you had something like a health variable or something and you do

08:53:04
something like if health is you know less than or equal to 100 and or maybe if you had any other condition so let's say the health you had a set Health function which is an RPC of course so then you would check if it is less than or equal to 100 because you don't want the player to set the health to value greater than 100 stuff like this but for now we'll just leave this to true this function will run just to Showcase I'm just going to print string once again so this and we'll call

08:53:37
this validate and we'll not do this on begin play so oops print string go ahead and run a debugger and before we do that I'll actually just show you guys how to handle rpcs as well I mean uh rep notify as well so let's say I wanted to make this uh rep notify I would use the replicated using flag uh we'll do it after this actually now if I were to go ahead and press play as you would see the validate function was also called on the server so the server is going to validate and accordingly it is going to disconnect

08:54:18
the client if the condition is not met so that function whatever we saw right there that has to return true in order for the RPC call to take place successfully and for the client to continue stay connected so this is basically validation and now let's talk about rep notify I'm back inside the header file and for rep notify over here you can just go ahead and create a function so what do we call this function this need not be a u function but you can make it as well so we'll call this one uh Onre

08:54:52
it's just a convention to use Onre but but it need not be on rep uh rapper for CPP let's say for CPP and this one will just be void no need to return anything you could return a value if you wish but there's really nothing much you can do with it go ahead and write a function definition for it now again what we can do is we can go ahead and just print something so we'll just copy this over and rather than validate we just print rep notify from C++ so now what we can do is now we can

08:55:32
feel free to come in here and rather than typing in replicated type replicated using equals and just pass in the function name so you don't have to pass in anything else and this is going to work as you would expect one thing that you would want to do is wherever you call this function uh that will obviously be on the server make sure you call this function as well separately so where you set the variable so we are setting this replicated CPP variable so we'll do that make sure you call this as well so if

08:56:10
you're setting this in Blueprint make sure you make this function a u function and make it blueprint callable so we'll do that actually there's one issue with it in C++ this is how we would uh the same this thing works in the same way as it works in Blueprint so we'll just do it on our RPC itself anyways we're running the RPC so in the implementation for it we'll not have the print string rather we will have our rep notify the way you do that is we'll modify the value of the variable if you

08:56:46
modify the value automatically rep notify will be called Equals uh I'll just type Rand mod Mod 19 I just chose a random number over there and what you want to do is you would want to call this function only over here and the rest will be handled for you now we can go ahead and run a debugger and you would see that uh rep notify will be called and rep notify from C++ is going to be printed it just works just like that so wait for the editor to load in and once we are inside the editor if I go ahead and press play as you can see

08:57:30
rep notify from C++ and it was called on the client as well since there are two versions of the character here so one on the client and one on the server both of them called it two times so that's the reason we got four prints and the same thing is going to work when we use the wrapper so if I just type in k for example you see the rep notify works so we get the validate rep notify as well as anything else that you would expect so rep notify on the server and the client and if you want to do the same in

08:58:04
Blueprint so you can go ahead and set our replicated CPP variable to something and you would notice something weird uh first of all I have to do it on the server so we'll do it on a server RPC so SV test rather than doing CL test we'll go ahead and set the value of the this variable and we can do SV test go ahead and close this and if I were to press K let's just wait for it as you see this rep notify is only called on the client this is not actually called on the server so in order for rep notify to

08:58:47
work again once you do this you will have to type in on rep rapper for CPP so make sure you actually type that so now if I were to go ahead and press K on the keyboard you see it runs both on the server and the client so this is just one extra step which you have to take in C++ that is if you have your replicated variable in C++ so that's about it for rep notify I guess we have covered almost all aspects of replication uh multicast is something which I'll just talk about so all the same parameters except over here you

08:59:25
would have net multicast so don't mind the spelling I mean the capitalization so I have my caps lock on net multicast and this will work as expected you can again have your reliable and validation and stuff like that uh the rest of it will remain exactly the same so you'll have your implementation and you can have your validate if required but you wouldn't really have a validate for a multicast RPC so I'll just go ahead and delete that and this should work just as expected so I'm not going to really show

09:00:04
that this is how you would basically set up a multicast RPC and the documentation is there we did the example for the server there are no syntactical changes to this so it should be totally okay so we'll just delete that definition and I guess then we are done with multiplayer guys [Music] now that we are done with covering all aspects of game development in Unreal Engine let's go ahead and actually take a look at how to install Unreal Engine from source so the main part is actually done now we'll be doing a couple of

09:00:43
things such as downloading the source looking at how we can build it as well as we'll be going ahead and changing the engine version on our existing project so first of all as I mentioned at the very start of the course make sure you guys do get access to this repository here as of this date the release Branch should have 5.1.0 and you should be able to download the zip file over here so download the zip first of all uh especially when you're installing unreal Source just to avoid you know the permission issues

09:01:20
which you're going to get make sure you head into your C drive new folder and just create a folder called unreal Source or something uh it need not be the C drive just uh make sure you do it in your SSD if you have one so in my case it's the C drive so that's the reason I'm doing it so I'll just go ahead and install it there so go ahead and extract the files or here under C I'll go ahead and browse the directory over there so see unreal Source go ahead extract and extract it under that

09:01:57
directory and hit okay now we're just a few steps away in order to install Unreal Engine so first of all go ahead and run your setup batch file and try to run it as an administrator just to ensure it has all the permissions for everything so run the setup batch file as an admin so something like this should show up and once it's completed we'll head into into the next step after the setup batch file has completed running you can go ahead and run the generate with project files dobat so this file is basically going to

09:02:35
generate your Visual Studio solution so let's go ahead and run that again try to run it as an administrator should work regardless but if you do get any errors just run it as an admin so you should see something like this and this should complete relatively quickly at this point you should be able to see your solution file so go ahead and open it up once the solution is open and you see ready over here at the bottom left hand side what you should do is you should go ahead and head into engine and if it does ask you to install

09:03:08
a few more components in Visual Studio make sure you just go ahead and do that just follow along but in my case I've already done that so I'm going to go ahead right click on uifi and click build now once your build has succeeded under your engine binaries win64 you should find unreal editor. exe so by default the build configuration is set to development editor if you don't see this it means your build configuration was probably something else and it didn't get built so anyways let's go

09:03:39
ahead and open it up and our editor should load up if we do get any errors we can go ahead and debug it now so everything seems to be working fine and it is going to compile some shaders once that's done I'll be right back [Music] all right so now what I want you guys to do is go ahead and copy your beginner course project and now I'll show you guys how to change the engine version so head your beginner course U project file right click switch Unreal Engine version and now you should see Source build at

09:04:15
whatever so basically I opened and closed the editor that's it so whatever we did there open unreal editor. exe I just closed it immediately and now I'm back to this location and you should see this so if I hit okay it is going to generate some Visual Studio project files and unless something's horribly wrong it should in theory work out of the box so that's about it and now you can go ahead and just Build Your solution once again cuz there may be a few API changes which you might have to

09:04:47
make so those will be lifted in listed in the output log and as well as in the release notes and the documentation or whatnot so head into your solution now we have switched the Unreal Engine version so now we can go ahead and right click on our beginner course and click on build so we get our first error here and this is actually fairly common so basically we have switched the Unreal Engine version and we have a plugin over here which is based on the older version of the engine there are two ways to fix

09:05:24
it one you can head into the marketplace and reinstall the plug-in which is meant for 5.1 or I'll just show you guys the way to do it without up using the marketplace so in the marketplace it's really easy you can just go ahead and update the plugin but over here if you really want to just use the same one what you can do is you can head into your engine installation directory so in my case it is C unreal Source Unreal Engine release engine plugins Marketplace uh it's not here because we

09:05:58
haven't yet installed so you'll find it there so we'll go to our previous installation program files andreal engine this is where I had it U 5.0 engine plugins and you should find Marketplace and the one we are interested in is low entry extended standard Library you don't need to copy it to the engine installation although you could uh what I'll do is I'll just take it to the plugins folder over here so over here and under inside the U plugin file we'll do the same modifications over here what we going to

09:06:37
do is under the engine version we are going to type in 5.1.0 and now if we go ahead and try to build this once again we shouldn't get that error hopefully so it will take a a while and if we do get any errors we'll go ahead and change it or fix those so we have a few errors here and these are mostly the changes which came according to the documentation due to the platform SDK upgrades but it's not really a problem so because I don't think any of you guys unless you guys work for a trip Tri s Studio or

09:07:24
something I don't think you'll be using this and this is from the plugin this is not something in the engine so nothing to worry so what we can do is we can simply just delete this code and just do return false and even for the Xbox one so we can just do the same thing and I'll tell you guys which file this is it's basically this file right here so in the error list you see platform PS4 whatever so just head into that just double click on that and you will reach there and over here as well

09:07:57
so line 264 so I feel like this was it so before changing it was in line 264 so now it's gone a bit up anyways let's try building this once again and as you can see the build has indeed succeeded but once the plug-in actually comes for 5.1 what you can basically do is install 5.1 here like in the epic games launcher install the plugin from the marketplace and then you can go ahead and copy that into the plugins folder in the engine level so what you would do is you would have it over here so C unreal Source

09:08:40
release uh and engine plugins over here you would create a new folder called market place or something and then you would like just copy it in anyways we not really worried about that right now now what we can do is now that it's built successfully we can go ahead and run a debugger and we should be able to run this in 5.1 so I did show you guys multiple things so the errors which you get will actually depend on what plugins you're using and how's your code base and what changes are made to the

09:09:16
engine's API itself so depending on that you'll have to look at the output log and the error list and do something and there are a few deprecation warnings as well so if you just have a look so I'm not really sure what this is but this will probably be changed soon once the plugin is updated but right now I'm not really worried since it's just a warning so now I can go ahead and run a debugger all right so our project has open successfully and it is prompting us to change a few project settings in

09:09:52
order to actually use Virtual Shadow maps and nanite so that's not really an issue we can head into the project settings and over here under it should in theory be here so platforms so let's just search for platforms it'll be under any one of these so platforms windows and you can go ahead and enable share model 6 and over here we can go ahead and I don't think we'll require Shader Model 5 so that should be about it and now you can go ahead and restart the editor all right so now I've restarted

09:10:42
the editor and now we are using Unreal 5.1 so that's about it for installing the source and changing your engine version now there are a few more ways you can handle some of the things such as the plug-in part but on the whole this is how you do it and if you do want any more specific references you always have the documentation which you can refer and the release notes and maybe the unreal slack as Discord server so that's about [Music] it all right so we're finally inside the last section of this course and

09:11:21
obviously it is about how to package your game so it used to be very simple before so you just go file package project but now you probably have to just do it through the project launcher which I will show you guys it's really simple so head into tools project launcher and you can use this but I'm going to be using a custom launch profile so go ahead and add create a custom profile and I'll just walk you guys through each option you can give a name to this Prof profile let's say this

09:11:54
is for testing let's say uh you are building this for testing so you can name this profile testing you can reuse this profile for the next time when you package the game as well packaging basically means you make your game or you turn your game into an executable basically uh now project is going to be beginner course of course and build configuration so debug and development will be used when you're actually you know testing out your game and you're still not yet at a stage where you

09:12:28
can uh send it to other people so your print strings and stuff are going to work but under shipping uh none of your print strings and stuff will work but it will take a bit longer to build and testing is somewhere in between debug development and shipping so it's below shipping but it's above development and debug basically so you can select any one of these I I'll just select shipping and here these are settings we don't need to worry about and about cooking the content you can do either on

09:13:06
the fly or by the book uh basically what on the Fly and by the book is going to differ in is basically if you do buy the book everything is going to be cooked uh beforehand basically so if you if you're packaging your game for shipping most of the times you will have buy the book and you would select Windows if you're developing a Windows game obviously if you have anything else let's say you're making an Android game you would select Android and stuff like that and under cook cultures you'll find

09:13:44
English somewhere here so it should be selected by default so I and you can select your Maps which you want to cook so we using all so we'll just select all but you can choose to cook only selected Maps but note that if you don't cook a certain map you won't be able to open it in game you're going to get errors your game will probably crash so that's one thing to note now release DLC patching settings these are some things which I'll not go over and under advance settings as well so you

09:14:20
can go ahead and mess with these so so you can enable this if you want all the content to go in a single dot pack file stuff like that and everything is pretty self-explanatory next package package and store locally then you can go ahead and give it a path so generally I'd like to do it in the project location saved and I'd like to create a folder called staged builds staged builds if you have used the project launcher in the in the older versions you probably already know what this is and is this dist is this build

09:15:03
for distribution to the public we have selected shipping so I would assume it is of course it's again your preference dois to Archive can select yes or no doesn't really matter and deploy we can select do not deploy because we aren't actually launching the game so if we select do not deploy basically you can launch it through the executable itself so once that's done you can head back and you can click on launch this profile so now once everything has been completed you can head into the

09:15:41
directory over there you should find a Windows folder and you should find your executable right there so open it up and you should launch your game so we will end up in this map right here again you can change your project settings and you can change the default map but anyways our purpose here was to check if the game packages and everything seems to be working the physics simulation works and so on so that's pretty much [Music] it okay guys so this is going to be the last last segment of the course as you

09:16:24
guys would know and I hope you guys would have enjoyed the course till now and congratulations if you have completed the course till here and the further part is going to be 2 hours of me creating an entire game so hopefully you guys will enjoy it uh see you in the engine all right guys so this is the last section of the course and this is not actually going to be about you know learning anything new how however in this part I will be live demonstrating without any Cuts how to make an endless Runner such as Temple Run or Subway

09:17:02
Surface or any other which you might have played so we'll be taking the most simple approach or at least as far as my knowledge is concerned if you do have anything simpler you can let me know in the comments and hopefully within an hour we'll be able to make the whole game with the menu animations and and all that kind of good stuff so let's get started so let me actually have a stopwatch here so that we have track of our time so I'll just create a game it's going to be third person because we'll

09:17:37
have the animation blueprint and stuff but anyways I don't think we'll be using that not to worry uh we'll go with blank actually C++ and we'll call this one endless Runner create it now this will take a little bit of time and I do have a couple of things being installed in the background and I also have a list of plugins that I'll be using so you guys will have a pretty good idea of what we'll actually do with plugins and stuff because in the course I think I just went over these briefly

09:18:17
but I went in depth about how to actually create your own plugins and stuff anyways so our project will be created soon and this will compile so until then we can go ahead and open up our epic games launcher head into library and we can close this editor for now until we add everything so what I what I'll do is I'll go ahead and search these one by one so City subway tunnel so I have to create a separate project for this not going to go over that right now so we'll go construction volume so volume 1 and volume two we'll

09:18:57
go ahead and add this to endless Runner we'll add this to endless Runner I'll I'll clear the cach later it's just taking up storage and we want Le extended so Le extended so we have already installed it to 5.0.3 so nothing to worry about there so Adventure character whoops so this will be the character which we'll be using and it's going to be hella fun uh we don't have time to actually model our own character that's the reason we are doing this so I'll just go

09:19:30
over this real quick so F variety pack not sure if we will get the effect we need but I'll just add it just in case okay I need to download it yet so not going to do that now so window dialogue box so I've already installed it so these two so we'll use this for obstacles and stuff and lastly we'll just have some trees maybe at the side we could have something Stone Pine Forest and go ahead and add it once everything is complete now depending on your system if you have a hard drive or something this

09:20:18
process is going to be a little bit slow so this is under my unreal projects endless Runner so we'll be using the file explorer for this and I'll just delete this later on so now once the engine is loaded up we can start making our game and we'll go ahead and create a Maps folder first so right click Maps we'll have only one and all the obstacles will be spawned at runtime dynamically when you're playing the game so we don't really care about having multiple Maps but we'll have two

09:20:51
so one is going to be our main menu and the other one is going to be the actual map so I'll go ahead and create the map and I'll call this one game map all right save that and go ahead and open the main menu head into project settings and just change that as well so under your maps and modes you should have open world we'll change that to main menu so edit a startup map will be main menu and it's going to be main menu again so editor we can start with our game map actually but the game has to start from

09:21:28
main menu so just go ahead and click import doesn't really matter all right now over here we can start making a main menu so right click create a new folder and we'll call this one content once again and inside this will actually create stuff because the main content folder is a bit clogged up so we'll call this one UI and we can create a main menu right click user interface widget blueprint create a user widget and we'll call this one main menu or bpor main menu and we'll suffix that with a WB to

09:22:11
indicate it's a widget and it's going to be just quick and dirty so we'll add a canvas panel here and at the center we'll just have a start button and an exit button so we'll add in a vertical box so vertical box and over here we can go ahead and make this Center align first of all Center align position zero with 0. five for the alignment value so this is going to make sure everything is centered we can go ahead and increase the size a bit even vertically and we can go ahead and add

09:22:48
in two buttons so button one and contr D to duplicate we'll make it so that it fills it and we obviously want the play button to be bigger we don't want our users to exit the game anyways we'll add in the the text here so add in some text add in some text and change the background color for both of these buttons make it almost black maybe not exactly black but almost so I like this shade of color now rename this to play or rather start we can try change the font maybe so the font we'll use is going to be the light one

09:23:32
so 40 seems about right make this one 40 as well and this one is going to be light and this one is going to be exit so we can add the functionality as well because this is pretty simple so on this button we'll rename this to exit button or it's really not required I guess so on click and for this one as well we are going to add an on click this is the start button so I'll just comment this out and for this we can go ahead and execute console command and we can type in exit now our exit button should work

09:24:09
we can go ahead and test that first of all we haven't even created the widget so under content we'll go ahead and create a new folder and call this one Blueprints and we'll have two sub folders here we'll call one as game and the another one as main menu because we'll have different player controllers and stuff for the main menu and the actual game so under main menu right click go ahead and head into blueprint class and create a player controller and we'll call this one

09:24:40
BP main menu player controller so this is basically for you know creating the widgets and stuff we'll just use the player controller now under the event craft we can just do it on beginning in play so we'll create a custom event custom event create main menu and create a widget it's going to be BP main menu widget blueprint and add this to the viewport now we I don't think we really need the reference but we'll just store a reference to it anyways so main menu widget blueprint we'll just have a

09:25:19
reference to it and from this we can go ahead and add it to the viewport all right and on begin play we can create the widget so create widget or rather create main menu is the function name so create main menu and now if I compile save it go ahead and press play as you can see nothing happens because we haven't changed the game mode yet so over here we'll create a new game mode so go ahead all classes game mode so we'll create a game mode base so we'll call this one bpor main menu game

09:25:58
mode now under your world settings go ahead and change your game mode to BP Main menu game mode and over here the player controller can be our BP main menu player controller and now if I go ahead and press play we should get our buttons start won't do anything but exit is going to work now let's actually head into our game map here so Maps game map we'll worry about the main menu a bit later later so we are in the game map we can go ahead and add our sky so Sky atmosphere Skylight and we can add in

09:26:30
our directional light we can also have a fog so we can have exponential height fog and we have everything set up now we could change the time of day as well we'll make this one Dynamic for now so fully Dynamic light cuz I don't have any time to actually build this so go ahead and rotate it to make it like a morning or evening scene this should be about good not going to spend too much time on it save it up and over here under content now we can start building the actual level so I'll just go to my

09:27:08
blueprint folder here under game I'm going to create the game mode and stuff for this one as well so type in game mode so I'll create game mode BP game mode this one is just going to be called BP game mode because this is for the actual game itself under your world settings go ahead and change that once again so bpor game mode we'll have a CPP game mode if we really require but I'll try to stick with blueprint as much now let's check our time so 10 minutes in now under your game mode we'll also

09:27:44
have a game state to count a score and stuff so game state so game State base BP and underscore game state so we have our game mode oops and we have our game State and now we can also have our character and stuff so we can create that first of all we can just uh right click blueprint class character and we can type in BP character open it up and we have some basic things already set up for this mesh we'll be using one of these which you bought under man under mesh full we have all these various options so we

09:28:31
have four options so we'll be using these four so these four will be the options for the players to choose from That's How we'll do it so we'll create a derived class for this for BP character so under our characters what we can do is I can type in character I'll just move this here and go ahead and type in sub classes so these will this is like your main character so every character is going to be a BP character but then we'll specifically make them choose a mish so go ahead and create a blueprint

09:29:10
Class Type in character and over here we can make it of type BP character and call this one character one we can actually just name name them maybe we'll call one Adam duplicate that we'll call One John I'm just giving generic names we had four so we can call one Jason and maybe we can call one bill I just chose random names so open this up and for the mes we can go ahead and start replacing it so head to the location where we had the mesh so this is going to be our first character we'll set up the animation

09:29:50
blueprint a bit later so it's a bit off but not to worry we can go ahead and adjust that 90 and we can head into the other classes here so under content blueprint game character sub classes we can head into Bill and this was called SK manful 1 so we'll call this SK manful 2 over here we can select SK Man full 3 so SK Man full 3 and for this one we can have SK manful 4 so SK Man full 4 so that's pretty much all set so I'm not sure if I should just use the default one here so man full

09:30:50
one not sure if it will inherit the transform so I'll just try this I'll compile compile this so if I open the full blueprint editor okay it has inherited the transforms that's a good thing so we don't have to do everything once again all right so we have our character set up uh in our main menu we can go ahead and add a character selection option so head into content uh our actual content folder under the main menu we can have a button somewhere and maybe over here we can type in change

09:31:31
character so I'll change the color of this I'm not really worried about the visuals as of now so I'll just go ahead and change this okay I change the color so background color I'll just make this dark again and we can add in some text and we'll call this one change character all right make this a little bit wider so that it's visible for a player so make this one 45 maybe or 35 35 seems good we'll make that one light once again maybe we could make start a bit uh Bolder so let's start B regular cuz we

09:32:14
want our players to deliberately click Start All right so once you click on the change character menu it should just give us a list and we will create the widget for that now we'll also need a game instance class head into Blueprints and game instance is General so we'll create one here so game instance go ahead and call this one main GI or something and under the project settings we can go ahead and change it so game instance oops game instance change that to main GI and over here we can have a variable for

09:32:56
selected character and we can change that actually we can change that to be of type BP character class so we have BP character we should see it somewhere here BP character class reference so this is going to be the the character which we have actually selected or we could have it in a struct we'll think about that a bit later now once we have that we can go ahead and start making the actual obstacles and stuff so one thing to note is that we want to make this modular in a way we want to be able to spawn them one after

09:33:35
the other let's just go ahead and do that so on when the game starts we want to have a bunch of obstacles and then we'll look at what to do uh we'll work on the obstacles after we work on the animations actually so we'll head into the skeletal mesh we have certain animations so content content blueprint we'll head into character and we'll create the animation blueprint right here so animation animation blueprint and we'll go ahead and select our ue4 mannequin skeleton this is the one which

09:34:14
comes with the pack actually so create and we'll call this one character an MBP open it up and inside this we have a bunch of things so we'll create a state machine doesn't really matter now we can go ahead and have an idol so we'll have idle and we can have we'll create a blend space for this so right click go ahead into animation so basically this is for transitioning between your idle and walk animations blend space and we'll call this one walk run okay oh here we'll have few things in

09:35:09
the horizontal and the vertical axis horizontal axis is going to be the direction and the vertical axis is going to be the speed so we'll go between 0 and 600 but we'll see see if we can do something else a bit later on now open this and we can have our third person walk halfway over here we can have our third person run full way and we can have our third person idle at zero so we transition between these something like this for the direction we'll have a negative 180 and positive 180 obviously so this will be like your

09:35:52
angle from your forward Direction that's basically what this is now we can change the animation blueprint after we actually set it up first so for the idle we have our idle animation playing and we should already have this working and we can have this as a new state so walk run we will set up the conditions not to worry oops go ahead and do that so on begin play begin play we can go ahead and get the pawn owner and cast to BP character and we can make this a pure cast because this will succeed or if it

09:36:37
doesn't we can go ahead and pull it and once we get access to our character what we can do is we can get access to the speed so get velocity so get velocity and we want the vector length right now we have a vector and we want the magnitude of this vector and we can promote that to variable and obviously the magnitude of the Velocity is nothing but speed so speed and we can also have Direction so get actor rotation we'll set it up a bit later actually okay so under the update animation what

09:37:26
we can do is uh we'll need this on every frame so we'll use a reference instead so promote this to variable and call this one character ref we'll be using this multiple times so we can drag this over there so this will be our speed and also what we can do is we can also get the direction so we can use this function known as calculate Direction and that is what we'll set the direction to be set Direction so we'll create a new variable called Direction it's going to be a float once

09:38:11
again and we're going to set the direction to be equal to whatever this is for the velocity we can just uh grab in our get velocity here and base rotation is going to be the actors rotation itself so get actor rotation and we can plug this into the velocity as well now what we are basically doing is we're calculating the direction so that we actually input the value correctly in our blend space basically we are not using this value anywhere else or here we can plug in our Direction and speed so direction and

09:38:54
speed so these were our vertical and horizontal axis values in our blend space we can also have jump which we will do we have we don't have a state transition so if speed is greater than let's say 10 we can go ahead and transition and over here as well if the speed is less than 10 we can transition so rather speed so speed is less than or equal to 10 we can go ahead and transition into this state so now we shouldn't have any of those warnings all right now if I actually create something here so I'll just

09:39:36
create a player start so we'll know where to start so player start and I'll just go ahead and box out a simple level so shapes so I'll have a cube and I'll just make this really really big so this is just for testing purposes and for the default Pawn class I'm going to select BP character and let's set up the animation blueprint over here if we go ahead and select our character anim anbp in theory everything should work fine so our camera is a bit off that's nothing to worry

09:40:20
about so under our BP character we need to set up a camera so add a component and this will be of type camera go ahead and add it we can adjust the view that's nothing to worry about and if I go ahead and press play we have our camera here so we can make that a little bit further back maybe tilt it down a bit and I hope this looks good okay so so this looks good so we have assess none in our character animation blueprint so that's only in the first frame which is happening basically so we

09:41:05
can convert this to a validated get that's a simple fix can go ahead and turn that into validated g go ahead and press play and now we shouldn't get those errors can set up our movement logic real quick here so it the character is always going to be moving and I think we might have to change the animation blueprint here because we always want him to be running cuz we don't want him to stop so we'll always have running actually so sorry for that but anyways something we can do so he'll always be running

09:41:53
so this is how he'll always be and we can also have you know a copy of this so we'll just copy this over and we can type in run fast we can make this go at a higher speed so there should be a speed multiplier somewhere here so playback speed is what it's called I assume so playback speed so nothing under the details we look into that so there's actually an option called playback speed so we are going to increase the speed and make it so that it's actually as if he's running now what we can

09:42:42
do is we can head into the character once again and now that we have him running continuously we'll actually do it so that the obstacles in the world actually go backward can create the blueprint for that now so we're finally heading into the obstacles so we spent 25 minutes not done really really that much and again in the blueprints folder we can go ahead and create a new blueprint class we'll do it in a new folder so we'll call this one course rather this will be the obstacle course

09:43:24
basically and we'll create a new actor and we'll call this one obstacle underscore base and we can go ahead and create a child blueprint class and we'll call this one obstacle one obstacle 2 and so on so obstacle 2 duplicate that duplicate that duplicate that we have five we'll see if it if it gets to hectic we reduce this number over here we'll need some sort of a base so we can try using some of the things which we got from the content packs so under hanger I guess we had a

09:44:04
road I believe I type in road we have this which is pretty taable I believe oh here Road set we have this so we can use this just that we'll need to know what's the length of this and stuff I don't think we'll go for nanite or anything this is fine so close some of these which we are not using head back into the obstacle base over here we can go ahead and add in a static mesh and this will be common for everything so head back select that and go ahead and and put that in so this is there add the

09:44:58
origin but not to worry we'll find a way to fix that so it would have been nice if we had multiple Lanes but we have to live with this right now so I'll just go ahead and reenter this I'm not sure how big this is going to be so I think that is pretty well centered we can go ahead and add in an arrow component just for a reference so add in an arrow component attached to the root this one is going to be add the origin obviously we'll just rotate that for our reference or we'll keep the rotation to

09:45:45
zero we'll look into the rotation and stuff so we'll duplicate this once again so control D to duplicate and we'll just have one over there I think one is enough but we'll just have it just in case all right so this is exactly at the end now at first we can spawn for example 10 of these and then we can later see what to do we can have something in the side by the way we don't have anything so we'll just add in a plane in and for this we can increase the scale of this maybe we can make this 100

09:46:32
I guess okay that's a little too bit 50 maybe change it on the Y 50 is a bit too much 40 maybe 30 35 32 seems to be about right so it aligned perfectly ly here and it aligned almost perfectly here as well we can have 32 now this is approximate you can do it accurately when you actually do it so go ahead and duplicate this once again we'll attach it to the root duplicate this will be for the other side all right so we have something on both the sides now if we head into a derived classes we should also have all of

09:47:41
those so we can spawn this first of all just for testing it out so open the level blueprint and we can just do a for Loop so for Loop uh we can have a loop of length 10 let's say We'll select An Origin we'll start from a certain point so Target point we can start here maybe we'll make the Z value of this zero we'll make the X and Y Zer as well so this is going to be where we start and we can go ahead and start spawning this further on so we'll have access to this target point now so create a reference to

09:48:40
Target point so we are going to spawn actor from class and it's going to be BP obstacle or I'm not sure what we call called it obstacle base this is for testing so it's fine so we can get actor location it's going to be zero I'm aware but in case we wanted to change it the logic should still work that's why I'm using the target point so get actor location we'll break this down actually split the struct pin now the Y and the Z are going to remain zero so I have to see which is the

09:49:22
forward axis here actually so in the obstacle base we have y as the forward axis we can rotate everything by 90° if we don't mind can just rotate everything by 90 oops we change the location so we can change this to 90 and stuff doesn't seem to be working we'll we'll have y as the forward axis in our case don't mind so the x value is going to be zero we are going to split the struct pin so we're going to multiply this multiply this by the index and we can go ahead and split this

09:50:14
and the Y is going to be this x and the Z are going to remain zero let's go ahead and just test this out so go ahead selected viewport so if I click f8 and if I were to notice we don't have anything so we should have our Target okay we are taking the target points Y location but we need the last obstacles location so we need the value of this actually we need the location of this Arrow so this Arrow so this arrow is going to be located at 3,200 so we'll just copy the number we'll just brw foret

09:51:18
here so we have the target Point that's where we start and into 3200 so it's netive 3200 so I'm not sure if we really need this this is going to be zero anyways so this into 3200 index into 3200 now now let's try this okay so our obstacle course is spawned successfully so a bit of an issue with the direction over there but that's totally okay all right so we have that completed so we spawned our initial course so we can grab in our player start first of all and we can rotate that we can

09:52:28
delete one of them we can maybe rotate that 90° so now we should face the right direction now move this a little bit to the left so for reference we'll just have one obstacle so we'll just have obstacle base we'll set everything to Z 0 0 0 and we'll base the player start accordingly so our player start just disappeared somewhere okay it's up there so we'll click end to snap it to the ground go ahead and do that and now we should in theory be centered hopefully yep we we will be centered

09:53:25
now now if I go ahead and press play as you can see we are centered now we can also set up the logic to move sideways so we can linear interpolate actually so we'll add in Target points so copy this over we'll copy the X location of this so X is going to be 20 we need 20 here and the Y location really should be the same actually again so Y location should be the same now we have got these in the same spot now we can have few more so these two are equally spaced now we can set up some logic so that we

09:54:20
slide between these basically head back into the character to set that logic under your BP character if we press the right arrow we won't do changeable controls so right arrow so right and we can have left as well so keyboard events left under light right and left we can change them so if we press right we also need access to which Target point we are at right now we can have all of these in a blueprint we can have these in the game State content blueprints game game State we can type in uh we'll have an

09:55:12
enum it's going to be simple so content we'll create enums so enum right click create an enumeration and over here we'll call this one which side of the road you're in basically so I don't I don't even know what to call this e which side I guess I mean which is kind of stupid but at the same time it's descriptive so it's either going to be left okay you're at the center by default so I'll have Center first center left and right so if I save that and head back

09:55:55
into my game State now I should be able to create a variable of type which side which side e which side just my naming convention so we'll call this one with side maybe all right so we'll have access to this at any given instance and on begin play we can store a reference to this get game State we can go ahead and cost to our BP game State and we'll have a reference to that promote that to a variable and call this one game State ref okay now from here when we press right we can first of all get access to the

09:56:50
variables the first variable which we need is the only variable which we have right now basically which is the side so we'll type in side and we'll do a simple switch so if we are at the center right now we can go to the right if we are at the left right now we can go ahead and head to the left basically uh if we are at the left we can head into the center if we are at the right we don't need to do anything so basically on Center and left we can do that again we'll copy all this

09:57:38
logic depending on which side we don't want to do anything if we on the left side here in this case and we can linear interpolate on tick so linear interpolate is what we'll just do so we'll type in lurp and we should find a linear interplate and we should be able to feed in the alpha we'll think about a logic for that now we'll have access to where we are by default we are at the center just a a small break there now over here we can continue with our side switching logic so we'll actually get

09:58:29
hold of all the locations and stuff so by default we are over here so if I press play we are over here but when we want to move we want to move to either this or this so we'll actually have a few variables for this I'm going to be hardore in this but you can have a more elegant solution for all of these so I can go ahead and under my game State itself I can have right location right location center location and left location so I'll duplicate these so I'll call this one left location and I'll call this one Center

09:59:18
location and we'll manually set these values so this value over here is -230 -270 and 0 this is the left location so -230 -270 270 and zero we can actually save some data I Believe by using floats we only need the we we only need to linear interplate the X directions so we'll just store the X values of these so this is 270 20 and -230 not sure if they're spaced equally I'll just have a look at the top view I want them to be spaced equally so between this and this there is a difference of

10:00:24
250 between this and this there is a difference of 250 so yep they are spaced equally okay so the right location is going to be 270 left location is -230 and this is going to be 20 so I'll just store these like this now what I can do is I can go ahead and actually move the character so I'll try seta location not sure if this is going to work so if we are at the center we'll try this to try to set this to the right location so we are going left so left left location so we only want to change the

10:01:16
X so go ahead and split the struct pin change the left location and the rest is going to be the actor's location itself so get actor location go ahead and split this Y and Z will just remain as is all right so we can go ahead and try this so if I press the left Arrow so nothing is really happening here so we can see by printing if something is happening so nope we are not actually taking the input something has to do with the input so Arrow left keyboard not really sure I I'll try to use a and d for now so a on

10:02:09
the keyboard so we'll use WD so when I press a on the keyboard we can try that a is going to be instead of the left Arrow all right so we did we don't have access to the game State according to this that's that's mostly because we didn't set it so that's pretty simple to handle so we can change that to BP game State now over here we can try the left Arrow logic itself so if I type in left not sure what else we have so left is the only thing we have so we can go ahead and try this so

10:02:57
left Arrow doesn't seem to work okay left Arrow works so that was the game State issue not R thing so we can use this logic we can linear interpolate instead or we have have our interp nodes anyways we can have a variable for the Target location so this is where you know we want to get our character so Target X location just to be precise so linear interpolate is going to be a little tough so F inter two is what we'll use it's a pure function so F inter to f F inter to constant because we want

10:03:54
it to interpolate in a constant rate so Delta time is going to be Delta seconds inter speed we can adjust that so we can promote this to variable and we can call him sideways speed over here we can replace this with the target X location that's going to be the X oh this is an integer will make this float so Target X location and current is going to be our current X location so Target is our Target X current is our current X location so current X location so we can get the actors X location again all right so this should be it for

10:04:57
the sideways movement and over here we can go ahead and set these if we want to go left we don't want to do anything when we are on the left side all right we can get the game State and we want to go left so left location and we can duplicate that and if we are right we can get the center location okay but the logic isn't done yet I'll get back to it so we can use a select to just make things a little bit more simple so if we are add the center we'll go left if we are at the right we'll go

10:05:46
to the center so the logic should make a lot more sense now and we can set this over there move it in similarly we can copy over this Logic for our right so that it simplifies things a bit so if we are on the right we don't want to do anything we'll go to the center if we are on the left and we'll go to the right if we are on the center so get the right location so this is what we'll set it to all right now our logic should work once if I go ahead and press play so if I put put the left Arrow nothing really

10:06:47
seems to be happening let's just check out y oh okay our inter speed is zero okay so now if I try all right nothing really happens so let's try 100 so our ACTA location seems to be fine so current and Target is okay and now we can go ahead and print hello so we're not changing the location I assume that's what's happening so when I press the left key on the keyboard and when I press the right key so we are changing the target X and the target Y location so we'll try it without the inter

10:07:55
first a bit of debugging will so we can just copy this in so I'll just remove this logic from tick if I hit left or right nothing really is happening so we can print it and check what's going on all right once again the input isn't working we'll use a so we'll go ahead and use a on the keyboard maybe go ahead and use a so if I type in a the input okay it's just about the window being in Focus all right so if I go ahead and run this okay this works now we can try it with the interp

10:09:09
logic so now we don't need this okay the speed is just way too less so we can go a bit crazy on this 50 maybe nope still very slow 200 okay it's still really slow so 500 okay this is not going to help oops it's going 50 so if I make this 500 okay this is a lot better but maybe th000 would be fine all right so this seems about right but now we need to change our actual State itself so again we'll use this select node right there so if we are in the center we have to set our side so we'll

10:10:39
grab a reference to the game State and we'll set side depending on where we are so if we were at the center and we moved left we'll set our side to left so Center we'll set it to left if we were at the left it's going to be left itself if we are at the right we'll make this Center copy over the logic okay so for this so everything will remain the same except when we are on the left and and we go right it's going to be Center if we are on the right it's going to remain

10:11:23
right if we are at the center it's going to go right okay so now we can go ahead and try this out so something happened with our logic right there okay so we had to get the actors's location instead we made it zero so it just sunk under the ground so go ahead right left right left right okay so it is a bit glitchy it is a bit glitchy at times so let's try enabling teleport sometimes that should fix the issue okay when I'm add the right he's moving to the Center for some reason so

10:12:23
when I'm at the right and I click right again so the logic is when I'm at the right and I click right again I should still remain at the right when I'm at the left I move to the center so let's try that so I go to the right click right again I go to the Center for some reason so when I'm on the right the target shouldn't actually be this it should be the right location itself when I'm on the left this shouldn't be zero this should be the left location itself because you're doing the inter P

10:13:01
tick so that's why it's happening left right and Center all right so now our logic is working totally fine and we can stop printing hello it's just annoying at this point okay then I think we exceeded one okay we're pretty close but we are left with our last few steps now we have to make the obstacle move which is pretty simple now we can spawn it dynamically instead rather than spawning it or rather just using this I think we are spawning it yep we are so I can press f8 head into my

10:13:44
perspective View and now for the magic head to the obstacle blueprint itself course obstacle base we can try this on tick so on tick we want to set the actors's location so we want to change the location of this actor we'll get the current location so get location of this actor so get actor location and when we move forward we are increasing ining the y basically so when we move forward we are increasing the Y so the logic was wrong okay when we move forward we are going more towards the negative y

10:14:38
direction so what we can do is we can go ahead and move it backwards so we want to increase the Y so the x is going to remain constant the X will be as is delete that split the struct pin Z is going to remain constant but Y is going to be y plus let's just say 1 time Delta time Delta seconds let's try Delta seconds itself first this should remain constant for All actors because this is tied to frame rate so I think it's moving but it's moving very very slowly yep it is moving as you can see

10:15:30
but it's moving very very slowly so we can just go ahead and multiply this so multiply this by some value let's just say we multiply this by 100 so not sure if yep there we have it so as you can notice it's not actually the character that's moving it's the whole obstacle course which is moving and what's weird is our character is actually following it even though we haven't actually attached him over there okay so we can fix the uh X location of the character as well

10:16:19
because he he seems to be just sliding along so there is actually a setting somewhere here so it shouldn't slide along the surface so something or there character movement maybe and there is something over here okay ground friction let's try zero on that okay we we are just still moving back so if if I hit f8 actually the the whole thing is moving back so instead of that we'll just set the uh location the X location every time to be constant or rather the Y location I'm not sure what it was so

10:17:12
we'll copy it so Y is -270 so -270 I don't want that to change and as you can see our logic is working and it seems like we are moving forward the speed is something which we can worry about a bit later so maybe make this 300 and as you can see it feels like they're actually moving but what's actually happening is the whole course is just moving the character is actually standing still so now our man is going forward we can finally go ahead and set up the obstacles itself I guess and add

10:17:57
in a jump State obviously because right now he doesn't jump so we can adjust the speed maybe 350 a little more quick would have been nice go ahead okay with that's something we'll worry about later now uh for our next step so I don't think we really require teleport so our X Y and Z is all set so for this we'll be using the jump as well so we'll go ahead and create a binding for our space bar space bar and we'll call this one jump and when I release this we are going to stop

10:18:47
jumping okay so now we should in theory just go up we can adjust the settings of the jump under our character movement component and we can also have animations so under our animation blueprint we can set it up so content blueprints game character and MBP we can ignore this and we can add a state and this going to be jump jump start and jump Loop jump Loop all right so jump start jump Loop and we'll see what animations we have and from our jump Loop we want to go back to our run animation basically

10:19:49
so jump start is going to be a third person jump and for the transition we'll have we'll check if we are jumping so we have our character reference here so is there any variable not sure we can try this okay nothing's really happening okay we are getting a runtime error saying we don't have the character ref so we'll only access this in the anim graph so go ahead if this is valid we'll go ahead and okay we we can check if this not valid first of all so we only get it once and occasionally

10:20:55
it's going not valid so we can promote this to variable and call this one jumping and in our transition can set it up okay so the variable isn't doing anything so we can head back to the character and create a variable for it in the first place so jumping now we can go ahead and set this to true we can go ahead and set this to false as soon as we release it get jumping okay this logic should work uh this is jump start to jump Loop so when our time remaining for our jump is less than let's say 0.005

10:22:11
seconds we'll enter this transition and jump Loop to third person run when this jumping is false basically so not not Boolean I guess it's called so we'll just invert the value now if I go ahead and press space okay the animation is weird so we can again do and maybe and if the jump Loop has at least played once so jump Loop so we can get access to the jump Loop here so time remaining time remaining for the jump Loop is less than 005 we can try this logic okay we just went went into a

10:23:19
completely random State there again probably some logical error okay so in our jump Loop we haven't fed the animation okay so our jumping logic is working so we can change this to maybe something a little more smaller 02 so this is going to feel a lot smoother okay so we are jumping now we can start adding the actual obstacles under the course we can head into obstacle base and over here we don't want anything this is not something we'll actually be spawning obviously obviously what will spawn is

10:24:27
going to be these [Music] so under obstacle one we can have stuff I'm not even sure at this point if we're able to see the sides we're barely able to see it and we also need to destroy it once we actually reach a certain point and we also need to keep spawning it basically so wherever our player start is so let's go ahead and add a trigger volume so trigger box so the x is going to be 20 the Y is going to be whatever this is and Z is going to be zero let's say and we'll just increase the extent

10:25:37
of the box maybe 500 500 and 500 okay and we'll set the hidden in game to false so hidden in game is false so f8 so this can go way ahead so a little more so we can select this trigger box and we can do time to by the way that's a pretty handy thing which you can do in Blueprint so just a little bit more so more okay I want to simulate now so go ahead and simulate okay so as soon as we end overlap on this we want to spawn a new one so go ahead on actor end overlap on actor end overlap trigger box

10:27:14
we'll try to print first okay so as soon as we go out of this uh first of all for the last index we'll go ahead and promote this to a variable so we'll call this one last spawn obstacle so we'll always have a reference to that go ahead copy this over so spawn actor we'll make use of this remember we had our Arrow component so the the arrow which is there opposite to the origin is what we need game course obstacle base so near the origin we have an arrow and over here as well we have an arrow we'll make

10:28:09
use of this Arrow so the location of this Arrow so this is called Arrow one so we'll call this one end so so that's a little more descriptive under the level blueprint now so we'll get the end so get end so get end and from end we can get uh get the location so get World location and we can probably copy this over just like that and we can change this to this and the rest of the logic should actually work just like that okay so now if we actually wait for this as soon as this goes away one more is going to

10:29:11
be spawned but there's another thing uh we want to destroy it uh once we actually go after a certain point we want to actually just destroy it like once we are behind the player we have no reason to still have it so we can have a trigger box for that once again so 500 maybe 500 and 500 go ahead and over here as well we'll set a big overlap for this instead so on actor Bea so so begin overlap on actor begin overlap destroy actor okay let's try this out so I'm not sure where this box

10:30:14
is uh let's unhide it so hidden game set to false okay so in theory we should be destroying it okay we destroyed uh the Box itself so other actor is what we have to destroy whoops we need to take this a little more further back so now if we wait for it to reach there so we are continuously spawning the box over there and if I actually head back into my view I cannot see anything happening and our world is spawning normally how cool so over here we can add a couple of things so up obacle one we can add a few

10:31:20
shipping containers maybe oh we can make it random actually that would be nice if we just make this completely random so somewhere at the center I'm not sure where the center is I think it's -600 but this is where the Center is going to be oops I moved the end itself so first duplicate it and this is going to be -600 this going to be Center obstacle and we can go ahead and duplicate this and this is not going to be called Center obstacle this is going to be called Left obstacle obstacle and we can call this one right

10:32:25
obstacle so our right obstacle is going to be to the right obviously and our left obstacle is going to be to the left obviously so this is 250 this negative 250 okay so we have set that up we should have done this in the base actually so we'll cut this and we'll paste this in a base so don't mind that now we should have our obstacle both in the base and the others and obviously the logic is going to be in base itself so since we are randomly spawning it it's totally fine we can use the base

10:33:15
itself I assume now in the event graph on event begin play we can go ahead and create a static mesh or rather spawn a static mesh at that location for that we'll need a few actor classes so obstacles over here we can delete these and we play everything should work however uh under our uh under this folder we can make a few actors actually so obstacles we'll call this path actually pathore base in case we need any derived classes now click on blueprint class actor and this is just going to be obstacle

10:34:23
one uh few will be dodgeable few will be not so we'll make uh Dot jable and non doj obstacles doj uh we'll just have three for each we'll create Childs so child contrl d control d and we'll name this one child three so 1 2 3 so this one is going to be non doible so we'll go ahead and create a child crl dtrl D and this is going to be Child 3 obviously okay so finally we can go ahead and add stuff to these obstacles so op obstacle dodgeable child one we can instead of the default scene

10:35:27
route obviously uh obstacle dodgeable here as well we'll simply have a static mesh static mesh so that's done we leave the root it's fine and we can look for some stuff here so we have quite a few meshes so we can have a barrel in one place so we can have boxes we can have barrels we have so many options here so we're going to select this let's say let's try this so in path you want to spawn actor from class so for the class we'll make this obstacle dodgeable so spawn transform is going to

10:36:32
be this so oops uh Center obstacle let's try this first so Center obstacle and get World transform go ahead and try this out okay it's just sliding along for some reason and we want to attach it yeah that's the reason so attach to component we want to attach this to our actual plane or we can just uh do it for the root comp component so now in theory this should work okay so this seems to be working fine uh one more thing we can make this a bit faster actually so we can promote this to

10:37:40
variable so speed so we'll make this one 500 okay as soon as we hit something uh we should stop and our game should get over so we'll have event hit here first we'll print something go ahead and test this out so if the other actor is an obstacle C to obstacle uh we should have made a base class to be honest go ahead and head into content blueprint game course obstacles we'll create one called actor of type obstacle obstacle iCal base and we'll inherit these from the base classes so class

10:38:58
settings so obstacle obstacle base and these will also change so We'll Inherit this from obstacle base so obstacle base obstacle base all right so we can go ahead and cost to obstacle base and we're going to print or rather we can just exit the game execute console command and we'll type in exit let's try this okay our logic is working okay we still hit it so we need a better jumping logic that's that's the problem with our jumping logic it's not our obstacles so under

10:40:03
this we can go ahead and change stuff in the character movement so under jump we should have this parameter here so if we change this to 500 for example so now we are able to dodge this obstacle successfully and they're a little bit too far apart I believe these obstacles so what we can do is we can have two actually in each one so go ahead and select all three of these so I'm not sure what 75% of 3200 so 75 into 3200 it's going to be 2400 so at400 we'll have it and we'll go ahead and duplicate

10:41:10
this so these and we'll have these at 800 so we'll have a gap of 1,600 between each obstacle and now if I go ahead and press play uh we have to set up more logic actually so we are spawning the obstacle dodgeable here uh now we'll make uh some non- dodgeable obstacles as well so set up the non- dodgeable one we can have some like a shipping container or something so the way I do it is going to be if I add in a static mesh once again and we'll have a shipping container maybe container okay we have quite a few

10:42:14
that's nice let's try with only the non dodgeable one non doible uh the rotations of go ahead and rotate it by 90° okay so this is not exactly on the floor but we can fix that head into to the left view okay it is on the floor not sure why it's not on the floor over there can try just moving it a bit that about fixed our problem and we obviously should be able to move aside and Dodge it so we are spawning obstacles and now we can set up a little bit of logic to make this random a little

10:43:58
bit uh for dodgeable we can have few more so for dodgeable we leave it as this child one let it be as this child two we can make something else so this static mesh can be we can look over what we have here can have this roadblock thing and change the logic obviously so do jabble I think it was child one so child one child two rather child two open it up I mean it is a bit down but you get the point so change that 10 20 we'll just move all of those by 20 units and for the third one as well we'll just

10:45:24
add one now obviously you can go ahead and make more of these I feel like if we have some sort of a traffic cone or something like that so I'm just looking for what I can have so okay these seem like the perfect choice let's try that again forgot to change it so under my path so course path base we can go ahead and change this to child three to test it again it's a bit low but that's not an issue okay I forgot to get the window in Focus once again that's my def fault and we have to move it down I

10:46:26
believe so move it down by 20 units okay so we have our dodgeable obstacles let's set up our non- dodgeable obstacles as well so in our child one can again look for what else we have maybe if we have a truck or something nope uh we can look for what we have so construction volume one measures so can have a fence yeah that's not a bad idea so this is child one so let child one be the same let's let's actually open up child 2 and let's actually open up child three so these are the ones which we'll try to

10:47:24
change over here meshes we'll select the fence for one uh the rotation can be zero uh change this non dodgeable child three so it's a little too big so we can scale this down maybe 8 okay so I don't think you can dodge this one okay we can dodge it when we move aside so we'll just have one last one so for this one so obstacle child two we'll change it right now so child two these are the various obstacles basically non dodgeable child two select that and this is child two I assume yep

10:48:44
so we can look for something else which we may have okay this looks like something interesting or light generator whatever this is let's try that I don't think this should be something which you should be able to dodge okay so that works now we can set set up some randomizing logic so that we spawn everything in random so this logic is the same we need to select the class basically first we can select a random integer So Random integer so this is going to be the number of uh random integer in range

10:49:41
actually so this is going to be the number of dodgeable obstacles so we need at least one dodgeable obstacle otherwise the game's going to get unplayable so we can either have one or we can have all the way up to three and what we can do is depending on the number now this is going to be number of dodgeable obstacles what we have so promote this to variable so number of dodgeable obstacles okay so now that we have this if we have only one what we can do is we can select one so number of dodgeable

10:50:28
obstacles so we can switch on int and we can select something so so we can start at one so start pin at one if we have only one obstacle our logic is going to be really simple so we'll just select a random one over there we need to do this Two Times by the way or multiple times probably I'm not sure so uh we'll have we'll have more obstacles to be honest these are not enough so we'll spin past them a little more closer copy these right obstacle left obstacle Center obstacle control D to

10:51:31
duplicate and left obstacle to where Center obstacle to okay we didn't duplicate everything so Center left and right so Center left and right control D to duplicate okay we we aren't duplicating anything we'll just duplicate these so okay left Center and right can move this somewhere in the center right at the center and we can space these two equally apart which I believe they already are are they fully spaced yep but we need to space them out a bit more we have 800 for the spacing

10:52:29
here so we can select our obstacle one we can try giving you know negative 600 maybe so if I do4 400 so that will be way too much space 500 maybe we can try 600 have 3200 let's divide it let's take 33% of that so calculator so it's somewhere around [Music] 1066 so so we'll have 600 it's fine if they're not equidistant you can obviously do the math yourself so obstacle is what we need so one oops two and three so 32 00 - 600 is going to be 2600 okay now let's see if this

10:53:53
works yeah obviously we are not spawning it that's different but now in theory we our logic should work so we can actually Loop through so we can select the number of dodgeable obstacles for each level so we'll have uh an array of this so we'll create an array I'll change the type it's fine so we can do for each Loop and for each index we can try and get a random integer so we can set array element so this is the index we can do a simple for Loop so for Loop so from zero to two so size to fit we'll do

10:55:00
that and we'd actually want to reserve three locations so 1 2 3 so we don't need size to fit so in this index we're going to set this item so for all our three levels we have we know the number of obstacles which will be dodgeable once we have that number we can go ahead and spawn them so we can have this in an array and randomize them actually anyways don't worry too much about the logic just my logic which I'm making up we can select this so we can store these in an array so create an array

10:55:57
so promote to variable or we can actually just have an array so what are we using this for we just using this for the location so we can get the transform of this we can only have the transforms in the array that would work I guess so first we'll have the transforms go ahead and create an array for transforms transforms one transforms 2 transforms three we'll need three arrays so we'll the location is enough for us so array of vectors transforms 2 transforms 3 I know I shouldn't be calling them

10:57:01
transforms but we'll take a look at the right obstacle uh the first level ones basically so we have this selected so right obstacle one we'll we'll go according to naming order transforms one we'll compile this blueprint so we have three elements uh we can access it right here so the first one is going to be this I'm not sure if we can paste this if we can we have right obstacle copy this okay we took that so left obstacle copy this and and okay the right and the left have okay they

10:57:56
don't so paste one has -250 and the center one have probably we'll probably have zero so we'll paste it we'll have zero over here okay and now that we have this let's grab our obstacle twos or obstacle ones so this is -600 1 2 3 -600 this will be constant so one is going to be 250 another one is going to be netive - 250 similarly we can grab our two so -600 this is basically our midpoint -600 250 -250 and this is about it now once this is done we'll collapses to function so

10:58:58
determine number of dodgeable obstacles okay we have the number of do jable obstacles now now what we can do is we can Loop through this so for each loop I really wish we could have a two dimensional array for this that would have helped us a lot now what we can do is we can go ahead and randomize this can we not randomize this okay we cannot so we have a plug-in which which will help us so low entry we can restart save everything all right so back here I think now we should have okay we're

11:00:18
coming close to 2 hours I think this will be done in 2 hours not one blueprints game uh course path base and we should have a randomize oops nope we don't so I think we might need a few functions so how do we go about random randomizing this we can look at the epic games launcher if we have any plugins so array helpers I guess I had one so we'll go ahead and install this to the engine we can simultaneously use it once we have this so once we actually randomize this uh depending on this we can go

11:01:11
ahead and set this so switch on int and we'll use select for this so we just close the editor just to let that happen and now if we go ahead and launch Our Endless Runner okay go to edit uh plugins so edit plugins and array array helper go ahead and restart so this is the sort of stuff I just hope it doesn't take too long right hopefully we have some sort of a randomize function so randomize okay we still do not have a randomize opt uh option so let's just look for it so randomize array unreal I don't

11:02:28
know is it called is it just called something else so okay never mind it's called Shuffle so first of all we'll Shuffle the arrays we'll shuffle all the three we'll do that before we actually set this we'll go ahead Shuffle this go ahead and Shuffle this once again uh we'll put that in the previous function itself so we can go ahead and Shuffle generally I don't recommend you guys uh do array operations in Blueprint but but anyways once this Loop is completed we can do that and this will

11:03:21
go to the return node just for you to understand the flow of logic here and now depending on this we can go ahead and spawn them so the array element is going to be the number of obstacles so this switch is going to start from one so start index is one you'll either have 1 2 or three so if you have one or two we can use select probably copy this over so everything else is zero so we can just leave it as this so we can go ahead and over here if this is one if we have one doible obstacle we can go ahead and

11:04:27
spawn just one of them as dodgeable so dodgeable so one is going to be dodgeable and the spawn transform we'll just use the first index so we we'll select so depending on which index it is so transform one transform 2 transform 3 so option one option two and option three so we'll select any one of these arrays and if we have to spawn only one do jble so we can get uh we can get a copy of the first one we'll split the struct pin here and we'll just get this location now we we need to just repeat

11:05:27
this logic so control D and we want to do two non- dodgeable ones so doible and index one and two are going to be non- dobl so non dodgeable uh we we have to spawn a child class of this so can use a select once again so Random integer and Max is going to be two so it's going to be Max is two so one and two so it's random number between 0 and Max minus one let's just use random integer in range so little bit confusing so minimum is zero maximum is two okay and this is going to be doible so

11:06:35
doible obstacle doible child one child 2 and child three this is this is what we have done and for this one this is non doible so we'll copy the logic but instead of dodgeable we'll have non dodgeable so child one child one child two and child three okay and we need this once again so copy over this entire logic all right so this is going to be the same this is going to be for index 2 now if we have two we can go ahead and copy this over so contrl C and control V and we can just move this aside

11:07:46
so for index zero it's going to remain the same oops control V oops uh copy this contrl C and contrl V uh index is still going to remain the same uh once this is done we need the attach as well we didn't copy over the attach okay so we we have to duplicate this whole thing so index is this and index is going to remain the same everywhere so now we need two doible obstacles so for this one as well we have dodgeable and this is going to be index one obviously and for index 2 we can go ahead and have

11:08:44
this all right right so copy this and again we can pass the index so array index go ahead and pass that in and when we have all three dodgeable obstacles uh we'll just go ahead and copy this much contrl C and contrl V so in case of three this is what we'll do so index is still going to remain the array index contrl D and crl D copy this over move the execution pins and the index will obviously just remain the same so the last one is going to remain the same and this is going to be two this is going to be

11:09:39
one and this is going to be zero so make sure you have 0o 1 and two okay so now our logic should work and if I were to go ahead and press play okay everything works okay all right so okay we stepped on to something uh we need to make sure this doesn't happen in our first one so okay we have to just ensure that the obstacles aren't spawned in the first one basically so we'll create a Boolean first box so if this is not the first box we'll go ahead and do this so inside the level blueprint

11:10:50
under this if we go ahead and refresh noes uh we have to pass this in so expose on spawn all right so now if I refresh I should get this so only if this is uh index zero so dou equal to 0 then this is the first box otherwise it's not okay so now our logic is working let's go ahead and play the game now all right so as you guys can see our game is working as expected we don't have a score yet we'll just set it up quickly so as you can see our logic is working so we can set up a scoring

11:12:06
system real quick and dirty here content uh we'll do the start thing also it's really simple so go ahead and open level um we call this one game map I believe so Maps game map go ahead and paste that in uh we can start from the main menu go ahead and play start and we started the game so as you can see everything is working as expected you could have some stuff at the side and we'll have a scoring system we can have a Time based scoring system so it's the score is going to go up at a

11:13:00
constant rate content we'll create a widget for it so uh user widget and we'll call this one on hard and we'll we'll just simply have a text so we'll wrap this with a canvas panel and this is going to be our score once we'll set the game mode and stuff so game map oh here we'll have BP uh we don't have a player controller we create that game go ahead head into blueprint class player controller bpor player controller so you should have BP play controller so on begin play we can go

11:14:11
ahead and create the widget so create widget it's going to be HUD and we can go ahead and add to viewport right so let's look at our time we don't have much I think it'll take probably just a little over 2 hours but it'll be done so once we create this we can grab a reference so promote this to a variable and we'll call this one heart now I don't recommend you guys use bindings but I think in this case just to make this real quick I'll use bindings so we can have game State uh on

11:14:52
construct we can get reference to the game state so get game State cost to BP game State and what we can do is we can grab a reference to it and we can create a score variable content blueprint uh have blueprint main menu I guess no game so game game State and we can have a score so we'll make this an INT 64 so that we can have larger scores so in iser 64 and we we can have a timer so set timer by function name and it's going to be something which happens every not. 5 Seconds let's say

11:15:55
and we're going to increment the score so promote to variable score timer and we can have a custom event increment score or increase I'll call it doesn't matter we'll not worry about that we are going to get the score and we'll set it to score plus two maybe plus set score so we'll go ahead and do that copy this put it in the function name make this looping and we can use a binding here so we can bind this we can get the game State can make this a validated G this is a little more expensive on your

11:16:43
computer so don't do this so we can get the score and we can convert this to text can use a format text node and stuff I'm not really going over that so we'll just do that actually so format text all right and we don't need to convert this if we press play as you can see our score is increasing at a constant rate and you can see it on the top left hand side for those of you on mobile phones and who are not able to see it I'll just make this text a little bigger so 40 make this one regular we don't need

11:17:41
bold and this should be good so as you can see everything is working fine and you can go ahead and set up any logic if you want if you want to like you know save it or whatever but for now I'm happy with this so that's it for this video guys thanks for watching we do have a complete game and instead of exit you can just uh show the score on a widget or something uh we'll do that uh let's not leave it halfway the last part before we just complete it so we'll create a widget and we'll call this one end

11:18:28
screen okay we'll add a border wrap this with a canvas panel so we can go ahead and wrap with canvas panel and this border should take up the whole thing so offsets are going to be zero and the brush color is going to be something black black maybe and we can just go ahead and add some text so we need to align it right at the center so vertical box uh we can use an overlay rather overlay is going to be helpful here so overlay so border is going to be filled the overlay is going to be filled

11:19:22
as well so 0 0 all right and over here we can have text and this is the advantage of using a canvas panel so 40 can make this regular maybe can go ahead and put score and we can go ahead and give the value so let's go ahead and set that so event construct get game State cost to our BP game State and we can get access to the score variable get score and we can set the text of this so set the text set text and this is going to be about it we'll format it so format text so this is the score

11:20:46
so let's go ahead and Center that make it 0.55 and make everything else zero here oops uh the size shouldn't have been zero uh make this one Center aligned and make sure for any vertical alignment which we have okay no we don't so I'll just just reduce the size of this maybe to 100 okay this should be good now if I go ahead and press play nothing will happen because we haven't spawned the end screen uh where we have our event hit in our character so we can cast to obstacle and

11:21:35
instead of that we can go ahead and create a widget create a widget end screen and we can add it to the viewport all right let's go ahead and do that so I'm testing the end screen so I'll just die immediately okay so our score is 300 apparently which is nice okay not sure why we didn't exit immediately there uh we need a do once I understood the problem so do once because once we die the game's over don't want to redo that so okay we need to do ones from here actually we just went over the obstacle which was

11:22:48
kind of stupid so go ahead and try this out and our score is 280 so that's it for this video guys I hope you guys really enjoyed this entire course I know it's been over 11 hours at this point but hopefully you have learned something new and I hope you enjoyed the last part where we actually made an entire game and we didn't use any C++ to be honest so that's about it hope you guys enjoyed and see you guys later goodbye

