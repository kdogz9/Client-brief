# Development Commentary Template 

## Brief 

 How does the design of video game space affect the actions and experiences of players? Consider how different game spaces have been categorised in the literature and concepts of space and place discussed in the lecture.  


## Project Outline  

The project we are making is heavily inspired by little nightmares as Super massive games is our client brief for this project. We came up with a game idea where the player is trapped in a witches kitchen and they need to do a bunch of different puzzles to escape from the witch.These puzzles involve making potions, pulling boxes to be able to jump on surfaces and avoiding objects that are falling. 

I found the beginning quite slow but I enjoyed making a Figma board and breaking down each task I needed to do so that I could stay on track and understand what needed to be done for the game. I also enjoyed making a moodboard of little nightmares and exploring images related to this game and also images for our own theme of a witch kitchen. 

I think I may run into some issues with working with the animations as I have never worked with animations before but with the right documentation I think I should be able to overcome this challenge and end up understanding implementing animations a bit better. 

## Research (Suggested Word Count 1,100) 

### Methodology  


I copied the game mechnaics that was discussed from the second week of the project and broke it down into simple mechanics so I knew what I needed to code. This made it easier to find what code I needed to implement throughout the project. I then highlighted each mechanic so I knew what needed to be done and what I had finished so I could keep on track. Breaking down the mechanics also helped me find the correct documentation I needed to be able to get help with for the project. 

<img src="Client brief.png">
Figure 1. Figma Jam Board, Mechanic Breakdown.

### Game Sources  
Little Nightmares is a puzzle-based game where players control a small character navigating through a mysterious building filled with monstrous creatures. The goal is to escape the building without being caught. The environment is dark and atmospheric, relying heavily on the use of light and shadows to create tension. This approach has influenced our design, where we've intentionally crafted a dark environment with minimal light sources. Additionally, our character’s color scheme is designed to stand out in the shadowy surroundings, much like in Little Nightmares, enhancing their presence in the eerie world. 



### Academic Sources  
I recently read a book called *Animating Real-Time Game Characters*, and one of the chapters discusses how the environment and space influence design elements, particularly when it comes to animation sets. This insight made me realize that focusing on character movement is crucial in defining the space around them. By understanding how a character moves, designers can better shape the environment to complement and enhance those movements.

I also read *3D Character Animation*, which explores how timing can significantly influence a character's emotion and personality. The book emphasizes that animation plays a crucial role in conveying physical presence within a space, as the speed and pacing of movements can alter the context of a situation. 
how player animates effects imersion and

### Documentation Sources  
I used in-depth YouTube tutorials to create the game mechanics our group had discussed. I utilized UI tutorials to develop a game menu (How To Create A Main Menu - Unreal Engine 5 Tutorial, 2022). Additionally, I followed tutorials for creating an interactive system, allowing objects to be picked up (How To Pick Up And Drop Items | Hold Items In Hand - Unreal Engine Tutorial, 2021). I also learned how to implement a potion mechanic through another video (Unreal Engine - Ingredient Pickup and Potion Crafting, 2025). By adapting the techniques shown in these videos, I was able to tailor them to meet the specific needs of our project.I also referenced some documentation sources on the unreal engine website.This was helpful as I was able to see peoples discussions and how they broke down the issues they had and how they were solved. This was a more beneficial way of learning sometimes. (How can I change a characters jump height in blueprints? - Development / Character & Animation, 2017)

## Implementation (Suggested Word Count 1,100)  

### Process 

This concept led me to focus on creating a ragdoll animation for the character when killed, as it allows the player's death to be communicated more dramatically and realistically, changing the emotional tone of the moment and adding to the overall experience.
 
- Provide a step-by-step breakdown of your development process, including key milestones and decisions made throughout the project.  
- Highlight any tools, frameworks, or techniques used, and explain how they contributed to the implementation.  
- Include screenshots, diagrams, or code snippets where relevant to showcase your progress.

### New Approaches  
I had to explore how to implement animations and create the blueprints for them. To better organize my approach, I learned to use Figma boards, which allowed me to condense my group's ideas and determine which parts needed to be developed and which were unnecessary. By breaking everything down, I was able to pinpoint the documentation I needed and tackle tasks step by step, ensuring each was completed to a high standard. I also highlighted areas that needed more attention or less time, helping me stay on track without feeling overwhelmed. Creating a Figma board gave me a clear visual of my tasks, allowing me to stay focused and avoid falling behind. Although the animations and blueprints were challenging at first, with practice, I began to understand them more, though I still need more practice to master them.

### Testing
For user testing, I used a blind approach by uploading the project to itch and asking people to playtest it. I linked a Google form with questions to gather feedback. During testing, several issues were identified, such as the music being too loud, so I added a pause menu that allowed the player to adjust the volume and exit the game. Players were also having trouble with the recipe not disappearing unless they were near it, so I changed it so the recipe would disappear when the player walked away. Additionally, I made the recipe order clearer, as some players were unsure they needed to pick up the ingredients in a specific order. They also found that the AI seemed too similar to the player, but that was due to it not being fully implemented. It has since been changed to a witch. One player mentioned they didn’t know how to interact with the cauldron, so I added a prompt to the cauldron to resolve this.

### Technical Difficulties
Throughout this project, I encountered several small difficulties during playtesting. These issues included the player’s jump being too high, the box flying when pulled, and the menu preventing the player from moving once they entered the level. To resolve these problems, I adjusted the jumping velocity for the player, fixed the axis on the box, and modified the force applied when the player pulled the object. Additionally, I changed the node for the UI from game to UI, allowing the player to move freely within the level.I also had to uncheck a colision box on the camera to stop it from following the player and making the player get stuck. 

In the future, I would make sure to pay more attemtion to the blueprints to advoid any slight mistakes and I would also make sure that the physics on objects works correctly rather than leaving it to the last minute. 
 


## Outcomes (Suggested Word Count 300) 

### Source Code/Project Files
- Provide a link to your complete source code or project files.  
- Ensure the link is publicly accessible or shared with the appropriate permissions.  
- Include a brief description of the files provided, highlighting key components or any instructions required to run the project.

### Build Link
- Share a link to a playable or executable build of your project.  
- Ensure the build is accessible across relevant platforms and is publicly accessible.  
- Include any necessary instructions for running the build, such as system requirements or installation steps.

### Video Demonstration
- Embed a video or provide a link to a recorded demonstration of your project in action.  
- The video should showcase key features, functionality, and any unique elements of your project.  
- Include a brief commentary or text overlay in the video to explain the different aspects of your project as they are shown.

## Reflection (Suggested Word Count 500) 

### Research Effectiveness  

Researching *Little Nightmares* provided valuable insight into common game mechanics, which I could incorporate into my own project. It helped me understand key elements like camera angles and environmental design, as well as influenced the types of puzzles I implemented, such as pulling boxes and collecting items.It also influenced the type of AI we used and how they killed the player by grabbing them with their hand out like how a monster does in little nightmares. Academic sources further guided the animation process, particularly the use of ragdoll physics when the player is killed, creating a unique outcome each time. However, I believe that diving deeper into puzzle design could have added more depth to the game. Additionally, exploring more academic sources related to coding and game theory might have enriched my understanding and implementation of the game's mechanics.

### Positive Analysis 
The successful parts of the project included staying on track, completing the mechanics quickly, and ensuring everything worked within a reasonable time frame. I worked hard on the project and explored learning through YouTube tutorials and documentation, which helped me understand the concepts I was learning. As a result, I felt more comfortable with blueprints and was able to resolve issues, such as the box problem mentioned earlier. Additionally, I used my problem-solving skills to tailor the tutorials more specifically to my game. Over time, I became more confident and began working on blueprints independently. 

I feel like I have answered the question quite effectively within the animations and how I went about implementing them in order to make the game space feel more immesersive. This helped add different outcomes each time and draw different emotions out from the players each time as the players could have a different outcome each time. 

- Provide evidence to support your analysis, such as test results, screenshots, or user comments.

### Negative Analysis  
There were several areas of the project that didn’t go as planned. I encountered an issue with not having the level design until week 9, which put a strain on me as I had to fix errors that cropped up later. I also struggled to divide my attention between the write-up and the project itself. Learning animations and how to implement them proved to be another challenge. Additionally, I had to make adjustments to the level when implementing the blueprints to ensure they worked properly in the new level, which led to small delays. I didn’t manage to user test my game until week 9, and it wasn’t fully complete due to missing aspects from my group partners. Through this experience, I’ve learned that I need to take on more of a leadership role to ensure everyone completes their tasks on time, giving me enough time for user testing and to address any minor issues without the pressure of time constraints.

I feel like I have answered the question effectively, but also I could've paid more attention to the effect of the environment as well as animations to fit my role a bit more and to make my games a bit more effective.

### Next Time
If I were to do a similar project again, I would plan everything out using Figma, as it helped me stay on track throughout the process.I would also look at different academic sources into coding or development as well as animations so I could broaden my knowledge.Additionally, I would make use of more documentation sources beyond just YouTube tutorials to extend my knowledge and avoid getting stuck in a comfort zone.

I would probably use Trello next time round as it would help oragnise and delegate tasks to all of the different memebers in the group. This would make sure everyone sticks to the deadlines and I have the content in time.

## Bibliography  


A destroy actor and respawn tutorial. (2022) At: https://www.youtube.com/watch?v=Z_3B_EKSCDY (Accessed  29/03/2025).

How can I change a character's jump height in blueprints? - Development / Character & Animation (2017) At: https://forums.unrealengine.com/t/how-can-i-change-a-characters-jump-height-in-blueprints/283857/6 (Accessed  01/04/2025).

 How To Attach A Weapon To The Player | Give The Player A Weapon - Unreal Engine Tutorial (2021) At: https://www.youtube.com/watch?v=mSCPg3d5Kgg (Accessed  29/03/2025).

How To Create A Main Menu - Unreal Engine 5 Tutorial (2022) At: https://www.youtube.com/watch?v=kumZj_mov58 (Accessed  29/03/2025).

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
 
- Provide a detailed list of any third-party assets used in the project.  
- This includes asset packs, music, sound effects, 3D models, textures, scripts, or code from external sources.  
- Declare any use of AI tools (e.g., ChatGPT, GitHub Copilot, Meshy) or pre-existing code. Specify the purpose of these assets/tools and how they were integrated into your work.  
- Ensure you clearly distinguish between your original work and any external contributions to maintain academic integrity.

<br>