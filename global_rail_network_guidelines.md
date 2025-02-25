# Global Rail Network Guidelines
One goal of the server is to build a public rail network that connects the entire world like in real-life countries. Here are a few basic guidelines to make this possible.

> [!WARNING]
> We have set the max train speed to 300 km/h (even in curves) in the Config. **PLEASE set the max speed of EVERY train and EVERY track according to the speed guidelines mentioned below!**

- ### Coordination
  Keep up to the [standards](https://github.com/MisterJulsen/MinecraftCommunityServer/blob/main/standards.md) and make sure existing rail traffic is not affected when extending the network (e.g. new track, new train). If in doubt, ask Server Staff or Trusted Players. Use `#public-railways` in discord to discuss.
- ### Stay realistic
  No tight curves, unrealistic track switches, overlapping tracks (crossings excluded), steep climbs/descents, floating tracks
- ### Exceptions
  Exceptions are possible at any time, but should be clarified with the affected players or the Server Staff (e.g. before building a new/special track at a train station)
- ### New routes
  Use existing infrastructure if available, before building new routes.
- ### New Scheduled trains
  Before sending a scheduled train onto the rail network, make sure not to cause any problems on the route (e.g. blocking other trains with long waiting times) and the desired route is not already operated by other trains (Overcrowding). If in doubt, ask Server Staff or Trusted Players.
- ### Trusted Players
  Players who already have experience in the public rail network and make responsible decisions. Every player can reach this status.
- ### Private rail networks
  Do not build a private rail network next to the public in a similar scale (local subway/tram/train network excluded). Instead, expand the public network.
- ### Train Speed
  Every train on the public rail network must specify the maximum speed of its category at the beginning of the schedule. (e.g. 50% for regional trains) [You can find exact values ​​in the standards.](https://github.com/MisterJulsen/MinecraftCommunityServer/blob/main/standards.md)
  For that use the "Set Primary Speed Limit"instruction at the start of the schedule as shown:

  ![Example of a train schedule with max speed](https://github.com/user-attachments/assets/973c04b1-4ee2-4c23-8adc-826228f53f6b)

- ### Train Dissasemblng
  Dissasemble trains only at private rail yards to avoid trains braking platform edges and blocking tracks.

- ### Track Speed
  On each route, the maximum track speed **MUST** be set (independently of the trains) by train signs, depending on the environment (e.g. straight track, curved track). Before curves, the speed must also be temporarily reduced. There are no specific values, it is done by eye and what feels realistic. For basic routes, we recommend 50%, on straight high-speed routes, 100% can be used.
  
  ![Train signs to set max speed](https://github.com/user-attachments/assets/823f66c5-b914-46fc-b033-f5b94c0e5cce)  
  ![Temporary speed limit before curves](https://github.com/user-attachments/assets/a8aded5f-b374-4f92-878f-fdbd1dc4ca99)
  ![End of temporary speed limit after curves](https://github.com/user-attachments/assets/7d996a91-1a48-4ed5-8d36-ab97f11278ae)

- ### Level Crossings
- #### Automatic Level Crossings
  Automatic level crossings should:
  - Trigger at least 20 seconds before the train reaches the crossing. Distance can be figured out from line speed using the formula:
    ```
    line speed percentage * 83m/s * 20s = min distance between crossing and trigger
    ```
  - Have both visual and audio warnings which are self contained (i.e. whistle boards do not count).
  - Have barriers. These should not close on both sides of the road (half barriers), this is in case pedestrians or vehicles are on the crossing when the barriers close.
- #### More basic crossings
  Automatic level crossings may not be suitable for certain areas, such as rural areas with not much use. They should:
  - Be clearly marked with signs requesting that they should look before crossing.
  - Have a whistle board and/or another form of audio warning.
  - Approaching trains must be clearly visible and enough time should be given for a pedestrian to cross before a train reaches the crossing.
  - If exposed to road traffic, the open crossing should be marked with a railway crossing sign/x.
  - If exposed to road traffic and warning lights are not used, give way/yield signs or stop signs should be used.
  This type of crossing may also:
  - Have warning lights. These must trigger 20 seconds before a train reaches the crossing as described above.
  - Have a gate.
  - Have barriers which make pedestrians zigzag and pay attention
- #### More advanced crossings
  Where half barriers are not suitable, full barriers may be used, however, these **MUST** be monitored during and after closure by either a crossing operator, signaller, or train crew. A train should not proceed until it is confirmed that the crossing is safe, this could be done using a signal that is usually powered (making it show danger).
