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
- Fear of not having enough resources in the border. Mitigated by [having all resources present inside the border](#all-resources-are-present-inside-the-border)
- Less interaction with other players. Mitigated by playing singleplayer
## Preference for smaller world sizes
- More interaction with other players. Mitigated by having a fully walkable world.