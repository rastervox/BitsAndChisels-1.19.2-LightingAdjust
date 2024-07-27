# Bits And Chisels
![Java CI with Brachyura](https://github.com/CoolMineman/BitsAndChisels/workflows/Java%20CI%20with%20Brachyura/badge.svg)
[https://github.com/CoolMineman/BitsAndChisels](https://github.com/CoolMineman/BitsAndChisels)

Bits and Chisels is a Fabric mod for modern Minecraft that lets you remove small bits from blocks using chisels. You can use these bits to build detailed decorations or whatever else you want. Requires Fabric API. Has Canvas Renderer support for shaders. Uses greedy meshing and the Fabric Renderer API to achieve high FPS post-1.13 rendering changes. This mod was inspired by Chisel and Bits.

This is a quick fork I made when I wanted to make small lightbulb and lamp style lights, but the light value never got above 2. I don't know Java or Minecraft modding at all.

Still in the process of trying to find how to build the jar

# Build Instructions
Okay, so this was a process. It too a while to figure this shit out, because nobody who forked Bit-and-Chisels made it easy for people to figure out what to do. This instruction is here so nobody has to go through the same mess of an afternoon that I did just to change a little bit of code.

So, to build Bits & Chisel on your own, you gotta:

1. Run the brachyura-bootstrap-0.jar from admin command prompt

cd (your source directory)
java -jar brachyura-bootstrap-0.jar

2. If there is an error, remember to install JDK 17 for windows. It should work then.

3. Run the same thing, but with "build" at the end

java -jar brachyura-bootstrap-0.jar build

4. It will likely spit out a directory where it tried to download Stacc-1.3.4.jar, and failed. Either get the Stacc jar frm your modpack you are already using, or find a jar of it online, and put it in the directroy, with the exact name that the error message has put.

5. If it doesn't work, the only other thing I did was change the url in the Buildscript.java file from "https://storage.googleapis.com/devan-maven/" to "https://ueaj.dev/maven"

6. The build SHOULD be in the build folder. If there was an error, that is up to you cause I have no idea what would have gone wrong.