# Who Counts as What?

An interactive history of the race question on the U.S. census, from 1790 to the proposal to drop it from the 2030 census. By Gwen Sharp, as a companion to Chapter 7 (Race and Ethnicity) of *A Sociology Experiment*.

**Live site:** https://gsharpokie.github.io/whocountsaswhat/

## What it does

- **The census, year by year.** Sixteen stops from 1790 to 2030. Each shows that census’s choices as form-style checkboxes, highlights what was new, strikes through what was dropped, and says whether a census taker decided a person’s race or people chose for themselves. Original enumerator instructions are quoted where they make the point (the 1890 fractions, the 1930 “one-drop rule,” the 1940 reversal on Mexicans).
- **Same person, different census.** Students pick one of four people (one Black and one White parent; born in Mexico; family from India; family from Lebanon) and follow how that person would have been recorded across the years.
- **Talk about it.** Four discussion questions, including one that asks students to weigh the arguments for and against asking about race at all.

The page opens on 1930, the most striking year. Use **← Earlier** to start from 1790.

## For instructors

Each year has its own link, for a slide or an assignment. Add `#y` and the year to the end of the address:

- https://gsharpokie.github.io/whocountsaswhat/#y1890
- https://gsharpokie.github.io/whocountsaswhat/#y1930
- https://gsharpokie.github.io/whocountsaswhat/#y2030 (the proposed 2030 change)

## Keeping it current

The **2030?** stop describes the Census Bureau’s September 10, 2026 proposed rule (91 FR 57524) to remove race and ethnicity questions from the 2030 census form. Public comments closed November 2, 2026. Update this stop when the rule is finalized, changed, or withdrawn, and update the **2024** stop if the 2024 federal standards are revised.

## Editing the page

Everything is in `index.html`. Near the top of the `<script>` section:

- `const STOPS = [` holds one entry per census year. `list` is the full set of choices (used only where verified); `add` and `drop` are the changes highlighted for that year; `text` is the explanation.
- `const PEOPLE = [` holds the four people. Each line in a `trail` is `["year", "how they were recorded", "note"]`; use `null` for “No race question.”

To edit, open `index.html` on GitHub, select the pencil icon, make the change, and select **Commit changes**. The live site updates within a few minutes. Use curly quotes and apostrophes, and keep the commas between entries.

## Turning on the site (one time)

Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the **main** branch and the **/ (root)** folder, and select **Save**. The site goes live a minute or two later.

The page’s “Suggest a correction” link opens a new issue in this repository, so keep Issues turned on (Settings → General → Features).

## Sources

- U.S. Census Bureau, “Measuring Race and Ethnicity Across the Decades: 1790–2010” (2015).
- Original enumerator instructions (1890, 1930, 1940, 1950) and the 1980 questionnaire, via IPUMS USA.
- Pew Research Center, “Counting Race” and “The Changing Categories the U.S. Census Has Used to Measure Race” (both 2025).
- U.S. Census Bureau, “Improvements to the 2020 Census Race and Hispanic Origin Question Designs” (2021).
- Office of Management and Budget, Directive No. 15 (1977) and its 2024 revision (89 FR 22182).
- U.S. Census Bureau, proposed rule on demographic questions, 91 FR 57524 (September 10, 2026).

Full links are on the page.

## Author

Created by Gwen Sharp ([@gsharpokie](https://x.com/gsharpokie)).

## License

© 2026 Gwen Sharp. Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): you may share and adapt it for noncommercial purposes with credit. See [LICENSE](LICENSE).
