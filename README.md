# iTheon-PDA-Taskboard v0.1.14

This mod adds a new taskboard tab to the PDA where you can accept all the dynamic tasks remotely

How to use it? <br>
On Taskboard tab there's a Refresh tasks button - click it once and wait for the tasks to be processed (time depends on the population density in radius, but is pretty fast). <br>
You'll get a list of tasks split into categories. Next to the task description you will see two buttons - these require double click for some reason (I'll work on changing that). Accept task - self-explanatory - accepting a task automatically refreshes the board, as some tasks automatically remove others from the available list (vanilla Anomaly stuff). Next task - tells PDA to prepare info about the next task in category.

To dos: <br>
fix double click required for Accept task and Next task buttons - no idea where it comes from for now


Possible questions: <br>
Q: Why you didn't make one full board of tasks? <br>
A: Engine limitation. I've tried doing it in several different ways, but there needs to be a delay between fetching detailed info about tasks of similar type. With no delay, specific info about the task (e. g. target name and location) will not load properly. You could accept such a task, but you wouldn't know who exactly you have to kill and where he is before you accept it. With full list - even when I've set certain delays to 10 seconds - it sometimes happened anyway. With split list, there doesn't need to be any delay.

Credits:<br>
Mr. Demonized - optimized time events script<br>
https://github.com/IIJTypmaH - Russian translation<br>
https://github.com/Igigog - WTF support

Changelog:

v0.1.14
- Add taskboard keybinding
- Change order of the tabs (place taskboard next to map)

v0.1.13

- Exclude Gavrilenko from the list of processed npcs

v0.1.12a

- Add missing xml file

v0.1.12

- Add a separate PDA tab for taskboard

v0.1.11

- Exclude Outskirts merc mechanic tools task from the list of available tasks (it's impossible to take normally and can't be finished)
- Adjust the task description fetching code - now the descriptions of the fetch tasks look exactly like they do in the dialog window

v0.1.10

- Exclude Yar's CoC task from the list of available tasks

v0.1.9

- Add WTF support by Igi

v0.1.8

- Add options to disable text trimming and increase the task row height

v0.1.7

- Speculative fix for rare bug with messed up details pairing (as a side effect the task categories will now always be rendered in a sorted order)

v0.1.6

- Fix accepting quests that assign you a temporary companion

v0.1.5

- Increase maximum number of simultaneously rendered task categories
- Expose normalizer table for other mods

v0.1.4

- Add conditional shortening of the task description and details

v0.1.3

- Fix weird bugs caused by refreshing board when there was a task without details on it

v0.1.2a

- Fix task giver override not getting cleared after processing fetch tasks

v0.1.2

- Add Mr. Demonized's "optimized time events" script as an integral part of the addon (required for vanilla Anomaly)

v0.1.1

- Fix Sidor and Forester distance evaluation<br>
- Introduce delay for refreshing the tasks<br>
- Visual tweaks<br>
- Add mcm config
