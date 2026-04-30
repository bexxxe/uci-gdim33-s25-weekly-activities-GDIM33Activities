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
