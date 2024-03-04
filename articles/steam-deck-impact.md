# Steam Deck - What impact for the developers?
## Steam Deck & other PC handhelds - What impacts for game developers?
*??th March 2024*

### Introduction
With all the hype around the current generation of handheld PCs (Steam Deck, Rog Ally, Legion Go, etc...)

### A bit of history & context
The idea of having 

### Developing for Steam Deck & other Handheld PCs

### How many players on Handheld PCs ?

#### Raw numbers

#### Share of the market

### A bit of Methodology - Different ways to estimate Steam Deck stats for your game
Sadly, Steam doesn't provide a way to know precisely how many of your sales are from Steam Deck players. There are still several datas within Steamworks that can be used to throw estimations and that's what we're gonna use in the rest of the article.  
*This part is going to be Steam specific, as that's a bit of a given for these kind of consoles. Also, I'll only Steam Deck as there's no real way to get data on the others unless you've implemented your own analytics to track users' hardware.*

#### Extrapolating from Linux Sales
The number of sales that come from Linux is a known one, and based from that, we can estimate a number from that.    
However it is impossible to know what share of Linux users on your game are indeed Steam Deck users. We've got a steam-wide number for that, but not only the purchase habits of the average Linux user & the average Deck user might be quite different, but also this number will vary on each game depending on how fitting for Steam Deck it is, your controller support, whether it has Deck Verified status, whether your game has native linux build, etc... So, while ~40% of the Linux Sales would be a the 'default' steam-wide users number, a fitting game could be quite above that percentage.  

It's the only method that estimates sales directly but it's also one that has a big part of uncertainty.

#### Hardware Survey
We've talked about the Steam Hardware survey earlier and we can also get that data for the players of our game. Then, there's only to look at the part of "SteamOS Holo".

This is in theory the best way of estimating your share of Steam Deck sales, however it has some caveats.
First, that data is updated only once per month and is quite delayed. So, it won't be useful until a couple months after your launch.
And second, is that you've only got data for a small subset of your game's users (2-3%) within a given hardware survey. This means that if you don't have a very high number of users (thousands)

#### Daily Active Users
The Players page within Steamworks features Steam Deck specific data.

#### Controller Sessions


#### Analyzing those different numbers
The numbers we end up with 

### Case Study - Breakout Survivors
I released [Breakout Survivors](https://store.steampowered.com/app/2468060/Breakout_Survivors/) on November 30th 2023. As the game has very simple graphics, not a lot of UI, full controller support, runs that last up to 30mins max, etc... the game is a great fit for handheld PCs. Prior release, I had several people asking me whether the game would be compatible with Steam Deck, proving me that there was interest for it (to be honest, the game releasing at the same time as the Steam Deck OLED might have helped with that).  
While during development, I couldn't test for the Steam Deck specifically (didn't have one at the time) nor did anything for it specifically, the couple of feedbacks I had were that it was working and didn't worry much about it as I had both native Linux builds and a proper controller support.  
After release, the game got popular enough with Steam Deck users for Valve to pick up the game for a Deck Verified review two weeks after release. First review only had a "playable" status due to some texts being too small but after a quick update to address the issue, it got the Verified status.

Now, let's take a look at the numbers :
- Linux Sales Extrapolation : 4% sales from Linux (85/2108). With a 50% Deck/Linux rate (that I'd consider quite low), that'd give a 2% of sales.
- Hardware Survey : 7.4% owners on Steam Deck (4/54) - Way too low of a sample size to be reliable
- Daily Active Users : 13.8% daily Steam Deck users (8/58) - Sample too low to be very precise
- Controller Sessions (1) : 31% of daily active users using controllers (18/58) with 40% of the sessions being Steam Deck/Controller (985/2467) - 0.4\*0.31 = 12.8% of daily active players (at most) - Sample bit too low to be precise again
- Controller Sessions (2) : 27.2% users played with a controller at least once (541/1992) with 40% of Steam Deck/Controller (985/2467) - 0.4\*0.272 = 10.9% of players (at most)

The quick things we can get from those would be :
- 2-3% of Steam Deck Sales for Breakout Survivors (I consider the 2% number a low guess + other numbers hint for higher)
- Steam Deck users seem to spend a lot more time on my game than other players (due to the huge diff between active users based stats & the high controller sessions)