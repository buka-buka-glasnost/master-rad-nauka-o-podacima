# Analiza scenarija: "Božji usamljeni ljudi"

Računarska analiza jezika protagonista u četiri scenarija Pola Šrejdera, urađena za master rad
*Božji usamljeni ljudi: računarska analiza jezika protagonista u scenarijima Pola Šrejdera*
(Univerzitet Singidunum, 2026)

Korpus čine iskazi četvorice protagonista: Trevisa Bikla (*Taksista*, 1976), Džona LeTura (*Fatalna nesanica*, 1992), Ernsta Tolera (*Iskušenik*, 2017) i Vilijama Tela (*Kockar*, 2021). Svaki iskaz je obeležen narativnim modom - dijalog ili narracija - i to je osnovna osa poređenja u celom radu. Ukupno 1.158 iskaza i oko 13.700 tokena.

Notebook obuhvata sedam korata: spajanje parsiranih scenarija u jedinstven korpus, ocenjivanje sentimenta i emocija transformerskim modelima, ocenjivanje sentimenta leksikonskim pristupom (VADER), deskriptivne i leksičke mere, analizu zajedničkog i distinktivnog vokabulara, poređenje dva pristupa sentimentu i prikaz emocionalnih trajektorija kroz narativ. Naslovi odeljaka nose oznake potpoglavlja iz rada, tako da se svaki izlaz može povezati sa mestom na kojem se tumači.

**Podaci.** Sami scenariji nisu deo repozitorijuma, jer su zaštićeni autorskim pravom. Izvori su navedeni u radu: tri scenarija sa sajta scriptslug.com i jedan sa sajta imsdb.com, svi preuzeti u junu 2026. Kod za parsiranje nalazi se u prilogu rada. Notebook polazi od izlaza tog koraka - četiri '.csv' fajla sa kolonama 'speaker', 'type', 'record_no', 'line'. Ocenjen korpus 'all_lines_scored.csv' priložen je uz repozitorijum, pa se svi koraci posle ocenjivanja mogu ponoviti bez pristupa scenarijima.

**Pokretanje.** Redom, od prve ćelije. Ocenjivanje celog korpusa na procesoru traje nekoliko minuta, sa grafičkom karticom znatno kraće. Potrebni paketi: 'pandas', 'numpy', 'scipy', 'scikit-learn', 'transformers', 'vaderSentiment', 'nltk', 'matplotlib', 'seaborn'. Za NLTK je potrebno preuzeti i listu zaustavnih reči ('nltk.download('stopwords')'). Ćelija sa leksičkim profilom koristi 'include_groups', pa zahteva pandas 2.2 ili noviji.
