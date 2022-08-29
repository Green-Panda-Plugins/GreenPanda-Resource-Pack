## About
Required resources for the Green Panda plugin pack.

## Installing

### Client
To install it on your client, download [release.zip][1] and put it in your resource pack folder.

### Server
This project is set up to automatically generate a new release.zip for every commit. You can optionally use [WorldResourcePack][2] in order to generate new hashes when a new version is released.

- Go to your server's server.properties
- Open it and find the key "resource-pack"
- Set the value to `https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/blob/main/release.zip?raw=true`.
- Restart your server

**TIP**: If you don't want the resource pack to update automatically (which removes the step of having to regenerate hashes), then you can instead link to a specific verison by replacing "main" with the SHA of a commit. You can find the SHA by going to [commits][3] and clicking the copy icon next to the version you want.<br>E.g. `https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/blob/f7c2a3464dc553f2ad1dc980032f9ce0b82bb4eb/release.zip?raw=true`

## Geyser support
If you're running the plugins on a server using Geyser to allow bedrock players to connect, you can still use this resource pack! You'll need to do some extra steps to set it up however. I use Kastle's [bedrock resource pack converter][4] to generate the bedrock resource pack, but it's set up to do this automatically so all you have to do is download it.

- First, you'll need a version of Geyser that supports custom model data. You can download it [here][5], or from the [github repo][6].
- Next, download the bedrock resource pack files. Navigate to [actions][7] and download the artifacts from the latest workflow. 
- Upload the resource pack `geyser_resources.mcpack` to the `packs` folder of your Geyser folder. 
- Upload the mappings file `geyser_mappings.json` to the `custom_mappings` folder of your Geyser folder.
- Restart your server

**TIP**: If you don't see the custom mappings folder, you need to start the server for Geyser to generate the folder the first time.

[1]: https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/blob/main/release.zip?raw=true
[2]: https://www.spigotmc.org/resources/world-resourcepacks.18950/
[3]: https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/commits/main
[4]: https://github.com/Kas-tle/java2bedrock.sh
[5]: https://ci.opencollab.dev/job/GeyserMC/job/Geyser/job/feature%252Fextensions/
[6]: https://github.com/GeyserMC/Geyser/tree/feature/extensions
[7]: https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/actions?query=branch%3Amain+is%3Acompleted
