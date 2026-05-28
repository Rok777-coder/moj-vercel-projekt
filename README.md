Environment variables se uporabljajo za konfiguracijo aplikacije brez zapisovanja obcutljivih podatkov neposredno v kodo.

Environment variables se uporabljajo za konfiguracijo aplikacije brez zapisovanja obcutljivih podatkov neposredno v kodo.

\# Moj Vercel projekt



\## Opis

Kratek spletni projekt, ustvarjen z namenom spoznavanja sodobnih razvijalskih orodij, nadzora različic in avtomatizacije objavljanja na spletu.



\## Uporabljene tehnologije

\- HTML

\- CSS

\- JavaScript

\- GitHub

\- Vercel



\## Deploy

Production URL:

https://moj-vercel-projekt.vercel.app



\## CI/CD

Projekt uporablja GitHub in Vercel integracijo za neprekinjeno integracijo in neprekinjeno dostavo. Vsakič, ko se koda pošlje (push) na GitHub repozitorij, Vercel samodejno zazna spremembe in izvede nov deploy brez potrebe po ročnem posodabljanju.



\## Dodatna konfiguracija

V nastavitvah Vercel projekta (Project Settings -> Environment Variables) je bila dodana okoljska spremenljivka (Environment Variable) s ključem `SITE\_NAME` in vrednostjo `Moj Vercel projekt`. Ker gre za statični HTML projekt, te spremenljivke niso neposredno vidne v brskalniku, se pa uporabljajo za konfiguracijo aplikacije brez zapisovanja občutljivih podatkov neposredno v kodo.



\## Težave

Med delom sem naletel na naslednje izzive:

1\. \*\*Napaka pri prvem pushu na novo vejo:\*\* Pojavila se je napaka `src refspec update-content does not match any`. Težavo sem rešil tako, da sem najprej pravilno ustvaril vejo z `git checkout -b update-content` ter pred pushom uspešno izvedel `git add .` in `git commit`.

2\. \*\*Težava z osveževanjem GitHuba:\*\* Po uspešnem pushu na spletni strani GitHuba nisem takoj videl gumba "Compare \& pull request". Težavo sem odpravil s preprosto osvežitvijo brskalnika (F5).

3\. \*\*Konflikt pri checkoutu na main:\*\* Git lokalno ni pustil skoka nazaj na `main` vejo zaradi nepotrjenih lokalnih sprememb. To sem razrešil s prisilnim preklopom veje in prenosom zadnjega stanja z `git pull`.

