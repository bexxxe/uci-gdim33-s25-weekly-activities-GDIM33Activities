# GDIM 33 In-Class Activities
## W1
### Activity 1
https://docs.google.com/drawings/d/1OjKFC-45Vjxww_mOeZDNmFHeWapBdBEBz_H8RkfJXjQ/edit?usp=sharing)

1. I found the cluttered, busy, and hoarder vibe popping up a lot. I love lots of layers and lots of things to look at. I really enjoyed the fun colors and details of everything on my board. I have been playing cozy/indie pixel-art-esque games, especially games with striking lighting like Eastward (despite being pixel art). The games are from different genres, so it's hard to group them other than by visuals.  
2. I chatted with two table members, one was gambling, money, dopamine vibe. The other was low-poly retro games with saturated colors and a sense of nostalgia. I think the busyness of the gambling core is very similar to the dense, filled vibe I had.
3. Elijah said that he is into story-heavy games as well as being into puzzle games lately. I also really enjoy story-heavy games espcially lore games that make you think.


### Activity 2
https://docs.google.com/drawings/d/1z7B0QOzfWqonLkrC7Ff_KNYUN0jdluheUiCFFZj9QEc/edit?usp=sharing)


## W3
(https://docs.google.com/drawings/d/1z7B0QOzfWqonLkrC7Ff_KNYUN0jdluheUiCFFZj9QEc/edit?usp=sharing)

1. Saving the event name is useful because we can call on it again in future graphs across GameObjects.
2. I used the Debug log on the Walrus click to see if the click triggered. It's hard to tell whether the nodes work for something other than movement, so seeing a response in the console is helpful.
3. I think the Set Cursor lock could be relevant when chatting with the NPCs, but my game is also stationary, so I'm unsure how much value that would add.
4. Yes, Game State would be helpful for the NPCs; they would need to walk into frame and stop to have a conversation with the player.

## W4
Playtest

1. In my game, the shop inventory UI is done. There is one customer who comes up and asks for what they want, but I have not put in what happens when they get the item. You can drag things in and out of inventory and put them on the counter in front of the customer. My main goal is for the layout to be intuitive enough that people can tell what to do and for the customer prompt to be readable.
2. My playtest members are: Andrew Xu, Pinhsuan Wang, Sonia

Devlog
1. A writer could add more dialogue without writing more code because everything is in Unity, and you can add lines without writing more code.
2. There is no Limit.
3. The purpose of the regenerate Node Button is to reload the node so that any new nodes that were added can get put in, including C# scripts that were added.

## W5
Activity 1: Breakdown
Im choosing to add scriptable objects to my game for the items. So that when the customer asks for something, the dialogue will be in the objects.
Big Steps:
1. Create the Scriptable Object and test that data can be read and stored.
Then
2. Connect the Scriptable Object to the items and the mat so that the correct dialogue triggers based on the item.

Detailed Steps

Step 1:

1. Create an ItemData script that has fields for item name, item sprite, correct dialogue, and wrong dialogue. Then I save and check whether it worked and whether there are any errors in the console.
2. Create one ItemDate asset in the project window using the Create menu. Fill in the fields in the inspector, check that everything is going ok, and save.
3. Add a public ItemData Field to the object script that is already there. Then, start by adding debug.log to print the item name and check whether it has the correct name in the console.
   
Step 2:

1. Add a public field to the mat where the item will sit, then assign it to one of the items in the inspector. Test by adding a debug.log to confirm when the item is dropped.
2. Replace the compare tag in one of the scripts to check into the item drop with a comparison between the dropped items' data and the public on the mat. Add a debug.log to see if the item is correct. dropping the correct item should print "true," and another should print "false".
3. Add right and wrong dialogues into the values and run the game, drop the item, and see if it's working.

Activity 2:
I built a state machine for the items in the inventory and assigned tags to them. Having fields like Item name, correct dialogue, wrong dialogue, and item sprite. I only did this one item because I only have one customer so far. I tested at each stage. I also plan on adding a Scriptable Object for characters.

## W6
Playtest:

What's new: I made all the items and the NPC scriptable objects and added an end-of-day panel that shows how much money the player made. Before, I was using tags on the items, but I transitioned; it isn't really a noticeable feature at the front, but there was a change.

Game link: https://becxah.itch.io/racoon-pawn-shop

Goal: Just for everything to work, and hopefully, the game is intuitive enough. All the items have their own dialogue response and money value. There is only one sprite so far, so hopefully it will be more noticeable later. I hope that the player will finish out the day.

Playtesting Notes: I was using the trackpad, so the hold-and-drag controls weren't very intuitive. Said that they liked the dialogue and that it was cool. They also liked that the item hover indicated that the pointer is over the item. Said it would be cool if I added an interaction when the user clicks the dog.

Activity Questions: 

1. The Multiply setting doubles the values; the colors are from 0 to 1, so if the first color is 0.3 and the second color is 0.1, then the output will be darker because multiplying 2 decimals makes it smaller, making it darker and less saturated because it combines them.

2. It will get more translucent because its alpha is multiplied by alpha, doubling the alpha value, making it more translucent.

3. It's in the vertex data of the UV mesh on the shiba/game object.

4. Math and colors don't sound that appealing to me.

## W7

Devlog Questions:
1. The data for the Vertex Color node comes from the Shiba Mesh.
2. It's blended at the edges because each vertex has a color, and going between the vertices, they have different colors, so they become interpolated when they reach out to each other.
3. We are using a vertex from a mesh, which is less detailed than a texture. This is helpful because it helps artists notice discrepancies or mistakes in the mesh.
4. In the back leg of the Shiba, there is a discrepancy in colors compared to the colors around it. 
5. UV map because it will give us all the colors applied to the mesh.
6. The surface of the leg isn't perpendicular to the surface.
7. It's additive because it adds color, making it more opaque for the brighter parts.

## W8
Playtest:

What's New: I added some new art, like the background, and did some UI work. It was wonky last time, so I aligned them better and also fixed my layers. Just some smoothing of the game and a visual upgrade; also fixed some timeline issues.

Playtest Link: https://becxah.itch.io/rps-playtest

Goal: For everything to still work and for the new dialogue and characters to be understood. I Im a little concerned that the dialogue might be hard to understand, but I hope people get the game's goal. I hope that all the mech still work.

Playtest Notes: There is a bug (this wasn't there before) where multiple objects can be placed on the mat, and even if it was the wrong item, the NPC would take it away. People didn't really know how to give NPC items, so I suggested adding a highlight over where I needed to place the item, aka the mat. Some of the dialogue was confusing to players, and some tried every item before giving the right one. A lot of people don't know that nectar is a liquid. Someone also suggested that the player should lose money if they got it wrong, for some stakes. Also, a cutscene was suggested to give context.

Activity Questions:
1. The value of the Time node keeps increasing. The result of taking a time gives us a decimal value that cycles between 0.0 and 0.99. So we get a looping animation that moves the texture from its normal UV sample to the maximum-displaced sample.

2. It needs to be black because black acts as a transparent, and does not alter the base sprite texture, unsure.
   
3. It's because of the name that we gave it, it's named MainTex and only uses the texture that was assigned to the og item.
   
6. Multiplying time by speed inside the function speeds up the cycle's frequency, making the effect move faster, otherwise it wouldnt change speed.

## W9
Brainstorming:

Game: Ori and the Blind Forest/ Ori and the Will of the Wisps

Brainstorm: There were lots of different types of shaders in the game, including interactive foliage and full-screen distortion, like fog or mist. For foliage manipulation, you would need to bend it using geometry and a player proxy so that the player can interact with the environment around them. For the Fog and mist, it would need to be a full-screen post-processing effect that warps the UV and uses a volume component that can be triggered both in gameplay and out of play.

ShaderGraph:
<img width="1212" height="797" alt="image" src="https://github.com/user-attachments/assets/17c45556-2367-4259-992b-d37f6cdba263" />
I Im trying to make a glow effect for one of the objects, but it was only glowing in the scene, not in the game. I needed to install Post Processing in my Unity packages, tick a box on my camera to enable post-processing, and create a global volume for bloom.

## W10
Playtest:

What's New: I mainly made some quality-of-life changes and bug fixes so that everything runs more smoothly. I changed the dialogue of one of the characters to hopefully make it clearer. I also fixed the mat and how people could place multiple items there.

Platest link: https://becxah.itch.io/rps-playtest

Goal: For the item, the 2nd NPC wants to be clearer so people know what they want. Also, hopefully, no more bugs with items and placing.

Playtesting Notes: There aren't any bugs when placing items anymore, but players are still struggling with where to put them, so I really need to fix that. My game is dialogue-dependent, so it's hard for non-English speakers to understand some words. I think adding color descriptions helps a bit with narrowing down the options.

Devlog:
Strategy: Think about the genre of game to make, and think about what the key points of it are. Think about the key mechanisms and the most important part of them. Planning everything on paper helps write down ideas and breaks down the planning process. Start with the easiest and most fun mechanism to motivate starting the game-making process. Break down those big mechanics into smaller bubbles to help identify what each needs. Playtest and fill in holes that stunt the game experience.

Narrow down your goal if it seems unrealistic or if you don't think you can complete it. Generally, after the first build, you will narrow down your window and know what you are and aren't capable of. Usually, people shoot beyond what is possible, so being flexible is a plus.


