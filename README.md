# Pride Emoji

A COLR emoji font for LGBT+ pride flags. Non-exhausive, contributions welcome.

Thanks to the work by Mozilla on [twemoji-colr](https://github.com/mozilla/twemoji-colr) and Catmoji for the build system.

## Unicode

Currently, the pride emoji are represented by a well-formed (but "invalid" in the contemporary Unicode 14) *emoji tag sequence*. We use `U+1F308 RAINBOW` as the `tag_base`, which should avoid any conflict with the sole existing use for emoji tag sequences: Subdivision flags.

We can then use lowercase `a` to `z` in the Tags block (U+E0000 to U+E007F) to spell out the name of a flag. This has the benefit of giving us an unbounded amount of pride flags, without needing to provision new codepoints in Unicode.

So, to recap: `U+1F308 RAINBOW`, some ASCII sequence with component-wise addition with `0xE0000`, `U+E007F CANCEL TAG`.

The currently-implemented flags are:

|Tag (ASCII)|Character|
|-|-|-|
|`bi`|Bisexuality Flag|🌈󠁢󠁩󠁿|
|`nb`|Non-Binary Flag|🌈󠁮󠁢󠁿|
|`wlw`|Lesbian Flag|🌈󠁷󠁬󠁷󠁿|
|`mlm`|Gay Male Flag|🌈󠁭󠁬󠁭󠁿|

## Art

The art for the pride flags included in this repository is based on [twemoji](https://github.com/twitter/twemoji)'s Transgender and Rainbow flags.
