# Je možné github použít pro zálohování jakéhokoli obsahu?

(konverzace s AI Gemini)

GitHub **není určen** pro obecné zálohování jakéhokoli obsahu, ačkoliv technicky umožňuje nahrát širokou škálu souborů. Jeho primárním účelem je správa verzí zdrojového kódu a spolupráce na vývoji.

Zde jsou hlavní omezení, která byste měli zvážit:

1\. Velikostní limity (Limitující faktor)

-   **Soubory:** Maximální velikost jednoho souboru je **100 MB**. Pokud nahráváte přes prohlížeč, limit je dokonce jen **25 MB**.
-   **Repozitáře:** GitHub doporučuje udržovat repozitář pod **1 GB**. Nad **5 GB** vás pravděpodobně kontaktuje podpora s žádostí o nápravu. Existuje sice teoretický "tvrdý" limit 100 GB, ale ten je vynucován spíše výjimečně a není garantován.
-   **Git LFS:** Pro větší binární data (videa, grafika) je nutné použít [Git Large File Storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github), které má ovšem v bezplatné verzi přísné limity na šířku pásma a úložiště.

2\. Typ obsahu a soukromí

-   **Binární soubory:** Git (systém, na kterém GitHub běží) je velmi neefektivní při verzování velkých binárních souborů (fotky, filmy, archivy). Každá změna v souboru může způsobit, že se v historii uloží celá jeho nová kopie, což extrémně rychle vyčerpá místo.
-   **Důvěrnost:** Přestože jsou soukromé repozitáře bezpečné, GitHub v podmínkách upozorňuje, že nenese odpovědnost za ztrátu dat a doporučuje používat externí nástroje pro skutečné zálohování samotného GitHubu.

3\. Nevýhody oproti cloudovým diskům

-   **Složitost:** Na rozdíl od Google Drive nebo Dropboxu vyžaduje GitHub znalost příkazů Gitu nebo používání specializovaných aplikací.
-   **Rychlost:** Nahrávání a stahování (cloning) velkých objemů dat je na GitHubu výrazně pomalejší než u služeb určených k ukládání souborů.

**Shrnutí:** Pro zálohu fotek z dovolené nebo filmů je GitHub **zcela nevhodný**. Pro textové dokumenty, konfigurační soubory nebo drobnější projekty je skvělý díky možnosti sledovat historii změn.

Chcete poradit s nastavením **[Git LFS](https://git-lfs.com/)** pro konkrétní projekt, nebo hledáte spíše doporučení na **tradiční cloudové úložiště**?
