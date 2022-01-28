# MavenMCP 1.8.9

### About
Maven MCP 1.8.9 is an updated version of MCP. It uses Maven, has a clean code structure, supports Linux and version control in your projects!

### About the structure
The code is split into two groups: Resources (assets, graphics, shaders etc.) and code.<br>
Libraries are loaded from Maven.

### Setting up workspace
1. Clone the repository
2. Let it setup and index (just wait)
4. Specify project SDK to **Java 8** It might not work with other versions of JDK
5. Once it indexes, the project should be ready to go! :)

### Building
To build a working .jar file, which later can be put to `/versions` in MC folder, you just need to run `mvn clean package` command.
<br>You can also use the Maven menu *on the right side*, or add a new run configuration, and run it from there (my favourite way).
<br>Once the process is complete, artifacts will be in `/target` directory.
<br>There's no requirement to delete MANIFEST from the jar before putting to MC folder.

### Running
To launch the client in the IDE, you need to execute Start.java, **and specify working directory to `./test_run/`**.<br>

An example run configuration.<br>
<img src="https://developers.marcloud.net/i/launchConfig.png"/>

Minecraft's directory will be `./test_run/`. All saves, resource packs etc. will be there.

### Migrating from old version of MCP
Nothing easier. 
Move your existing java code to `/src/main/java`, and any resources i.e. shaders, fonts etc. to `/src/main/resources`.
If you added new libraries, make sure to add them to pom.xml, and you're set :D

### Support
If you have any questions about this repo, let me know on <a href="https://marcloud.net/discord">my Discord</a>! ^^

<br><br>
**May 1.8.9 survive!**