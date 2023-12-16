---
date: '2023-04-18 05:38:00 +0000'
---

I proved that shogi is either a first-player win or a draw (i.e., not a second-player win) if both of the following assumptions are true:

1. Both P-26 G-32 [^1] (A) and P-76 G-32 [^2] (B) are perfect play for the second player.
2. Either G-68 P-84 [^3] (A') or G-68 P-34 [^4] (B') is perfect play for the second player.

Proof: By strategy-stealing. Assume that shogi is a second-player win. Then both (A) and (B) are second-player wins by Assumption 1. However, in both (A') and (B'), by playing G-78, the first player can be equal to the second player in (A) and (B), respectively. (Either is perfect play for the second player by Assumption 2.) It then follows that shogi is a first-player win. Contradiction.

Although neither assumption can be proven, this shows the connection between the opening theory of shogi and its game-theoretic value. Most contemporary shogi engines would support both assumptions. However, especially in (B) of Assumption 1, it may be controversial whether the move G-32 is perfect or not.

By the contrapositive, if shogi is a second-player win, then at least one of the following must be true:

1. P-26 G-32 is not perfect play for the second player.
2. P-76 G-32 is not perfect play for the second player.
3. Both G-68 P-84 and G-68 P-34 are not perfect play for the second player.


[^1]: http://kyokumen.jp/positions/91901
[^2]: http://kyokumen.jp/positions/61913
[^3]: http://kyokumen.jp/positions/14532033
[^4]: http://kyokumen.jp/positions/14532034
