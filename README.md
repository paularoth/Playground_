# Playground_komplettering

De mindre förändringar jag gjort i koden är att jag har ändrat ikonen för kompasspilen så att den, förhoppningsvis, passar in något bättre. 
Ändrade även hur delayen på vibrations-feedbacken sätts. Från att den sätts via olika nivåer till att den är en direkt funktion av vinkeln, med undantag för rätt riktning +- 10 grader då vibrationsmotorn stängs av. 

Den största förändringen i funktionalitet som jag implementerat är att appen nu varnar då enheterna (förälder och barn) är inom GPS:ens felmarginal. 
GPS:ens felmarginal är statiskt satt till 8m, vilket är baserat på USA:s officiella information om GPS. Som säger att "global average user range error" är 7.8m med en sannolikhet på 95%. https://www.gps.gov/systems/gps/performance/accuracy/
Varningen består av att rubriken som innehåller avstånd byts ut mot en varning och att ikonen för kompasspilen slutar snurra och byts ut mot en varningsikon. 
Ikonen kommer härifrån https://www.flaticon.com/free-icon/warning_130441#term=alert&page=1&position=, ikonen i appen är något modifierad (jag la till en vit bakgrund för bättre synlighet).
