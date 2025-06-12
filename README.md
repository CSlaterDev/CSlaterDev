Hi, I'm Connor! Welcome to my portfolio.

I have several ongoing projects right now, some games (mostly made in Unreal Engine) and some mods (mainly for the game Skyrim). Please take a look at some of the recent things I've been working on below.

I'm currently working on a crafting-focused RPG similar to Stardew Valley. While progress is ongoing, so far I've implemented several complex features that I am happy with.

 <img width="1920" alt="game1" src="https://github.com/user-attachments/assets/ea70047b-7a37-4b69-aec6-7fbef5b661c6" />


## **Features**


### **Schedule system for fully independent NPCs**

The game has a complete NPC schedule system, allowing NPCs to act independently, travel between levels, and perform complex behaviour based on the time of day, day of the week, or even arbitrary coded requirements. NPCs can move through and travel between levels even when the player is in another level, making them really seem like independent actors. The system even allows for special dynamic events to occur - for example, if something catches an NPC's eye, the NPC is able to "think" if it's worth interrupting their schedule for. If they're just out for a walk, they're more likely to interrupt their schedule than if they're going to bed. As each NPC has a unique schedule, it allows for great displays of each NPC's individual personality.
The NPCs themselves are persistent characters within the game world, able to level up and equip items independent of the player.

 <img width="1147" alt="game2" src="https://github.com/user-attachments/assets/29d020d7-d2a9-4ce3-bcf0-09ddadc5196b" />


### **Dialogue System**

The game allows for conversations between the player and multiple NPCs, complete with NPC and player portraits, a typewriter effect and arbitrary code execution based on player responses, or at certain points in the conversation - for example, opening a shop menu.


### **Items & Crafting**

Every instance of an item in the game is unique, with generated stats, traits and innate elements. The range of the generated stats is controlled by a data table / csv file, with each area in the game allowing for its own stats and traits for each item.

Items can be combined in a crafting minigame into brand new items, carrying over traits from the base parts. This allows for the creation of unique, powerful equipment.
 
<img width="1003" alt="game5" src="https://github.com/user-attachments/assets/96912f04-f33f-4165-ba4f-3a6098edb386" />


### **Quest System**

The game has a robust and versatile quest system, which can be used for anything from your typical "fetch" quest, to background quests which monitor the player's actions and progress and trigger special events at specific points. Quests are capable of listening to several game events and starting or updating themselves based on parameters defined in each quest. In addition, the quests support arbitrary code to decide whether they can or should start, allowing for even more flexibility. The quest themselves track both their stage and state, stage is a simple integer which allows for nearly infinites steps in a quest, with state being used to track things like whether the quest has started, whether the player completed it or failed it etc. Quests feature several event dispatchers which allow the rest of the game to react to quest updates, and also the quest itself to easily react when its state changes without having to directly call a function to do something. In addition, both active and inactive objects can be passed to quests so that quest can observe and access their events - for example, to trigger a quest update when an NPC kills something. All quest data carries over between levels. The quest system is extremely flexible and can be used for almost anything without repetitive set-up or extensive custom code.

 
<img width="972" alt="game4" src="https://github.com/user-attachments/assets/713aeb79-f28c-4699-9902-62c1a7f041d4" />


 
<img width="434" alt="game3" src="https://github.com/user-attachments/assets/a9117483-e08f-4e8d-abc0-130ea1179624" />




## **Mods**

I've been active in the Skyrim modding community for several years and have published multiple mods. In the past, I mainly created small bug fix mods to fix things that are forgotten or left out by the larger patch mods. These mods were created using the official toolkit for modding and using Papyrus, the propriety scripting language used by Skyrim, which I had to learn. Recently, I wanted to do something more complex and do something that had never been done in Skyrim before, while also enhancing my C++ skills. 
My goal was to create a complete degradation system for all armor pieces in Skyrim, as well as other new custom data not found in Skyrim, such as size for a particular armor piece. While other degradations mods do exist, they all make use of the game's existing tempering system and have various limitations, such as not affecting NPCs, or visibly updating containers or NPCs when the player interacts with them. I wanted something that worked seamlessly, as if it was a part of the base game. To do this, I needed to create a C++ plugin which hooked into the game's code at launch and replaced game code with my own. Thankfully, this was made much easier by the work of talented modders who have created systems to more easily do this. While there were a few bumps in the road, I'm very happy with how the mod turned out, with it receiving over 300 downloads in its first week and earning a spot on the trending page of the largest Skyrim modding site.







<!--
**CSlaterDev/CSlaterDev** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
