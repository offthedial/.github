# updating Off the Dial data for new seasons
> [!NOTE]
> If you don't have permission to modify the files directly, create a pull-request.

## adding new weapons to the site
1. Navigate to https://github.com/offthedial/site/blob/HEAD/src/components/weapons.js. This is where the weapon data is stored.
1. Replace the `importedWeapons` variable with the new weapons data from the corresponding `weapons.json` file linked to in the file.
1. Delete all non `MAIN_` weapon keys.

## adding new maps to the bot & overlays
1. Navigate to https://github.com/offthedial/bot/blob/master/offthedialbot/commands/to/maplist.py#L80. This is where the maps are stored
1. Add new maps to the list, make sure the maps follow the order listed in the corresponding `stage-ids.ts` file linked to in the file. That way it's in sync with the sendou.ink map generator.
1. For the overlays, navigate to https://github.com/cq-overlays/dashboard/blob/37870663e84ec2f55cc4e557ec89c0faf91c70f7/schemas/loadedData.json#L125.
2. Do the same thing, add the new maps to the list.
