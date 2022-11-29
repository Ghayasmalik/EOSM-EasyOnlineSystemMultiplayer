# EOSM-EasyOnlineSystemMultiplayer

EOSM is small yet easily modifiable template. Purpose of this template/Boiler Plate is to provide any
developer good starting point and easy to modify code to their needs. Having to right all new code
again and again lead to problem and time it take to right code that should be basic need of game.
This pack include the Basic Online System where you can login to the Epic service (only epic for now).

I have made widget system that use level name to get and set all the widgets so all the widget can be
maintain in one place and called automatically.

Note: This is my way of doing thing and all blueprint are independent so widget and online system can
be delete or use separately.

Basic needs:
 You will need epic games account.
 Must be Logged in to Epic Online Service and set up product in there.
 Active internet connection.
 Advanced Sessions Plugin (open source on GitHub).
 EOS Plugin to be enable(All plugin with EOS name).
 Replicated Graph Plugin to be Enable (For bulk data to be formatted in graph and easy
to handle packages. Good for big player base games).
 Fill out eos Details in Plugin panal.

All the Logic is in Game Instance Blueprint “GI_EOSM” that control the online system and All
the Game UI/HUD is control from the Widget “Main_HUD”.

Advance sessions plugin is must to have so C++ can be skipped and only blueprints can be use.
It provide with many great new function that can be use with stream too.

#GI_EOSM:

This blueprint is baseline of all the online system and is alive as long as the game/instance is
running. So your login details and all the online system is available to you in any blueprint in
editor.

#Main_HUD:
This Blueprint Control all the widget that are been shown on the screen at any given time of
game/instance lifecycle. This use name and number system where level name verify and then Branch
node is use to select the correct widget to show. This provide one place to handle all the ui things now
new level can be added and only update is going to be to add that last level name in branch node in last
of all branches and it will work as intended.
