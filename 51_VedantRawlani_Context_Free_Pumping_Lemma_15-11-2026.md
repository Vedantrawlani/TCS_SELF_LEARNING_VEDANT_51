# Context-Free Pumping Lemma (JFLAP experiment #33)

**Language tested:** L = { a^n b^n c^n : n >= 0 } (not context-free).

1. Computer picks m. Prover picks w = a^m b^m c^m.
2. Computer decomposes w = uvxyz with |vxy| <= m and |vy| >= 1. Because |vxy| <= m, vxy cannot touch all three letter blocks, so v and y together contain at most two distinct letters.
3. Prover picks i = 2: u v^2 x y^2 z raises the count of at most two letters but not the third, so the counts become unequal and the word is not in L.

Every legal decomposition fails, so L is not context-free.

**Caveat:** derived by hand from the lemma, not from a recorded JFLAP session.
