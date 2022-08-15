## About
Required resources for the Green Panda plugin pack.

## Installing

### Client
To install it on your client, download [release.zip][1] and put it in your resource pack folder.

### Server
This project is set up to automatically generate a new release.zip for every commit. [WorldResourcePack][2] is optional but recommended to regenerate the hashes when a new version is released.

- Go to your server's server.properties
- Open it and find the key "resource-pack"
- Set the value to `https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/blob/main/release.zip?raw=true`.
- Restart your server

**TIP**: If you don't want the resource pack to update automatically, then you can instead link to a specific verison by replacing "main" with the SHA of a commit. You can find the SHA by going to [commits][3] and clicking the copy icon next to the version you want.<br>E.g. `https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/blob/f7c2a3464dc553f2ad1dc980032f9ce0b82bb4eb/release.zip?raw=true`

[1]: https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/blob/main/release.zip?raw=true
[2]: https://www.spigotmc.org/resources/world-resourcepacks.18950/
[3]: https://github.com/Green-Panda-Plugins/GreenPanda-Resource-Pack/commits/main
