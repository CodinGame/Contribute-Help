[Coders Strike Back](https://www.codingame.com/multiplayer/bot-programming/coders-strike-back) is CodinGame's official tutorial for bot programming. It will show you how submissions, leagues and bosses work.

For a more detailed guide on getting started with bot programming, check out the [Ghost in the Cell guide](pages/bot-programming/gitc.md)

Coders Strike Back is a game where you control one racing pod (then 2). Your goal is to finish the race first by passing through the multiple checkpoints of the track. You control the direction (x and y coordinates) and the thrust (an integer between 0 and 100) of your pod.

## Boost

After reaching the Bronze league, you unlock the ability to boost. It's an action that will boost the speed of your pod, _usable only once per game_.

To use this action, you only have to replace the thrust value by the keyword `BOOST` in your output. Example:
"3000 2000 BOOST"

## Controlling 2 Pods

From the Gold league, you control another pod. To handle this, the game protocol changes and you have more inputs to read. This is one of the very few games where the protocol changes from one league to another.

Check the updated protocol at the bottom of the statement or reset your code to see the changes.