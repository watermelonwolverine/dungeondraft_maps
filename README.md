# How to find out which asset packs were active for a map?

Open the dungeondraft_map file with a text editor (like Notepad++). You will see text in json format.
Under `header` -> `asset_manifest` you will find all asset packs listed that were active when the map was last saved. This doesn't mean all packs were actually used though. This is an important difference because I always activate all my packages but usually don't use them all.

## Optional: Find out which asset packs were used

If you don't want to download or purchase all the asset packs only to later find out they weren't actually used read this section.

To find out if they were used and if you need to get them search the file for the `id` of the asset. If you can't any references to that id the asset pack was never used.

### Example: 


    {
        "header": {
            "creation_build": "1.0.1.3 awaken dryad",
            "creation_date": {
                "year": 2021,
                "month": 8,
                "day": 18,
                "weekday": 3,
                "dst": false,
                "hour": 17,
                "minute": 32,
                "second": 21
            },
            "uses_default_assets": true,
            "asset_manifest": [
                {
                    "name": "CH - Buildings",
                    "id": "DZw7eElc",
                    "version": "0,6",
                    "author": "Crosshead",
                    "custom_color_overrides": {
                        "enabled": false,
                        "min_redness": 0.1,
                        "min_saturation": 0,
                        "red_tolerance": 0.04
                }
                }
            ],
            }
        ...
    }


This means that CH-Buildings asset pack of version 0.6 was used.
The id of CH-Buildings asset pack in this example is `DZw7eElc`. So to check if this asset pack was used we would need to search (usually Ctrl+F) for `DZw7eElc`. If we can't find any other references than the one under `asset_manifest` the pack wasn't used.

# Where to find the asset packs that were used?


|Name                             |Version        |URL                                                                   |
|---------------------------------|---------------|----------------------------------------------------------------------|
|Crosshead                        |1              |https://www.patreon.com/Crosshead                                     |
|CH-Buildings                     |0.6            |https://www.patreon.com/Crosshead                                     |
|CH-Gardens                       |1.0            |https://www.patreon.com/Crosshead                                     |
|CH-Giant                         |0.2            |https://www.patreon.com/Crosshead                                     |
|CH-Nature                        |0.4            |https://www.patreon.com/Crosshead                                     |
|CH-Prefabs                       |0.1            |https://www.patreon.com/Crosshead                                     |
|CH-Ruins                         |0.3            |https://www.patreon.com/Crosshead                                     |
|CH-Sea                           |0.4            |https://www.patreon.com/Crosshead                                     |
|CH-Team                          |0.6            |https://www.patreon.com/Crosshead                                     |
|Darkness                         |1              |https://cartographyassets.com/assets/15323/darkness-terrain-brush/    |
|Krager's Shadows & Light Pack    |1.0            |https://cartographyassets.com/assets/7713/kragers-shadow-light-pack/  |
|Crosshead modified               |1              |In this repository in the "assets" folder                             |

# Support

If you want to support me you can:

- Become a Crosshead (https://www.patreon.com/Crosshead) patreon so they can make more assets
- Purchase Dungeondraft (https://dungeondraft.net/) so they can further improve their program
- Upvote my posts in reddit: https://www.reddit.com/user/YummyOr4nges
- Share your own work
