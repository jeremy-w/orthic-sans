# Orthic Sans
Orthic Sans aims to provide a font using the [Orthographic Cursive alphabet](https://jeremy-w.github.io/orthic/manual#the-cursive-alphabet) for the core English alphabet focusing on the fully-written style. (No -ing, though the hooked -ks is probably appropriate.)

(Focusing on the fully-written style avoids the need to be context-sensitive in order to discern whether to use explicit ING or the -ing suffix, for example.)

## Why?
Simply: Orthic reading practice.

The main way to master reading a new alphabet is to read text in that new alphabet.

If a computer can set texts in Orthic, then it's easy to generate reading material, though perhaps awkard.

But if a font can do this rather than some out-of-band custom "text drawing" software,  students of the system can practice as a part of their everyday computer usage within the apps they're using already.

## What's Tricky
The primary technical challenge lies in sorting out cursive attachment and the several ligatures required:

- ch
- sp, ps, nsp, ph, phth
- th and word-final th
- dw, tw, wn, wm, wk
- wr, wh, word-final ws, initial w, medial and final w
- sw, sh, sr
- rce
- xh, xp, xt
- hooked ks
- all doubled letters, which should be a single letter with a dot below instead, except for EE/EI/IE, which is its own letter
- adjacent opposite-direction curves (`[mn][td]` and `[td][mn]`), which run together (e.g., "mt" does not go below the baseline).
- diphthongs, which depend on the preceding and sometimes following letter for their shape

## What's Changed from Textbook Orthic
Making Orthic fit for more than context-rich English text requires:

- systematically distinguishing uppercase and lowercase letters (is it `customerId` or `customerID`?)
    - perhaps a cross-mark? (this is nearest in spirit to the way handwritten Orthic indicates proper names)
    - perhaps double-stroking/outlining the letter, like `\mathbb`?
    - perhaps an over-dot? (though that would be "fun" with diacritics)
- making R vs L vs H vs CH easy to tell apart, even in isolation (is it "h. 1" or "ch. 1"?)
- distinguishing qu vs Qu vs qU vs QU vs just q/Q
    - we'll cross this bridge when we come to it. to start, we may just depart from Orthic and use the qu character for just q.
- distinguishing i from e, without having to sweat the following characters overmuch
    - perhaps an above-dot rather than an in-line-with-the-tick dot?
    - perhaps an "embedded" dot at the end of the uptick for I?

## Roadmap
- Sans font covering ASCII
    - Without cursive attachment or ligatures
    - With cursive attachment
    - With ligatures
    - Bonus: With diacritics (aim for broader "Latin alphabet" support)
- Mono font
- Maybe go back for a proper Italic version of each.

# Why not build atop an existing font?
I tried that. Building atop an existing font was a bad move:

- It's overwhelming for me as a novice
- I can't really reuse a ton of its "DNA" very well, due to the peculiar needs
  of the target script

I soon abandoned that approach in favor of building something small and
functional, though almost certainly uglier than what a proper type designer
would come up with, from scratch.
