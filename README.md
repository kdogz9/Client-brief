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
- Research academic papers, books, or articles that provide theoretical guidance for your project. Include a brief summary of each source.  
- Describe how the academic research applies to your project and shapes your design and development decisions.

### Documentation Sources  
I used in-depth YouTube tutorials to create the game mechanics our group had discussed. I utilized UI tutorials to develop a game menu and animation videos to implement character actions, such as crouching. Additionally, I followed tutorials for creating an interactive system, allowing objects to be moved and hobs to be turned on and off. I also learned how to implement a potion mechanic through another video, and used Unreal Engine in conjunction with these tutorials. By adapting the techniques shown in these videos, I was able to tailor them to meet the specific needs of our project.

- talk about camera video (Unreal Engine - Side Scroller Camera Tutorial, 2023).

## Implementation (Suggested Word Count 1,100)  

### Process
- Provide a step-by-step breakdown of your development process, including key milestones and decisions made throughout the project.  
- Highlight any tools, frameworks, or techniques used, and explain how they contributed to the implementation.  
- Include screenshots, diagrams, or code snippets where relevant to showcase your progress.

### New Approaches  
I had to explore how to implement animations and create the blueprints for them. To better organize my approach, I learned to use Figma boards, which allowed me to condense my group's ideas and determine which parts needed to be developed and which were unnecessary. By breaking everything down, I was able to pinpoint the documentation I needed and tackle tasks step by step, ensuring each was completed to a high standard. I also highlighted areas that needed more attention or less time, helping me stay on track without feeling overwhelmed. Creating a Figma board gave me a clear visual of my tasks, allowing me to stay focused and avoid falling behind. Although the animations and blueprints were challenging at first, with practice, I began to understand them more, though I still need more practice to master them.

### Testing
- Document the user testing conducted, specifying the type of tests used (e.g., automated testing, guided user testing, blind testing).  
- Present feedback or issues identified during testing, using graphs, tables, or visual aids to summarise results.  
- Describe how these issues were addressed. If any issues were not resolved, provide a clear justification for leaving them unaddressed.

### Technical Difficulties
Throughout this project, I encountered several small difficulties during playtesting. These issues included the player’s jump being too high, the box flying when pulled, and the menu preventing the player from moving once they entered the level. To resolve these problems, I adjusted the jumping velocity for the player, fixed the axis on the box, and modified the force applied when the player pulled the object. Additionally, I changed the node for the UI from game to UI, allowing the player to move freely within the level.I also had to uncheck a colision box on the camera to stop it from following the player and making the player get stuck. 

In the future, I would make sure to pay more attemtion to the blueprints to advoid any slight mistakes and I would also make sure that the physics on objects works correctly rather than leaving it to the last minute. 


- If any difficulties remain unresolved, explain the impact on the project and any mitigation strategies used to minimise their effect.  


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
- Assess the usefulness of the research conducted during the project.  
- Highlight which sources (games, academic, documentation) had the most significant impact on your work and explain why.  
- Identify any research gaps or areas where additional information could have improved your project outcomes.

### Positive Analysis 
- Reflect on the successful aspects of the project.  
- Highlight specific elements that worked well, such as technical solutions, creative decisions, or user feedback.  
- Provide evidence to support your analysis, such as test results, screenshots, or user comments.

### Negative Analysis  
- Identify the areas of the project that did not go as planned or could have been improved.  
- Discuss challenges you faced, whether technical, creative, or time-related, and evaluate their impact on the final product.  
- Reflect on any mistakes or missteps and what you learned from them.

### Next Time
- Outline what you would do differently if you were to undertake a similar project again.  
- Suggest improvements to your workflow, research methods, or implementation process based on your reflections.  
- Consider any new tools, techniques, or approaches you would explore in future projects to achieve better results.

## Bibliography  

Unreal Engine - Side Scroller Camera Tutorial (2023) At: https://www.youtube.com/watch?v=659FjVeibv0 (Accessed  26/03/2025).

A destroy actor and respawn tutorial. (2022) At: https://www.youtube.com/watch?v=Z_3B_EKSCDY (Accessed  29/03/2025).
 
 How To Pick Up And Drop Items | Hold Items In Hand - Unreal Engine Tutorial (2021) At: https://www.youtube.com/watch?v=EbZrfsJ1fWc (Accessed  29/03/2025).

How To Attach A Weapon To The Player | Give The Player A Weapon - Unreal Engine Tutorial (2021) At: https://www.youtube.com/watch?v=mSCPg3d5Kgg (Accessed  29/03/2025).

Unreal Engine - Ingredient Pickup and Potion Crafting (2025) At: https://www.youtube.com/watch?v=-hOStF6TkHQ (Accessed  29/03/2025).
 
 How To Create A Main Menu - Unreal Engine 5 Tutorial (2022) At: https://www.youtube.com/watch?v=kumZj_mov58 (Accessed  29/03/2025).

UNREAL ENGINE 5 HOW TO PICKUP AND READ NOTES TUTORIAL (2023) At: https://www.youtube.com/watch?v=719PxAugimo (Accessed  29/03/2025).

How To Display A Prompt Above An Item In-Game - Unreal Engine 4/5 Tutorial (2022) At: https://www.youtube.com/watch?v=tob3GEdMJFc (Accessed  29/03/2025).

Unreal Engine - Sound and Music In 6 Minutes (2021) At: https://www.youtube.com/watch?v=1GJRoUJvijw (Accessed  29/03/2025).

How To Use Trigger Box - Unreal Engine 5 Tutorial (2024) At: https://www.youtube.com/watch?v=SB9-NmFrY78 (Accessed  29/03/2025).
 
 how to make items fall when the player enters a zone unreal engine 5 - Google Search (s.d.) At: https://www.google.com/search?q=how+to+make+items+fall+when+the+player+enters+a+zone+unreal+engine+5&rlz=1C1GCEA_enGB1152GB1152&oq=ho&gs_lcrp=EgZjaHJvbWUqBggBEEUYOzIGCAAQRRg7MgYIARBFGDsyCAgCEEUYJxg7MgYIAxBFGDkyDQgEEAAYkQIYgAQYigUyBggFEEUYPDIGCAYQRRg8MgYIBxBFGDzSAQgzNDU2ajBqN6gCALACAA&sourceid=chrome&ie=UTF-8 (Accessed  29/03/2025).

How To Make & Trigger A Simple Cutscene | Unreal Engine 5 Tutorial (2024) At: https://www.youtube.com/watch?v=AXGcKi66ENc (Accessed  29/03/2025).
 
- Compile a complete list of all sources referenced throughout your project. This may include articles, journals, videos, games, software, documentation, or any other materials.  
- Ensure all references are formatted according to the [university's citation method](https://mylibrary.uca.ac.uk/referencing).  
- Organise your references in alphabetical order. Alternatively, you may separate them by type (e.g., academic sources, games, videos), but consistency is key.

## Declared Assets
- Provide a detailed list of any third-party assets used in the project.  
- This includes asset packs, music, sound effects, 3D models, textures, scripts, or code from external sources.  
- Declare any use of AI tools (e.g., ChatGPT, GitHub Copilot, Meshy) or pre-existing code. Specify the purpose of these assets/tools and how they were integrated into your work.  
- Ensure you clearly distinguish between your original work and any external contributions to maintain academic integrity.

<br>