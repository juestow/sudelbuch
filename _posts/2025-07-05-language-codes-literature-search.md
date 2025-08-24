---
layout: post
comments: true
title : Language Codes (and Language Bias) in Library Search Engines
categories: [Search, Bibliographic databases, Online catalogue, Literature search, MARC language code]
---

MARC language codes, a bibliographic format used by many library catalogues,[^1] allow users to search for publications in particular languages.

[^1]: See the [definition on the MARC website](https://www.loc.gov/marc/faq.html#definition):   "MARC is the acronym for MAchine-Readable Cataloging. It defines a data format that emerged from a Library of Congress-led initiative that began nearly forty years ago. It provides the mechanism by which computers exchange, use, and interpret bibliographic information, and its data elements make up the foundation of most library catalogs used today. MARC became USMARC in the 1980s and MARC 21 in the late 1990s." For more information see [https://www.loc.gov/marc/](https://www.loc.gov/marc/).

For instance, the search string
> la:ger Kempelen AND (Sprechmaschine OR Schachautomat)
will return results for publications on/by "Kempelen" in German.

Combined with Boolean operators, language shortcodes can be deployed for very specific search queries:
`la:ger Kempelen AND (Sprechmaschine OR Schachautomat)`
= publications in German containing either a) both the keywords "Kempelen" and "Sprechmaschine" or b) both "Kempelen" and "Schachautomat" (which produces eleven results on JSTOR: [https://www.jstor.org/action/doBasicSearch?Query=la%3Ager%20Kempelen%20AND%20(Sprechmaschine%20OR%20Schachautomat)&so=rel](https://www.jstor.org/action/doBasicSearch?Query=la%3Ager%20Kempelen%20AND%20(Sprechmaschine%20OR%20Schachautomat)&so=rel))

`la:ger Kempelen OR sprechmaschine`
= results matching the criteria "all publications in German that contain either "Kempelen" or "Sprechmaschine" (144 results [https://www.jstor.org/action/doBasicSearch?Query=la%3Ager%20Kempelen%20OR%20sprechmaschine](https://www.jstor.org/action/doBasicSearch?Query=la%3Ager%20Kempelen%20OR%20sprechmaschine))

`la:ger Kempelen AND sprechmaschine`
= publications in German that include both  "Kempelen" and "Sprechmaschine" (four titles on JSTOR: [https://www.jstor.org/action/doBasicSearch?Query=la%3Ager%20Kempelen%20AND%20sprechmaschine](https://www.jstor.org/action/doBasicSearch?Query=la%3Ager%20Kempelen%20AND%20sprechmaschine))

However, we can use language shortcodes to get the numbers for all publications in each language. By entering only the tag `la:` with a blank, user can examine if a specific language is underrepresented in the database.

The query `la:`  renders on JSTOR the following ranking:

1. English (2,849,657)
2. French (962,098)
3. Spanish; Castilian (394,701)
4. Italian (378,408)
5. German (216,161)
6. Portuguese (25,268)
7. Dutch; Flemish (12,375)
8. Hebrew (9,725)
9. Czech (9,029)
10. Irish (8,944)
11. Latin (7,303)
12. Danish (4,586)
13. Galician (3,707)
14. Polish (2,861)
15. Bengali (2,673)
16. Catalan; Valencian (1,971)
17. Arabic (1,598)
18. Russian (1,591)
19. Romanian; Moldavian; Moldovan (1,450)
20. Urdu (1,424)
21. Greek, Modern (1453-) (1,243)
22. Swedish (1,224)
23. Chinese (1,141)
24. Malayalam (837)
25. Norwegian (785)

![Screenshot JSTOR (2025)](/assets/img/jstor-marc-lang.png)

[https://www.jstor.org/action/doBasicSearch?Query=la%3A&so=rel](https://www.jstor.org/action/doBasicSearch?Query=la%3A&so=rel)

