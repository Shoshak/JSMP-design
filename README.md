# JSMP
*J stands for Just*
# Main principles
1. Prevent chaos not by enforcing server-wide strict rules, but by giving everyone, even beginner players, a chance for self-defense
2. [Deus otiosus](https://en.wikipedia.org/wiki/Deus_otiosus)
3. Any player can only gain an advantage through self-reliance, using in-game methods, without any external help, be it from another human or a non-human actor
# Worldborder is fixed at 10000 blocks
## Constants
- Average player speed while sprinting and jumping - 7.127 m/s
- Average boat travel speed - 8 m/s
- Duration of one Minecraft day - 20 minutes/1200 seconds
- Block length - 1m
## Reasoning
- For better player experience, you should be able to walk from one side of the world to another in one minecraft day. That results in a world that is 8520 blocks long (`7.1 * 1200`).
- The world should not be infinite due to the server having chunk pregeneration, backups and finite disk space
## Some players travel by boat
- Due to boat travel, the world should be about 12% bigger (8/7.127 = ~1.12) than walkable baseline.
## Preference for bigger world sizes
- Fear of not having enough resources in the border. Mitigated by having all resources present inside the border (see section "All resources are present inside the border")
- Less interaction with other players. Mitigated by playing singleplayer
## Preference for smaller world sizes
- More interaction with other players. Mitigated by having a fully walkable world.
# All resources are present inside the border
## Reasoning
- All resources available in-game should be obtainable for anyone
## Biomes present
- Mushroom fields
- Cherry grove
- Mangrove swamp
- Desert
- Savanna
- Badlands
- Lush caves
- Forest OR flower forest
- Taiga OR Old growth taiga OR Snowy taiga
- Jungle OR Bamboo jungle
- Frozen ocean OR Deep frozen ocean
- Jagged peaks OR Frozen peaks OR Snowy slopes
- Soul sand valley
- Crimson forest
- Warped forest
- Basalt deltas
## Structures present
- Ancient city
- Mineshaft
- Stronghold
- Buried treasure
- Pillager outpost
- Village
- Woodland mansion
- Shipwreck
- Ocean ruins
- Ocean monument
- Nether fortress
- Bastion remnant
## Running out of resources
- The server is private and thus does not have nearly enough players for that to realistically happen (see section "Server is whitelisted")
- Even if it does happen (to some extent), this will create competition, which is, arguably, more interesting than an abundance of resources
# You can no longer enchant netherite or diamond armor with protection
## Reasoning
- TTK of an iron axe should always be less than 8 seconds
- See main principle 1
# You can no longer boost yourself with fireworks while using an elytra
## Reasoning
- Elytra is one of the fastest methods of transportation that does not require any specific structures, biomes, weather conditions or attitudes to work
- Elytras are only available to players that have enough resources to travel to end cities
- See main principle 1
## Other methods being too slow
- Elytra is still the predominant (and the fastest) method of transportation if you have a high enough structure
- Hyperloops and "Dolphin's Grace status effect with Depth Strider III and Soul Speed III on a layer of soul soil underwater" are faster
# Server owners cannot interfere with the gameplay in any way
## Reasoning
- See main principle 2
## Emergency situations
- All emergency situations are announced to the community
- The community decides if the methods used to handle the emergency situation were applicable. If not, all reversible decisions made while handling the situation are reverted, and, if demanded by the majority of the community, a compensation to the victims is given
# Server opens and closes at fixed times throughout the day
## Reasoning
- No player shall gain an advantage simply by having a different daily schedule
- Server owners need time for maintaining the server
## Schedule differences
- Opening and closing times are decided by community vote
# Server is whitelisted
## Reasoning
- Effectively prevents bot attacks from happening
- Results in a more civil, localized community
# Anticheat is implemented
## Reasoning
- See main principle 3
## Anticheats presents
- Paper anti-xray
- GrimAC
## The "treadmill problem"
*in software development - a task that occupies an infinite amount of a programmer's time, because there's endless upkeep*
- Since the server is whitelisted (see section "Server is whitelisted"), it would be pretty easy to spot bad actors and punish them, since the amount of players is finite
- The goal of an anticheat is not to solve cheating completely, it is to discourage people to even try it
# Authentication is implemented
## Reasoning
- Prevent players from sabotaging or helping other players
- See main principle 3
## How is it implemented?
- If `offline-mode = true` - Mojang will take care of it
- If `offline-mode = false` - external authentication plugin
