![MonoGame.Extended Logo](https://raw.githubusercontent.com/craftworkgames/MonoGame.Extended/master/Logos/logo-banner-800.png)

# MonoGame.Extended
It makes MonoGame more awesome.

[![Join the chat at https://gitter.im/craftworkgames/MonoGame.Extended](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/craftworkgames/MonoGame.Extended?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](http://build.craftworkgames.com/app/rest/builds/buildType:(id:MonoGameExtended_CI)/statusIcon)](http://build.craftworkgames.com/viewType.html?buildTypeId=MonoGameExtended_CI&guest=1)

MonoGame.Extended is an open source extension library for [MonoGame](http://www.monogame.net/). A collection of classes and extensions to make it easier to make games with MonoGame. 

## Version 0.5 is available on NuGet
MonoGame.Extended v0.5 has been published as [a NuGet package](https://www.nuget.org/packages/MonoGame.Extended/) and can be installed now. Please read the [install guide](https://github.com/craftworkgames/MonoGame.Extended/wiki/How-to-install-MonoGame.Extended) to setup the Pipeline tool.

    Install-Package MonoGame.Extended

This release is compatible with MonoGame 3.5!

**Note**: If you're still using MonoGame 3.4 you must upgrade to 3.5 for everything to work.

## Forums
Our forum is part of the [MonoGame community](http://community.monogame.net/category/extended). Please ask any questions or post about problems or bugs that you have found there. Let us know if you're making a game with MonoGame.Extended!

## Development status
MonoGame.Extended has a growing community of contributors adding to the project all the time. We also have [Nuget packages](https://www.nuget.org/packages/MonoGame.Extended/) of published releases and of course you can [build from source](https://github.com/craftworkgames/MonoGame.Extended/wiki/Building-MonoGame.Extended-from-source) to get the latest and greatest.

Please keep in mind that the project is still evolving. Some breaking API changes are likely to occur as we progress.

## Usage
MonoGame.Extended is a portable class library that sits on top of MonoGame. It's designed to work on all supported platforms using a single portable DLL. At runtime, the portable library will call into the platform specific MonoGame DLL referenced in your project. If you do use it on another platform please [let us know](http://community.monogame.net/category/extended)!

## Documentation
We've got several feature demos in this repository and we're building up [the wiki](https://github.com/craftworkgames/MonoGame.Extended/wiki). You can also pop into [the forums](http://community.monogame.net/c/extended), check out [my blog](http://dylanwilson.net/), ask a question on [gamedev stack overflow](http://gamedev.stackexchange.com/questions/tagged/monogame-extended) or use our [live chat](https://gitter.im/craftworkgames/MonoGame.Extended).

## How to install

See the [How to install MonoGame.Extended](https://github.com/craftworkgames/MonoGame.Extended/wiki/How-to-install-MonoGame.Extended) guide. Here's the TL;DR version:

The library is distributed as a NuGet package. Add a reference to your project using the following command:

	Install-Package MonoGame.Extended

The package comes with 2 DLLs:

 - MonoGame.Extended.dll
 - MonoGame.Extedded.Content.Pipeline.dll
 
The `MonoGame.Extended.Content.Pipeline.dll` needs to be referenced by the [Pipeline tool](http://www.monogame.net/documentation/?page=Pipeline). To reference the DLL in the Pipeline tool you'll  need to edit your `Content.mgcb` file.

## Features

- **Tile based maps** using [Tiled](http://www.mapeditor.org/)
- **Bitmap fonts** using [BMFont](http://www.angelcode.com/products/bmfont/)
- **[Sprites](http://dylanwilson.net/sprites-and-spritebatch-extensions-in-monogame-extended)** (with SpriteBatch extensions!)
- **Particles** using the [Mercury Particle Engine](https://github.com/Matthew-Davey/mercury-particle-engine)
- **Input listeners** for event driven input handling (Keyboard, Mouse, Touch, GamePad).
- **Texture Atlases** using the JSON format in [TexturePacker](https://www.codeandweb.com/texturepacker).
- **2D Camera** with pan, zoom, and rotation.
- **Viewport Adapters** for resolution independent rendering.
- **Sprite Animators** using texture atlases.
- **Timers** including a continuous clock and a countdown timer w/ event integration
- **FPS Counter** that is handy for debugging.
- **Primitive Shapes** and sprite batch extensions to draw them.
- **Sprite Sheet Animations** - created with the [Astrid Animator](http://dylanwilson.net/introducing-astrid-animator) prototype.
- **Simple Collision Detection** - experimental.

## Contributing
If you would like to contribute start with one of the following:

 - Please post your thoughts on our [forum](http://community.monogame.net/category/extended).
 - Join the discussion on one of the [issues](https://github.com/craftworkgames/MonoGame.Extended/issues). We often use github issues to discuss new features as well.
 - Talk about it on your [blog](http://dylanwilson.net/) or [twitter](https://twitter.com/craftworkgames).
 - and of course, you can fork the project.

 
## Design goals
 - The primary goal is to make it easier to *make games*.
 - Choose the features you like and the rest stays out of your way.
 - A clean and consistent API familiar to MonoGame developers.
 - It's *not* a game engine, but extends the framework.
 - Follows [C# coding guidelines](https://msdn.microsoft.com/en-us/library/ms229002(v=vs.110).aspx).


## License

MonoGame.Extended is released under the [The MIT License (MIT)](https://github.com/craftworkgames/MonoGame.Extended/blob/master/LICENSE).
 
## Special Thanks

 - Matthew-Davey for letting us use the [Mercury Particle Engine](https://github.com/Matthew-Davey/mercury-particle-engine).
 - John McDonald for [2D XNA Primitives](https://bitbucket.org/C3/2d-xna-primitives/wiki/Home)
 - [LibGDX](https://libgdx.badlogicgames.com) for a whole lot of inspiration.
 - All of our contributors!
