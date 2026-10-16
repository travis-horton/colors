# colors — what changed, in plain words

The whole history of this project, newest first, written for someone who has never seen the code. It began on 20.0209 as a small set of drawing helpers and became, the same afternoon, a single piece of code for describing colors, shared by other projects. Every entry is one step on the main version: a pull request, or a day's changes on one topic.

## October 2026

**colors #18: Bump tmp, eslint and eslint-config-airbnb-base** · [PR #18](https://github.com/travis-horton/colors/pull/18) · merged 26.1016.1035 · v1.0.8
- Behind the scenes: an automatic dependency update — "Bump tmp, eslint and eslint-config-airbnb-base".

**colors #20: Bump ansi-regex** · [PR #20](https://github.com/travis-horton/colors/pull/20) · merged 26.1016.1032 · v1.0.7
- Behind the scenes: an automatic dependency update — "Bump ansi-regex".

**colors #17: Bump minimatch from 3.0.4 to 3.1.5** · [PR #17](https://github.com/travis-horton/colors/pull/17) · merged 26.1016.1030 · v1.0.6
- Behind the scenes: an automatic dependency update — "Bump minimatch from 3.0.4 to 3.1.5".

**colors #15: Bump js-yaml from 3.13.1 to 3.15.2** · [PR #15](https://github.com/travis-horton/colors/pull/15) · merged 26.1016.1001 · v1.0.5
- Behind the scenes: an automatic dependency update — "Bump js-yaml from 3.13.1 to 3.15.2".

**colors #14: Bump lodash from 4.17.21 to 4.18.1** · [PR #14](https://github.com/travis-horton/colors/pull/14) · merged 26.1016.1001 · v1.0.4
- Behind the scenes: an automatic dependency update — "Bump lodash from 4.17.21 to 4.18.1".

**colors #11: Bump brace-expansion from 1.1.11 to 1.1.21** · [PR #11](https://github.com/travis-horton/colors/pull/11) · merged 26.1016.0956 · v1.0.3
- Behind the scenes: an automatic dependency update — "Bump brace-expansion from 1.1.11 to 1.1.21".

**colors #16: the change log catches up on entries it missed** · [PR #16](https://github.com/travis-horton/colors/pull/16) · merged 26.1015.0728 · v1.0.2
- Behind the scenes: the robot that writes this file after each change now also writes in any earlier finished change it missed, oldest first, with a "recorded late" note when it is more than an hour late. If GitHub won't answer one of its lookups, it skips only that one, records the newest change anyway, and fills the gap on a later run.

**colors #10: the project's past, written down** · [PR #10](https://github.com/travis-horton/colors/pull/10) · merged 26.1010.1210 · v1.0.1
- Behind the scenes: the history file now tells the whole story of the project in plain words, from its first day on 20.0209 up to the history tool, one entry per step, numbered from version 0.1.0.

**colors #9: security updates and a self-writing history** · [PR #9](https://github.com/travis-horton/colors/pull/9) · merged 26.1010.1150 · v1.0.0
- **Security updates** · merged 26.1010.1150
  Behind the scenes: six borrowed helper packages were moved to the versions that fix their known security problems, gathered from six waiting automatic update requests into one. Nothing about how the project works changes.
- **History tool** · merged 26.1010.1150
  Behind the scenes: added the tool that writes a plain-language entry into this project's history file every time a change is accepted.

## April 2020

**Helper tools brought up to date** · [commit](https://github.com/travis-horton/colors/commit/cb0822f) · merged 20.0427.0842 · v0.1.1
- Behind the scenes: the code-checking tool's style rules and its add-on for checking how files connect were moved to newer versions, along with about a dozen small packages they rely on, including the fixed versions of two with known security problems. The color code itself did not change.

## February 2020

**The project begins: a color tool** · [commits](https://github.com/travis-horton/colors/commits/master?since=2020-02-09&until=2020-02-09) · merged 20.0209.1453 · v0.1.0
- **[Version 1.0.0 and style rules](https://github.com/travis-horton/colors/commit/1d28caf)** · merged 20.0209.1453
  Behind the scenes: the project's settings file was marked version 1.0.0 by hand, and the project got the rules for its code-checking tool. The old hand-made "1.0.0" and "v1.0.0" labels on the project point at this step; the version numbers in this file were worked out later and count from 0.1.0 here.
- **[Just colors](https://github.com/travis-horton/colors/commit/97bcdaa)** · merged 20.0209.1447
  New: the color tool's way of producing color text was renamed, and it was made shareable in the older style that most JavaScript projects then expected, as the one thing the project offers. The README was retitled "Colors": helpful methods for using colors in JavaScript.
  Try it: open Terminal and paste
      cd ~/code/colors && node -e "const Color = require('./color.js'); console.log(new Color(255, 128, 0).rgbString())"
- **[From drawing helpers to a color file](https://github.com/travis-horton/colors/commit/63742e1)** · merged 20.0209.1335
  Behind the scenes: the file was renamed for colors, a README was added, and the two circle-drawing helpers were removed, leaving only the color tool, which was then tidied to the style a code-checking tool recommends (the tool was added too).
  Fixed: in the first version, making any color stopped with an error, because the whole-number check was called the wrong way. Making a color now works.
- **[First version](https://github.com/travis-horton/colors/commit/34105d4)** · merged 20.0209.1300
  New: a small set of helpers for drawing in a web page: one draws the outline of a circle, one a filled circle, and a color tool describes a color by its red, green and blue amounts (whole numbers only) plus an optional see-through amount that defaults to fully solid, and turns it into the color text a web page's drawing understands, such as rgb(255,128,0).
