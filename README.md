# PageRank
Search Engine for https://www.lawfareblog.com using PageRank

Task 1:
Part 1:

Running power method on sample of urls
```
run pagerank.py --data=./small.csv.gz --verbose
DEBUG:root:computing indices
DEBUG:root:computing values
INFO:root:rank=0 pagerank=6.0257e-01 url=4
INFO:root:rank=1 pagerank=4.6414e-01 url=6
INFO:root:rank=2 pagerank=3.4544e-01 url=5
INFO:root:rank=3 pagerank=1.9498e-01 url=2
INFO:root:rank=4 pagerank=9.9210e-02 url=3
INFO:root:rank=5 pagerank=8.9347e-02 url=1
```

Part 2:
Running search query with input 'corona'

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --search_query='corona'
INFO:gensim.models.keyedvectors:precomputing L2-norms of word weight vectors
INFO:root:rank=0 pagerank=0.001003776676952839 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
INFO:root:rank=1 pagerank=0.0008922395063564181 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
INFO:root:rank=2 pagerank=0.0007039029151201248 url=www.lawfareblog.com/britains-coronavirus-response
INFO:root:rank=3 pagerank=0.0006915341946296394 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
INFO:root:rank=4 pagerank=0.000670412031468004 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
INFO:root:rank=5 pagerank=0.0006625585374422371 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
INFO:root:rank=6 pagerank=0.0006504578050225973 url=www.lawfareblog.com/congressional-homeland-security-committees-seek-ways-support-state-federal-responses-coronavirus
INFO:root:rank=7 pagerank=0.0006361958803609014 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
INFO:root:rank=8 pagerank=0.000612482544966042 url=www.lawfareblog.com/house-subcommittee-voices-concerns-over-us-management-coronavirus
INFO:root:rank=9 pagerank=0.0006018723943270743 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response
```

Running search query with input 'trump'

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --search_query='trump'
INFO:gensim.models.keyedvectors:precomputing L2-norms of word weight vectors
INFO:root:rank=0 pagerank=0.005782557651400566 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=1 pagerank=0.005233839154243469 url=www.lawfareblog.com/document-trump-revokes-obama-executive-order-counterterrorism-strike-casualty-reporting
INFO:root:rank=2 pagerank=0.005129670724272728 url=www.lawfareblog.com/trump-administrations-worrying-new-policy-israeli-settlements
INFO:root:rank=3 pagerank=0.004659898113459349 url=www.lawfareblog.com/dc-circuit-overrules-district-courts-due-process-ruling-qasim-v-trump
INFO:root:rank=4 pagerank=0.004593398422002792 url=www.lawfareblog.com/donald-trump-and-politically-weaponized-executive-branch
INFO:root:rank=5 pagerank=0.004307133611291647 url=www.lawfareblog.com/how-trumps-approach-middle-east-ignores-past-future-and-human-condition
INFO:root:rank=6 pagerank=0.0040934765711426735 url=www.lawfareblog.com/why-trump-cant-buy-greenland
INFO:root:rank=7 pagerank=0.0037590833380818367 url=www.lawfareblog.com/oral-argument-summary-qassim-v-trump
INFO:root:rank=8 pagerank=0.003450872143730521 url=www.lawfareblog.com/dc-circuit-court-denies-trump-rehearing-mazars-case
INFO:root:rank=9 pagerank=0.0034484383650124073 url=www.lawfareblog.com/second-circuit-rules-mazars-must-hand-over-trump-tax-returns-new-york-prosecutors
```

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --search_query='iran'
INFO:gensim.models.keyedvectors:precomputing L2-norms of word weight vectors
INFO:root:rank=0 pagerank=0.005129670724272728 url=www.lawfareblog.com/trump-administrations-worrying-new-policy-israeli-settlements
INFO:root:rank=1 pagerank=0.005016769748181105 url=www.lawfareblog.com/update-military-commissions-continued-health-issues-recusal-motion-and-new-cell-al-iraqi
INFO:root:rank=2 pagerank=0.004574609454721212 url=www.lawfareblog.com/praise-presidents-iran-tweets
INFO:root:rank=3 pagerank=0.004417411983013153 url=www.lawfareblog.com/how-us-iran-tensions-could-disrupt-iraqs-fragile-peace
INFO:root:rank=4 pagerank=0.004365929868072271 url=www.lawfareblog.com/haftar-attacking-tripoli-us-needs-re-engage-libya
INFO:root:rank=5 pagerank=0.0034236714709550142 url=www.lawfareblog.com/france-makes-play-try-foreign-fighters-iraq
INFO:root:rank=6 pagerank=0.0026927897706627846 url=www.lawfareblog.com/cyber-command-operational-update-clarifying-june-2019-iran-operation
INFO:root:rank=7 pagerank=0.002256679581478238 url=www.lawfareblog.com/document-sens-kaine-and-young-introduce-bill-revoke-iraq-force-authorizations
INFO:root:rank=8 pagerank=0.0019391420064494014 url=www.lawfareblog.com/aborted-iran-strike-fine-line-between-necessity-and-revenge
INFO:root:rank=9 pagerank=0.0018262730445712805 url=www.lawfareblog.com/its-not-only-iraq-and-syria
```

Part 3:
Get a list of the pages with the largest pagerank

```
python3 pagerank2.py --data=./lawfareblog.csv.gz
INFO:root:rank=0 pagerank=0.2874051630496979 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
INFO:root:rank=1 pagerank=0.2874051630496979 url=www.lawfareblog.com/lawfare-job-board
INFO:root:rank=2 pagerank=0.2874051630496979 url=www.lawfareblog.com/masthead
INFO:root:rank=3 pagerank=0.2874051630496979 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
INFO:root:rank=4 pagerank=0.2874051630496979 url=www.lawfareblog.com/subscribe-lawfare
INFO:root:rank=5 pagerank=0.2874051630496979 url=www.lawfareblog.com/litigation-documents-related-appointment-matthew-whitaker-acting-attorney-general
INFO:root:rank=6 pagerank=0.2874051630496979 url=www.lawfareblog.com/documents-related-mueller-investigation
INFO:root:rank=7 pagerank=0.2874051630496979 url=www.lawfareblog.com/our-comments-policy
INFO:root:rank=8 pagerank=0.2874051630496979 url=www.lawfareblog.com/upcoming-events
INFO:root:rank=9 pagerank=0.2874051630496979 url=www.lawfareblog.com/topics
```

Get a list of the pages with the largest pagerank but with the filter_ratio = 0.2 to remove all non-article pages

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --filter_ratio=0.2
INFO:root:rank=0 pagerank=0.3469613492488861 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=1 pagerank=0.29521211981773376 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
INFO:root:rank=2 pagerank=0.29039666056632996 url=www.lawfareblog.com/opening-statement-david-holmes
INFO:root:rank=3 pagerank=0.15178653597831726 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
INFO:root:rank=4 pagerank=0.15098513662815094 url=www.lawfareblog.com/todays-headlines-and-commentary-1964
INFO:root:rank=5 pagerank=0.15098513662815094 url=www.lawfareblog.com/todays-headlines-and-commentary-1963
INFO:root:rank=6 pagerank=0.15071173012256622 url=www.lawfareblog.com/lawfare-podcast-week-was-impeachment
INFO:root:rank=7 pagerank=0.14956679940223694 url=www.lawfareblog.com/todays-headlines-and-commentary-1962
INFO:root:rank=8 pagerank=0.14366623759269714 url=www.lawfareblog.com/cyberlaw-podcast-mistrusting-google
INFO:root:rank=9 pagerank=0.14239734411239624 url=www.lawfareblog.com/lawfare-podcast-bonus-edition-gordon-sondland-vs-committee-no-bull
```

Part 4:

Next few runs show the different results shown when alpha values are altered for alterations in how fast they converge, and when they have a filter for non-article urls. 

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --verbose
INFO:root:rank=0 pagerank=0.2874051630496979 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
INFO:root:rank=1 pagerank=0.2874051630496979 url=www.lawfareblog.com/lawfare-job-board
INFO:root:rank=2 pagerank=0.2874051630496979 url=www.lawfareblog.com/masthead
INFO:root:rank=3 pagerank=0.2874051630496979 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
INFO:root:rank=4 pagerank=0.2874051630496979 url=www.lawfareblog.com/subscribe-lawfare
INFO:root:rank=5 pagerank=0.2874051630496979 url=www.lawfareblog.com/litigation-documents-related-appointment-matthew-whitaker-acting-attorney-general
INFO:root:rank=6 pagerank=0.2874051630496979 url=www.lawfareblog.com/documents-related-mueller-investigation
INFO:root:rank=7 pagerank=0.2874051630496979 url=www.lawfareblog.com/our-comments-policy
INFO:root:rank=8 pagerank=0.2874051630496979 url=www.lawfareblog.com/upcoming-events
INFO:root:rank=9 pagerank=0.2874051630496979 url=www.lawfareblog.com/topics
```

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --verbose --alpha=0.99999
INFO:root:rank=0 pagerank=0.28859302401542664 url=www.lawfareblog.com/snowden-revelations
INFO:root:rank=1 pagerank=0.28859302401542664 url=www.lawfareblog.com/lawfare-job-board
INFO:root:rank=2 pagerank=0.28859302401542664 url=www.lawfareblog.com/documents-related-mueller-investigation
INFO:root:rank=3 pagerank=0.28859302401542664 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
INFO:root:rank=4 pagerank=0.28859302401542664 url=www.lawfareblog.com/subscribe-lawfare
INFO:root:rank=5 pagerank=0.28859302401542664 url=www.lawfareblog.com/topics
INFO:root:rank=6 pagerank=0.28859302401542664 url=www.lawfareblog.com/masthead
INFO:root:rank=7 pagerank=0.28859302401542664 url=www.lawfareblog.com/our-comments-policy
INFO:root:rank=8 pagerank=0.28859302401542664 url=www.lawfareblog.com/upcoming-events
INFO:root:rank=9 pagerank=0.28859302401542664 url=www.lawfareblog.com/litigation-documents-related-appointment-matthew-whitaker-acting-attorney-general
```

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --verbose --filter_ratio=0.2
INFO:root:rank=0 pagerank=0.3469613492488861 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=1 pagerank=0.29521211981773376 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
INFO:root:rank=2 pagerank=0.29039666056632996 url=www.lawfareblog.com/opening-statement-david-holmes
INFO:root:rank=3 pagerank=0.15178653597831726 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
INFO:root:rank=4 pagerank=0.15098513662815094 url=www.lawfareblog.com/todays-headlines-and-commentary-1964
INFO:root:rank=5 pagerank=0.15098513662815094 url=www.lawfareblog.com/todays-headlines-and-commentary-1963
INFO:root:rank=6 pagerank=0.15071173012256622 url=www.lawfareblog.com/lawfare-podcast-week-was-impeachment
INFO:root:rank=7 pagerank=0.14956679940223694 url=www.lawfareblog.com/todays-headlines-and-commentary-1962
INFO:root:rank=8 pagerank=0.14366623759269714 url=www.lawfareblog.com/cyberlaw-podcast-mistrusting-google
INFO:root:rank=9 pagerank=0.14239734411239624 url=www.lawfareblog.com/lawfare-podcast-bonus-edition-gordon-sondland-vs-committee-no-bull
```

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --verbose --filter_ratio=0.2 --alpha=0.99999
DEBUG:root:computing indices
DEBUG:root:computing values
INFO:root:rank=0 pagerank=0.7014895677566528 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
INFO:root:rank=1 pagerank=0.7014873623847961 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
INFO:root:rank=2 pagerank=0.10551629960536957 url=www.lawfareblog.com/cost-using-zero-days
INFO:root:rank=3 pagerank=0.03175504133105278 url=www.lawfareblog.com/lawfare-podcast-former-congressman-brian-baird-and-daniel-schuman-how-congress-can-continue-function
INFO:root:rank=4 pagerank=0.022039713338017464 url=www.lawfareblog.com/events
INFO:root:rank=5 pagerank=0.01602667197585106 url=www.lawfareblog.com/water-wars-increased-us-focus-indo-pacific
INFO:root:rank=6 pagerank=0.016025930643081665 url=www.lawfareblog.com/water-wars-drill-maybe-drill
INFO:root:rank=7 pagerank=0.016022762283682823 url=www.lawfareblog.com/water-wars-disjointed-operations-south-china-sea
INFO:root:rank=8 pagerank=0.016019931063055992 url=www.lawfareblog.com/water-wars-song-oil-and-fire
INFO:root:rank=9 pagerank=0.016019923612475395 url=www.lawfareblog.com/water-wars-sinking-feeling-philippine-china-relations
```

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --verbose --filter_ratio=0.2
INFO:root:rank=0 pagerank=0.3469613492488861 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=1 pagerank=0.29521211981773376 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
INFO:root:rank=2 pagerank=0.29039666056632996 url=www.lawfareblog.com/opening-statement-david-holmes
INFO:root:rank=3 pagerank=0.15178653597831726 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
INFO:root:rank=4 pagerank=0.15098513662815094 url=www.lawfareblog.com/todays-headlines-and-commentary-1964
INFO:root:rank=5 pagerank=0.15098513662815094 url=www.lawfareblog.com/todays-headlines-and-commentary-1963
INFO:root:rank=6 pagerank=0.15071173012256622 url=www.lawfareblog.com/lawfare-podcast-week-was-impeachment
INFO:root:rank=7 pagerank=0.14956679940223694 url=www.lawfareblog.com/todays-headlines-and-commentary-1962
INFO:root:rank=8 pagerank=0.14366623759269714 url=www.lawfareblog.com/cyberlaw-podcast-mistrusting-google
INFO:root:rank=9 pagerank=0.14239734411239624 url=www.lawfareblog.com/lawfare-podcast-bonus-edition-gordon-sondland-vs-committee-no-bull
```

```
python3 pagerank2.py --data=./lawfareblog.csv.gz --verbose --filter_ratio=0.2 --alpha=0.99999
DEBUG:root:computing indices
DEBUG:root:computing values
INFO:root:rank=0 pagerank=0.7014895677566528 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
INFO:root:rank=1 pagerank=0.7014873623847961 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
INFO:root:rank=2 pagerank=0.10551629960536957 url=www.lawfareblog.com/cost-using-zero-days
INFO:root:rank=3 pagerank=0.03175504133105278 url=www.lawfareblog.com/lawfare-podcast-former-congressman-brian-baird-and-daniel-schuman-how-congress-can-continue-function
INFO:root:rank=4 pagerank=0.022039713338017464 url=www.lawfareblog.com/events
INFO:root:rank=5 pagerank=0.01602667197585106 url=www.lawfareblog.com/water-wars-increased-us-focus-indo-pacific
INFO:root:rank=6 pagerank=0.016025930643081665 url=www.lawfareblog.com/water-wars-drill-maybe-drill
INFO:root:rank=7 pagerank=0.016022762283682823 url=www.lawfareblog.com/water-wars-disjointed-operations-south-china-sea
INFO:root:rank=8 pagerank=0.016019931063055992 url=www.lawfareblog.com/water-wars-song-oil-and-fire
INFO:root:rank=9 pagerank=0.016019923612475395 url=www.lawfareblog.com/water-wars-sinking-feeling-philippine-china-relations
```

Task 2
Part 1

Using personalization vector to filter the personalization vector
Webpage is considered important if other coronavirus websites think that this website is important

```
run pagerank.py --data=./lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona'
DEBUG:root:computing indices
DEBUG:root:computing values
INFO:root:rank=0 pagerank=8.8870e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
INFO:root:rank=1 pagerank=8.8867e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
INFO:root:rank=2 pagerank=1.8256e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
INFO:root:rank=3 pagerank=1.4907e-01 url=www.lawfareblog.com/brexit-not-immune-coronavirus
INFO:root:rank=4 pagerank=1.4907e-01 url=www.lawfareblog.com/rational-security-my-corona-edition
INFO:root:rank=5 pagerank=1.0729e-01 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
INFO:root:rank=6 pagerank=1.0199e-01 url=www.lawfareblog.com/britains-coronavirus-response
INFO:root:rank=7 pagerank=1.0199e-01 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
INFO:root:rank=8 pagerank=9.4298e-02 url=www.lawfareblog.com/lawfare-podcast-mom-and-dad-talk-clinical-trials-pandemic
INFO:root:rank=9 pagerank=8.7207e-02 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
```

Different results given with the absence of personalization vector
Webpage is considered important if any other websites think that this website is important
```
python3 pagerank2.py --data=./lawfareblog.csv.gz --filter_ratio=0.2 --search_query='corona'
INFO:gensim.models.keyedvectors:precomputing L2-norms of word weight vectors
INFO:root:rank=0 pagerank=0.008131962269544601 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
INFO:root:rank=1 pagerank=0.007790825795382261 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
INFO:root:rank=2 pagerank=0.005226220469921827 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response
INFO:root:rank=3 pagerank=0.0039583845064044 url=www.lawfareblog.com/britains-coronavirus-response
INFO:root:rank=4 pagerank=0.003811446251347661 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
INFO:root:rank=5 pagerank=0.003397284774109721 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
INFO:root:rank=6 pagerank=0.0033633282873779535 url=www.lawfareblog.com/cyberlaw-podcast-how-israel-fighting-coronavirus
INFO:root:rank=7 pagerank=0.0033556800335645676 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
INFO:root:rank=8 pagerank=0.0032159897964447737 url=www.lawfareblog.com/congress-needs-coronavirus-failsafe-its-too-late
INFO:root:rank=9 pagerank=0.0031036492437124252 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
```

Part 2

Finds all webpages that have an emphasis on corona, but then removes them if they contain the word corona in them.

```
run pagerank.py --data=./lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona' --search_query='-corona'
DEBUG:root:computing indices
DEBUG:root:computing values
INFO:root:rank=0 pagerank=8.8870e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
INFO:root:rank=1 pagerank=8.8867e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
INFO:root:rank=2 pagerank=1.8256e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
INFO:root:rank=3 pagerank=1.0729e-01 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
INFO:root:rank=4 pagerank=9.4298e-02 url=www.lawfareblog.com/lawfare-podcast-mom-and-dad-talk-clinical-trials-pandemic
INFO:root:rank=5 pagerank=7.9633e-02 url=www.lawfareblog.com/fault-lines-foreign-policy-quarantined
INFO:root:rank=6 pagerank=7.5307e-02 url=www.lawfareblog.com/limits-world-health-organization
INFO:root:rank=7 pagerank=6.8115e-02 url=www.lawfareblog.com/chinatalk-dispatches-shanghai-beijing-and-hong-kong
INFO:root:rank=8 pagerank=6.4847e-02 url=www.lawfareblog.com/us-moves-dismiss-case-against-company-linked-ira-troll-farm
INFO:root:rank=9 pagerank=6.4847e-02 url=www.lawfareblog.com/livestream-house-foreign-affairs-committee-holds-hearing-crisis-idlib
```

Part 3

Finds all webpages that have an emphasis on North Korea, but then removes them if they have the word nuclear in them.
```
run pagerank.py --data=./lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='north korea' --search_query='-nuclear'
DEBUG:root:computing indices
DEBUG:root:computing values
INFO:root:rank=0 pagerank=2.2198e-01 url=www.lawfareblog.com/whats-point-charging-foreign-state-linked-hackers
INFO:root:rank=1 pagerank=2.1071e-01 url=www.lawfareblog.com/north-korean-hacker-charges-line-drawing-necessary-not-sufficient-part-deterrence
INFO:root:rank=2 pagerank=2.1071e-01 url=www.lawfareblog.com/law-and-public-intuition-use-force-part-3-views-president-trump-and-north-korea
INFO:root:rank=3 pagerank=1.9394e-01 url=www.lawfareblog.com/defense-helsinki-conference-asia-response-sam-roggeveen
INFO:root:rank=4 pagerank=1.9162e-01 url=www.lawfareblog.com/document-joint-statement-president-trump-and-kim-jong-un
INFO:root:rank=5 pagerank=1.8451e-01 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=6 pagerank=1.1914e-01 url=www.lawfareblog.com/opening-statement-david-holmes
INFO:root:rank=7 pagerank=1.1914e-01 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
INFO:root:rank=8 pagerank=1.0427e-01 url=www.lawfareblog.com/helsinki-asia-response-philip-bobbitt
INFO:root:rank=9 pagerank=8.5580e-02 url=www.lawfareblog.com/senate-examines-threats-homeland
```
