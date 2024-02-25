---
---

I proved that shogi is not a second-player win (i.e., either a first-player win or a draw) assuming both of the following are true:

1. Both P-26 G-32 (A) [^1] and P-76 G-32 (B) [^2] are perfect play for the second player.
2. Either G-68 P-84 (A') [^3] or G-68 P-34 (B') [^4] is perfect play for the second player.

Proof: By strategy-stealing.  Assume that shogi is a second-player win.  Then both (A) and (B) are second-player wins by Assumption 1.  However, in both (A') and (B'), playing G-78 makes the first player equivalent to the second player in (A) and (B), respectively.  (Either is perfect play for the second player by Assumption 2.)  It then follows that shogi is a first-player win.  Contradiction.

Although neither assumption can be proven, most contemporary shogi engines may support both.  By the contrapositive, if shogi is a second-player win, then at least one of the following must be true:

1. P-26 G-32 is not perfect play for the second player.
2. P-76 G-32 is not perfect play for the second player.
3. Both G-68 P-84 and G-68 P-34 are not perfect play for the second player.

[^1]: http://kyokumen.jp/positions/91901
[^2]: http://kyokumen.jp/positions/61913
[^3]: http://kyokumen.jp/positions/14532033
[^4]: http://kyokumen.jp/positions/14532034
