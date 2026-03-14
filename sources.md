# Graphic Novel & Comics Sources

Weekly scan sources for the "Weekly graphic novel scout" cron job.
Runs every Sunday at 10 AM ET → delivers to Telegram.

## News & Reviews
1. [The Comics Journal](https://www.tcj.com/) — serious comics criticism
2. [Comics Beat](https://comicsbeat.com/) — indie/literary industry news
3. [Broken Frontier](https://www.brokenfrontier.com/) — UK-based, strong on indie & European
4. [Book Riot Comics/Graphic Novels](https://bookriot.com/category/comics-graphic-novels/)
5. [Publishers Weekly Comics](https://www.publishersweekly.com/pw/by-topic/industry-news/comics/index.html)
6. [The Nib](https://thenib.com/) — political/journalism comics
7. [The Comics Reporter](https://comicsreporter.com/) — deep cuts, long-form

## Publisher Blogs
8. [Drawn & Quarterly](https://www.drawnandquarterly.com/blog)
9. [Fantagraphics](https://www.fantagraphics.com/blogs/news)
10. [New York Review Comics](https://www.nyrb.com/collections/comics) — literary, translated
11. [Breakdown Press](https://breakdownpress.com/) — UK art comics

## European / Translated
12. [European Comics in Translation](https://www.europecomics.com/) — Franco-Belgian and beyond
13. [ActuaBD](https://www.actuabd.com/) — French BD news, catches releases months before English translations
14. [Lambiek Comiclopedia](https://www.lambiek.net/) — encyclopedic, great for European artists

## Awards
15. [Angoulême Festival](https://www.bdangouleme.com/) — the Cannes of comics
16. [Eisner Awards](https://www.comic-con.org/awards/eisner-awards) — nomination season is great for discovery
17. [Ignatz Awards](https://www.spxpo.com/) — indie/alt comics awards from SPX

## Bookshop Picks (Brooklyn / NYC)
18. [Desert Island](https://desertislandcomics.com/) — Brooklyn, curation aligned with Viktor's taste
19. [Books Are Magic](https://www.booksaremagic.net/) — Brooklyn bookshop
20. [Printed Matter](https://www.printedmatter.org/) — art books/zines, NYC

## Reddit Communities
21. [r/graphicnovels](https://www.reddit.com/r/graphicnovels/) — weekly top
22. [r/altcomix](https://www.reddit.com/r/altcomix/) — weekly top
23. [r/bandedessinee](https://www.reddit.com/r/bandedessinee/) — weekly top

## Cron Job
- **Job ID:** `da14bfea-ea04-4293-bb6e-5edc99c2adaf`
- **Schedule:** `0 10 * * 0` (Sunday 10 AM ET)
- **Session:** isolated, announce to Telegram
- **Also checks:** Brooklyn Public Library availability via discover.bklynlibrary.org
