this repo was made for one sole purpose:
  patch notes in my roblox games.
  it sounds silly, but it's a great system to synchronize the patchnotes of all your experiences!

Q: how does it work?
  A: i have created a custom discord bot, which reads when a game's placeid is mentioned in the #changelogs channel of my discord server,
  the bot then adds the new patch notes converted from markdown to rich text (so it can be properly displayed in a roblox textlabel, with bold, italic, headers, and lists) to the game's patch notes file in this repo.
  from there, i read the repo's raw file with an http request on roblox, and send that info to the client to display past and current patch notes forever!

Q: why not just upload your patch notes here, and then have the discord bot publish the notes in your discord?
  A: to be honest? its because i didn't think of doing that first 😭. but, doing it this way does have some pros,
  like how my friends/co-workers who don't know how to use git or are on mobile a lot can easily publish patch notes anywhere at anytime,
  and that i can just get the bot to format it to rich text and then publish that to github, rather than having to convert twice so that both roblox and discord could read the patch notes as intended.
  overall, if i were to do something like this again or rewrite the bot, i would definitely just upload the notes here, and then have them read by http requests and a discord bot instead of uploading to discord first.
