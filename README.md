# KitchenBot

KitchenBot is a dedicated helper for the kitchen. WIP, but the features we are planning are:
 - [ ] Conversational interface
 - [ ] Manage kitchen inventory
 - [ ] Manage favourite recipes
 - [ ] Manage shopping list
 - [ ] Telegram integration


## Inventory management ideas

 - When you get back from a grocery run, you can wake up the bot and list the items as you unpack them. 
   As you cook, you can ask the bot to update your inventory with what you used. The bot will then keep track of how much is left in stock.

 - Another option: look at the receipt and infer it from that, with possibly some user questioning? Also: try to directly recognize from video
   feed, although it might be challenging.

 - Some items are easy to track: "I used 2 eggs", while others are a bit more cumbersome (oil, salt, coffee are painful to weight every time);
   for the latter items, the bot will ask you periodically how much is left. Ideally at some point the shopping behaviours can be
   learned, and the info like "a bottle of olive oil lasts X weeks" can be made available to KitchenBot.

 - Food items are typically nonfungible; if I buy some bread today, while I had some leftover bread from 5 days ago, I don't just have "200g of bread", 
   but rather "100g of bread from yesterday and 100g of bread from 5 days ago". This should be reflected in the database schema.

 - KitchenBot should track food wastage as well; maybe via "thrown away on" and "thrown away reason" fields?

 - Some items have an expiry explicitly written on the package.

 - Errors are inevitable; there should be some way to fix them.