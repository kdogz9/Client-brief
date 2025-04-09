# Development Commentary Template 

## Brief 

 How does the design of video game space affect the actions and experiences of players? Consider how different game spaces have been categorised in the literature and concepts of space and place discussed in the lecture.  


## Project Outline   (179)

The project we are making is heavily inspired by Little Nightmares (Studios, s.d.), as Super Massive Games is our client brief for this project. We came up with a game idea where the player is trapped in a witch's kitchen and needs to solve a bunch of different puzzles to escape from the witch. These puzzles involve making potions, pulling boxes to jump on surfaces, and avoiding objects that are falling. 

I found the beginning quite slow, but I enjoyed making a Figma board (Figma, s.d.) and breaking down each task I needed to do so that I could stay on track and understand what needed to be done for the game. I also enjoyed making a mood board of little nightmares (Studios, s.d.) and exploring images related to this game and also images for our own theme of a witch kitchen. 

I may run into some issues with working with the animations as I have never worked with animations before, but with the right documentation, I think I should be able to overcome this challenge and end up understanding implementing animations a bit better. 

## Research 

### Methodology  (91)

I copied the game mechanics that were discussed from the second week of the project and broke it down into simple mechanics so I knew what I needed to code. This made it easier to find what code I needed to implement throughout the project. I then highlighted each mechanic so I knew what needed to be done and what I had finished so I could keep on track. Breaking down the mechanics also helped me find the correct documentation I needed to be able to get help with the project. 

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\Client brief.png">
Figure 1. (Figma, s.d.), Mechanic Breakdown.

### Game Sources  (92)

Little Nightmares (Studios, s.d.) is a puzzle-based game where players control a small character navigating through a mysterious building filled with monstrous creatures. The goal is to escape the building without being caught. The environment is dark and atmospheric, relying heavily on the use of light and shadows to create tension. This approach has influenced our design, where we've intentionally crafted a dark environment with minimal light sources. Additionally, our character’s color scheme is designed to stand out in the shadowy surroundings, much like in Little Nightmares (Studios, s.d.), enhancing their presence in the eerie world. 

### Academic Sources  (119)

I recently read a book called *Animating Real-Time Game Characters* (Steed, s.d.), and one of the chapters discusses how the environment and space influence design elements, particularly when it comes to animation sets. This insight made me realize that focusing on character movement is crucial in defining the space around them. By understanding how a character moves, designers can better shape the environment to complement and enhance those movements.

I also read *3D Character Animation* (Clark, s.d.), which explores how timing can significantly influence a character's emotions and personality. The book emphasizes that animation plays a crucial role in conveying physical presence within a space, as the speed and pacing of movements can alter the context of a situation. 


### Documentation Sources  (172)
I used in-depth YouTube tutorials to create the game mechanics our group had discussed. I utilized UI tutorials to develop a game menu (How To Create A Main Menu - Unreal Engine 5 Tutorial, 2022). Additionally, I followed tutorials for creating an interactive system, allowing objects to be picked up (How To Pick Up And Drop Items | Hold Items In Hand - Unreal Engine Tutorial, 2021). I also learned how to implement a potion mechanic through another video (Unreal Engine - Ingredient Pickup and Potion Crafting, 2025). By adapting the techniques shown in these videos, I was able to tailor them to meet the specific needs of our project. I also referenced some documentation sources on the Unreal Engine website. This was helpful as I was able to see people's discussions and how they broke down the issues they had and how they were solved. This was a more beneficial way of learning sometimes. (How can I change a character's jump height in blueprints? - Development / Character & Animation, 2017)

## Implementation (Suggested Word Count 1,100)  

### Process (887)

The development process for the project began with coding a crouch mechanic, followed by creating a simple pick-up and put-down system (How To Pick Up And Drop Items | Hold Items In Hand - Unreal Engine Tutorial, 2021) for the potion once the player makes it. I used a cube as a placeholder for this system.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image.png">


Figure 2. [BlueprintUE](https://blueprintue.com/render/n0rvq9nz/), Crouching implementation.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-12.png">

Figure 3. [BlueprintUE](https://blueprintue.com/render/4183zttv/), Pick up and put down implementation.

 I then worked on a pull and push system to allow the player to move boxes around for puzzles and to reach higher platforms, using force and velocity. This was a key milestone as it involved important coding concepts that were essential for me to learn. 
 
<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-1.png">
 Figure 4. [BlueprintUE](https://blueprintue.com/render/k_78x6s9/), Pull implementation in the player blueprint.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-11.png">

 Figure 5. [BlueprintUE](https://blueprintue.com/render/a5ptvy0q/), Pull implementation on the object itself. 

 Next, I implemented trigger boxes (How To Use Trigger Box - Unreal Engine 5 Tutorial, 2024) to make objects fall (how to make items fall when the player enters a zone unreal engine 5 - Google Search, s.d.), which also became a significant learning point as I grew more comfortable using them throughout the process.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-2.png">

  Figure 6. [BlueprintUE](https://blueprintue.com/render/ydz6hjrb/), Trigger box implementation.

I added a kill tag to items and set the death (A destroy actor and respawn tutorial., 2022) mechanic on the player instead of the objects, which helped avoid repeating code and creating blueprints for each object that would kill the player.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-3.png">

Figure 7. [BlueprintUE](https://blueprintue.com/render/cxr7iml9/), Death system implementation.

 I made the player have a rag doll animation when they were killed. This was influenced by my academic research (Clark, s.d.) which led me to focus on creating a ragdoll animation for the character when killed, as it allows the player's death to be communicated more dramatically and realistically, changing the emotional tone of the moment and adding to the overall experience.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-4.png">

 Figure 8. Rag doll animation when player is killed. 
  

I also coded a flip-flop mechanic to make an oven turn on and off when the player interacted with it, but this feature didn’t make it to the final project as it didn’t fit with the overall design. 

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-22.png">

Figure 9. [BlueprintUE](https://blueprintue.com/render/v622nwbk/) Flip flop implementation.

At this stage, I received animations and worked on implementing them so that certain animations would trigger when the player interacted with objects, such as pulling or picking them up (Unreal Engine - Ingredient Pickup and Potion Crafting, 2025). This was another key learning point for me, as I had never worked with animations before.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-5.png">
Figure 10.Player animation state machine 


I also added music (Unreal Engine - Sound and Music In 6 Minutes, 2021) and prompt text (How To Display A Prompt Above An Item In-Game - Unreal Engine 4/5 Tutorial, 2022) that appears above interactable objects to make it more intuitive for players, so they would know they could interact with them.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-6.png">

Figure 11. [BlueprintUE](https://blueprintue.com/render/qlxjbqiy/), Interactive prompt implementation.

Afterward, I created a main menu scene (How To Create A Main Menu - Unreal Engine 5 Tutorial, 2022) and later added a pause menu (How To Create A Pause Menu - Unreal Engine 5 Tutorial, 2022) based on user testing feedback, allowing the player to quit the game or adjust the music volume, which was a major concern.This was an easy task to pick up, and I feel more comfortable with UI creation now. 

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-7.png">

Figure 12. [BlueprintUE](https://blueprintue.com/render/jqjmtipm/), Main menu implementation.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-8.png">

Figure 13. [BlueprintUE](https://blueprintue.com/render/k801pugu/), Pause menu implementation. 

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-9.png">

Figure 14. [BlueprintUE](https://blueprintue.com/render/55497dmx/), Pause menu player implementation.This allows the player to press "P" to trigger the pause menu. 

I then moved on to developing an inventory system that allowed the player to pick up items in a specific order to make the potion (Unreal Engine - Ingredient Pickup and Potion Crafting, 2025). When the order was followed correctly, the player would receive a potion from the cauldron.  

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-13.png">

Figure 15. [BlueprintUE](https://blueprintue.com/render/-l14_d_8/) Inventory system for the player to be able to pick up the ingredients.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-14.png">

Figure 16. [BlueprintUE](https://blueprintue.com/render/55ra9vgu/) Cauldron system, checking if the player has the right order of ingredients and giving them a potion or restarting the level if its not working 

Additionally, I implemented a wrong recipe function that respawns the player if they make the potion in the wrong order, allowing them to reset the vegetables. This approach was a simpler solution than respawning the vegetables individually.

I also created a book that the player could pick up to see the recipe (UNREAL ENGINE 5 HOW TO PICKUP AND READ NOTES TUTORIAL, 2023) and understand the correct order, but I later adjusted this so that it would disappear when the player moved away, based on user testing feedback.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-15.png">

Figure 17. [BlueprintUE](https://blueprintue.com/render/ccb8voun/) Pick up and put down when moved away recipe system. 

I then implemented the potion "melting" the vent to allow the player to exit, using a destroy object blueprint. Although I initially planned to create a cutscene for this effect, there wasnt enough time to implement this.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-16.png">
 
Figure 18. [BlueprintUE](https://blueprintue.com/render/qx-ayi8e/) Vent melting implementation.

Toward the end of the project, I worked on cutscenes (How To Make & Trigger A Simple Cutscene | Unreal Engine 5 Tutorial, 2024), which was rewarding as it allowed me to experiment with something new and use my knowledge to add a spawn location afterward.Although this effect stayed in the test level only, I still used the code for the trigger boxes.

 
<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-17.png">

Figure 19. [BlueprintUE](https://blueprintue.com/render/vgzuxgcg/) Cut scene implementation. This was used for all four cut scenes, with the scene just changing for each different one. 

I also added a witch AI system that checks for the player and kills them upon detection, which involved working on animations, particularly for the witch’s grab animation when it kills the player. 

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-18.png">
  
Figure 20. [BlueprintUE](https://blueprintue.com/render/t7ycpu2u/) Witch AI checking for the player location and following them. 

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-19.png">

Figure 21. [BlueprintUE](https://blueprintue.com/render/h7knm8lf/) Witch AI movement if it cant find the player.This is so the witch is still moving around the scene. 

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-20.png">

Figure 22. [BlueprintUE](https://blueprintue.com/render/hn4zai_z/) Witch AI implementation.

<img src="C:\Users\keish\OneDrive\Documents\Games development\Git Projects\Client-brief\image-21.png">

Figure 23. [BlueprintUE](https://blueprintue.com/render/bgmc0lkz/) Witch grabbing animation blueprint, needed for when she kills the player. 

I developed all of these mechanics in a test level to save time and ensure everything was functional before receiving the final assets and level design. This approach made it easier to complete the project quickly, as I only had to change the static meshes of the objects when the level design was finished.  


As mentioned earlier, I used a Figma board (Figma, s.d.) to organize the game mechanics and keep track of what I had completed and what was still pending. This helped me avoid forgetting any important mechanics of the game. Additionally, I followed YouTube tutorials for these mechanics, which allowed me to see the blueprints and have them broken down and explained. This was extremely helpful in learning how to implement the mechanics effectively, and it also enabled me to add clear comments in the blueprints for other team members to read or use in future projects.


### New Approaches  (141)
I had to explore how to implement animations and create blueprints for them. To better organize my approach, I learned to use Figma boards (Figma, s.d.), which allowed me to condense my group's ideas and determine which parts needed to be developed and which were unnecessary. By breaking everything down, I was able to pinpoint the documentation I needed and tackle tasks step by step, ensuring each was completed to a high standard. I also highlighted areas that needed more attention or less time, helping me stay on track without feeling overwhelmed. Creating a Figma board (Figma, s.d.) gave me a clear visual of my tasks, allowing me to stay focused and avoid falling behind. Although the animations and blueprints were challenging at first, with practice, I began to understand them more, though I still needed more practice to master them.

### Testing (205)
For user testing, I used a blind approach by uploading the project to Itch and asking people to playtest it. I linked a Google form with questions to gather feedback. During testing, several issues were identified, such as the music being too loud, so I added a pause menu that allowed the player to adjust the volume and exit the game(How To Create A Pause Menu - Unreal Engine 5 Tutorial, 2022). Players were also having trouble with the recipe not disappearing unless they were near it, so I changed it so the recipe would disappear when the player walked away (UNREAL ENGINE 5 HOW TO PICK UP AND READ NOTES TUTORIAL, 2023). Additionally, I made the recipe order clearer, as some players were unsure if they needed to pick up the ingredients in a specific order. They also found that the AI seemed too similar to the player, but that was due to it not being fully implemented. It has since been changed to a witch. One player mentioned they didn’t know how to interact with the cauldron, so I added a prompt to the cauldron to resolve this (How To Display A Prompt Above An Item In-Game - Unreal Engine 4/5 Tutorial, 2022).

### Technical Difficulties (168)
Throughout this project, I encountered several small difficulties during playtesting. These issues included the player’s jump being too high, the box flying when pulled, and the menu preventing the player from moving once they entered the level. To resolve these problems, I adjusted the jumping velocity for the player (How can I change a character's jump height in blueprints? - Development / Character & Animation, 2017), fixed the axis on the box, and modified the force applied when the player pulled the object. Additionally, I changed the node for the UI from game to UI, allowing the player to move freely within the level. I also had to uncheck a collision box on the camera to stop it from following the player and making the player get stuck. 

In the future, I would make sure to pay more attention to the blueprints to avoid any slight mistakes and I would also make sure that the physics on objects works correctly rather than leaving it to the last minute. 
 
## Outcomes (Suggested Word Count 300) 

### Source Code/Project Files

[Git Hub reposistory](https://github.com/kdogz9/Client-brief)

### Build Link

[Itch build](https://starcreations.itch.io/witcheskitchen)

### Video Demonstration
[Youtube link](https://youtu.be/z5Mx8waMXi4)

Figure 24. A youtube link which showcases the player picking up the ingredients to make a potion and using it to escape via the vent. It also shows the witch AI and the cut scenes that have been made to improve the narrative of the game and make it feel more immersive. 


## Reflection (Suggested Word Count 500) 

### Research Effectiveness  (150)
Researching *Little Nightmares* provided valuable insight into common game mechanics, which I could incorporate into my project. It helped me understand key elements like camera angles and environmental design, as well as influenced the types of puzzles I implemented, such as pulling boxes and collecting items (Unreal Engine - Ingredient Pickup and Potion Crafting, 2025). It also influenced the type of AI we used and how they killed the player by grabbing them with their hand out like how a monster does in little nightmares. Academic sources further guided the animation process (Clark, s.d.), particularly the use of ragdoll physics when the player is killed, creating a unique outcome each time. However, I believe that diving deeper into puzzle design could have added more depth to the game. Additionally, exploring more academic sources related to coding and game theory might have enriched my understanding and implementation of the game's mechanics.

### Positive Analysis (152)
The successful parts of the project included staying on track, completing the mechanics quickly, and ensuring everything worked within a reasonable time frame. I worked hard on the project and explored learning through YouTube tutorials and documentation, which helped me understand the concepts I was learning. As a result, I felt more comfortable with blueprints and was able to resolve issues, such as the box problem mentioned earlier. Additionally, I used my problem-solving skills to tailor the tutorials more specifically to my game. Over time, I became more confident and began working on blueprints independently. 

I feel like I have answered the question quite effectively within the animations and how I went about implementing them in order to make the game space feel more immersive. This helped add different outcomes each time and draw different emotions out from the players each time as the players could have a different outcome each time. 


### Negative Analysis (199) 
Several areas of the project didn’t go as planned. I encountered an issue with not having the level design until week 9, which put a strain on me as I had to fix errors that cropped up later. I also struggled to divide my attention between the write-up and the project itself. Learning animations and how to implement them proved to be another challenge. Additionally, I had to make adjustments to the level when implementing the blueprints to ensure they worked properly at the new level, which led to small delays. I didn’t manage to user test my game until week 9, and it wasn’t fully complete due to missing aspects from my group partners. Through this experience, I’ve learned that I need to take on more of a leadership role to ensure everyone completes their tasks on time, giving me enough time for user testing and addressing any minor issues without the pressure of time constraints.

I feel like I have answered the question effectively, but also I could've paid more attention to the effect of the environment as well as animations to fit my role a bit more and to make my games a bit more effective.

### Next Time (118)
If I were to do a similar project again, I would plan everything out using Figma (Figma, s.d.), as it helped me stay on track throughout the process. I would also look at different academic sources for coding or development as well as animations so I could broaden my knowledge. Additionally, I would make use of more documentation sources beyond just YouTube tutorials to extend my knowledge and avoid getting stuck in a comfort zone.

I would probably use Trello (Trello, s.d.) next time round as it would help organise and delegate tasks to all of the different members in the group. This would make sure everyone sticks to the deadlines and I have the content in time.

## Bibliography  
A destroy actor and respawn tutorial. (2022) At: https://www.youtube.com/watch?v=Z_3B_EKSCDY (Accessed  29/03/2025).

How can I change a character's jump height in blueprints? - Development / Character & Animation (2017) At: https://forums.unrealengine.com/t/how-can-i-change-a-characters-jump-height-in-blueprints/283857/6 (Accessed  01/04/2025).

 How To Attach A Weapon To The Player | Give The Player A Weapon - Unreal Engine Tutorial (2021) At: https://www.youtube.com/watch?v=mSCPg3d5Kgg (Accessed  29/03/2025).

How To Create A Main Menu - Unreal Engine 5 Tutorial (2022) At: https://www.youtube.com/watch?v=kumZj_mov58 (Accessed  29/03/2025).

How To Create A Pause Menu - Unreal Engine 5 Tutorial (2022) At: https://www.youtube.com/watch?v=voIMzFOQEOs (Accessed  06/04/2025).

 How To Display A Prompt Above An Item In-Game - Unreal Engine 4/5 Tutorial (2022) At: https://www.youtube.com/watch?v=tob3GEdMJFc (Accessed  29/03/2025).

 How To Make & Trigger A Simple Cutscene | Unreal Engine 5 Tutorial (2024) At: https://www.youtube.com/watch?v=AXGcKi66ENc (Accessed  29/03/2025).

 How To Make Items Fall When The Player Enters A Zone Unreal Engine 5 - Google Search (s.d.) At: https://www.google.com/search?q=how+to+make+items+fall+when+the+player+enters+a+zone+unreal+engine+5&rlz=1C1GCEA_enGB1152GB1152&oq=ho&gs_lcrp=EgZjaHJvbWUqBggBEEUYOzIGCAAQRRg7MgYIARBFGDsyCAgCEEUYJxg7MgYIAxBFGDkyDQgEEAAYkQIYgAQYigUyBggFEEUYPDIGCAYQRRg8MgYIBxBFGDzSAQgzNDU2ajBqN6gCALACAA&sourceid=chrome&ie=UTF-8 (Accessed  29/03/2025).

 How To Pick Up And Drop Items | Hold Items In Hand - Unreal Engine Tutorial (2021) At: https://www.youtube.com/watch?v=EbZrfsJ1fWc (Accessed  29/03/2025).

 Unreal Engine - Ingredient Pickup and Potion Crafting (2025) At: https://www.youtube.com/watch?v=-hOStF6TkHQ (Accessed  29/03/2025).

 Unreal Engine - Side Scroller Camera Tutorial (2023) At: https://www.youtube.com/watch?v=659FjVeibv0 (Accessed  26/03/2025).

 Unreal Engine - Sound and Music In 6 Minutes (2021) At: https://www.youtube.com/watch?v=1GJRoUJvijw (Accessed  29/03/2025).

 UNREAL ENGINE 5 HOW TO PICKUP AND READ NOTES TUTORIAL (2023) At: https://www.youtube.com/watch?v=719PxAugimo (Accessed  29/03/2025).

 How To Use Trigger Box - Unreal Engine 5 Tutorial (2024) At: https://www.youtube.com/watch?v=SB9-NmFrY78 (Accessed  29/03/2025).
 

## Declared Assets

AmaticSC/fonts/ttf/AmaticSC-Regular.ttf at main · googlefonts/AmaticSC (s.d.) At: https://github.com/googlefonts/AmaticSC/blob/main/fonts/ttf/AmaticSC-Regular.ttf (Accessed  01/04/2025).
 
 This was used for the font of the UI and interaction text.

ChatGPT (s.d.) At: https://openai.com/index/chatgpt/

This was used to help write up this document and proof check it all.
<br>