# Teknisk dokumentation for SoundConnects - Eksamensprojekt 2sem

Dette website er udviklet i Astro, som er et digitalt framework, der gør det muligt at arbejde komponentbaseret i Visual Studio Code. Komponenter kan her både være sektioner i et flow på en bestemt side, eller mindre dele som burger menu eller footer, der går igen på alle sider.
For at sikre fleksibilitet og genanvendelighed i komponenterne har jeg anvendt Astro's props og slots. Dette gør det muligt at tilpasse indholdet dynamisk og effektivt genbruge komponenterne på tværs af forskellige sider og sektioner. Dette gør det også nemmere at lave indholdet dynamisk, da der allerede på tværs af Astro komponenterne bruges JavaScript.

### Projektstruktur:

- Billeder lægges i src/assets, og i tilfælde hvor den løsning ikke virker i forbindelse forskellige billeder i én komponent, bruges public/img
- Sider lægges i pages, og i tilfælde af dynamiske singleview, oprettes en specifik mappe indeni pages til dette, f.eks. pages/events

### Pages:

- filnavnet skrives med små bogstaver, og - bruges som mellemrum, f.eks. dj-pool.astro

### Components:

- filnavnet starter med stort bogstav, samt hvert nyt ord, uden nogen mellemrum, f.eks. DjPoolFiller.astro

### Classes:

- klasse navnet skrives med små bogstaver, uden mellemrum, f.eks. .gridcenter

### Const (Astro props):

- konstant navnet skrives med små bogstaver, uden mellemrum, f.eks. djname (med mindre der refereres til en dynamisk single event)

### Constants (var(--)):

- konstant navnet skrives med små bogstaver, og - bruges som mellemrum, f.eks. --bar-width

### Img (import):

- billede navnet skrives med små bogstaver, uden mellemrum, f.eks. djpool1

### Git branches:

- branch navnet skrives med små bogstaver, og - bruges som mellemrum.
- først nævnes hvilken side der arbejds på, derefter hvilken enhed/version, f.eks. events-mobile
- branchen merches først ind i main, når hele versionen så vidt muligt er gennemført

### Supabase

- websitet bruger brug af eksptern data hentet fra en database, så events.astro listen bliver dynamisk, og singleEvent.astro laves ud fra hvilke event du trykker på.
- singleEvent.astro filerne genkendes fra hinandnen ved at bruge hvert arrays id nr, som unik url
