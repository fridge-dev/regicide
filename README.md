## [Regicide](https://boardgamegeek.com/boardgame/307002/regicide)

This is a co-op game played with a standard deck of cards. Communication is limited; you may not disclose directly or indirectly what you have in your hand (no hinting!). You may remind other players of public knowledge.

## Rules intro

This is meant as a summarized refresher of the rules. If you're not familiar, read the [full rules](https://www.regicidegame.com/site_files/33132/upload_files/RegicideRulesA4.pdf?dl=1).

## Setup

1. Create the **Castle Deck**: `[shuf(jacks), shuf(queens), shuf(kings)]`
1. Reveal the top deck Jack
1. Create the **Tavern Deck**: shuffle A-10 with 0-2 jesters
1. Deal cards to each player up to hand limit

|Players|Jesters|Max Hand Size|
|-|-|-|
|1|0|8|
|2|0|7|
|3|1|6|
|4|2|5|

## Win and Loss Conditions
### The team wins if...
All face cards (Jacks, Queens, Kings) are defeated

### The team loses if...
A team member is not able to dispose enough cards to cover the damage dealt to them by an opposing Jack, Queen, or King

## Play a turn

Play moves player to player in clockwise order. On your turn...

**Step 1. Play card from hand or "yield" (skip directly to step 4)**

* You can't yield if all other players have Yielded on their last turn.
* If you can't play a card or yield, the players lose.
* _Played_ cards do not go to discard pile until enemy is defeated.

**Step 2. Activate suit power (mandatory)**

* ♥️: Heal X. Move X random cards from discard pile to bottom of Tavern Deck.
* ♦️: Draw X. Players collectively draw X cards starting with the current player and moving in clockwise order.
* ♣️: Deal double damage during Step 3.
* ♠️: Shield +X. Add X to the players' cumulative shield for the current enemy.

**Step 3. Deal damage to enemy**

If enemy is defeated...

1. Move enemy to top of Taven Deck (exact kill) or discard pile (overkill).
1. Move all played cards to discard pile.
1. Reveal the next enemy.
1. Current player restarts a new turn.

**Step 4. Enemy deals damage**

* Enemy damage = Enemy base damage - players' shield
* The current player discards cards with total value >= enemy damage. If current player can't discard cards to cover the damage, the players lose.

## Card Play

### Suit Powers

* ♥️: Heal X. Move X random cards from discard pile to bottom of Tavern Deck.
    * Random cards are chosen by blindly shuffling the discard pile and choosing from the top.
    * Combo/companion: This is always done before ♦️.
* ♦️: Draw X. Players collectively draw X cards starting with the current player and moving in clockwise order.
    * Skip players with maximum hand size.
    * There is no penalty for failing to draw from an empty the Tavern deck.
* ♣️: Deal double damage during Step 3.
* ♠️: Shield +X. Add X to the players' cumulative shield for the current enemy.
    * Shield is reset to 0 when enemy is defeated.

### Companion

Ace == Companion card.

Play Ace with another A-K card (excludes Jester; not allowed in Combos). Resolve both Suit Powers to the total summed value.

### Combos

Play sets of 2, 3, or 4 cards of the same value with total value <= 10. Resolve all Suit Powers to the total summed value.

Example sets (suit agnostic): pair of 2s, pair of 3s, pair of 4s, pair of 5s, triple 2s, triple 3s, quad 2s.

## Enemies

### Enemy Stats

|Enemy|Attack|Health|
|-|-|-|
|Jack|10|20|
|Queen|15|30|
|King|20|40|

Note: Attack means both the amount of damage the enemy does to current player in step 4 and the value of the card when a player plays it/discards it for taking damage.

### Enemy Immunity and Jester card

* Immunity: Suit Powers of cards with the same suit as the enemy are not resolved.
* Jester: When played, cancels this enemy's immunity. Current player instantly ends turn and chooses the next player.
    * Communication rules are temporarily changed, allowing players to _generally_ express desire/reluctance to go next.
* ♠️ clarification: Shield value is always updated, it is just not used to decrease enemy damage in step 4.
