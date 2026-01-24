Poatup instalace
---
1. Nejdriv instalace Kodi
2. instalace ceskeho repozitare dle https://repo.xbmc-kodi.cz/
3. Instalace i-vysilani
4. Instalace Oneplay

a) instalace one play z repozitare
b) instalace simple tv client



Doplněk pro Oneplay

Doplněk Oneplay umožnuje sledování živého vysílání Oneplay, pořadů z archivu, základní práci s nahrávkami a integraci s IPTV Simple Clientem (generování playlistu, EPG a spouštění pořadů). Pro PVR klienty přidává i kontextové menu v EPG, pro nastavení nahrávek).

Po instalaci doplňku je potřeba v nastavení zadat přihlašovací údaje do Oneplay! 

Pro použítí v doplňku použijte profil, který nemá nastavené Oblíbené kanály ve Oneplay. Oblíbené kanály mění pořadí kanálů a nefunguje pak správně jejich číslování.

Pokud cítíte neodolatnou potřebu něco autorovi symbolicky! přispět, můžete použít PayPal. 

Poslání logu

Pokud budete požádani o poslání logu, udělejte následující:

* pokud nemáte nainstalovaný doplněk Kodi Logfile Uploader, nainstalujte si ho  z Kodi Add-on repository - Doplňky programů (pokud zvládnete kodi.log vykopírovat a poslat emailem, není doplněk potřeba)
* v nastavení Kodi - Systém - Protokolování povolte Povolit protokolování ladění
* v doplňku na záložce Logování zapněte volby Logovaní požadavků a Logování odpovědí
* restartujte Kodi, aby se vytvořil čistý log
* nasimulujte problém
* spusťte Kodi Logifle Uploader, dejte upload a pošlete soukromou zprávou adresu k logu (alternativně můžete log poslat na email, který vám přes SZ pošlu)
* nastavení logování můžete stejným způsobem vypnout

Log nebo odkaz na něj nezveřejňujte na fóru, pokud to nebude jen nějaká konkrétní chybová hláška nebo část logu, v které nejsou žádné informace, které  by nemohl vidět každý! 


Zprovoznění IPTV Simple Clienta
IPTV simple client se konfiguruje v ramci konfigurace doplňku OnePlay

IPTV Simple Client umožňuje v Kodi využít funkcionalit PVR doplňků pro různé IPTV Služby. V doplňku Oneplay je potřeba nastavit adresář, kam bude uložený playlist a EPG, s kterým pak IPTV SC pracuje. Playlist je potřeba vygenerovat ručně, EPG pak můžete nechat generovat v pravidelném intervalu.

V nastavení IPTV Simple Clienta pak na záložce obecné vyberte v cestě k seznamu m3u playlist z adresáře, kam jste ho nechali vygenerovat (playlist.m3u případně playlist.txt) a stejným způsobem na záložce Televizní program pak v XMLTV cesta vyberte soubor oneplay_epg.xml, který obsahuje EPG.

Pro zpětné přehrávání je potřeba v nastavení IPTV Simple Clienta povolit tzv. catchup. Záložka Catchup je až za Časový posun, takže nemusí být vidět a bude nutné se v seznamu záložek posunout na konec. Kromě samotného povolení catchupu si můžete nastavit i jiné časové okno, pro které bude v televizním programu zpětné přehrání dostupné. V televizním programu byste měli vidět u pořadu, kde je zpětné přehrání k dispozici v levém dolním rohu zelenou tečku a v kontextovém menu Přehrát program.

V případě problémů hlavně po změnách může pomoct v  PVR a Živé vysílání - Obecné dát Vymazat data a vybrat Vše a po vymazání restartujte Kodi. IPTV Simple Client si pak playlist i EPG načte znovu a data se uloží do DB Kodi.

Kodi 18 (Leia)

Doplněk je k dispozici jen Kodi 19 (Matrix) a novější.

Nastavení

Záložka Přihlášení
Login - přihlašovací jméno do Oneplay (stejné jako např. na webu)
Heslo - heslo k Oneplay
Device Id (libovolný alfanumerický řetězec) - ID zařízení, pokud ho neuvedete vygeneruje se samo
Profilový PIN - profilový PIN v případě, že ho máte v profilu ve Oneplay nastavený
Rodičovský PIN - pokud se rodičovský PIN shoduje s nastaveným ve Oneplay, nebude nutné u chráněných kanálů zadávat PIN
Nová session - vynutí se získání nové session

Záložka Nastavení
Preferovat HLS streamy - při přehrávání se preferuje HLS stream bez DRM, pokud je k dispozici (může řešit problémy související s DRM ochranou)
Alternativní barva popisků - nastavení barvy doplňujících informací u položek (výchozí je tmavě šedá)
Obecné zobrazení seznamů v TV - seznamy v archivu i živého vysílání budou mít obecný vzhled a ne podle typu položek
Řazení epizod - řazení epizod v kategoriích
Počet nejnovějších epizod oblíbených - počet nejnovějších epizod každé série, které se budou zobrazovat v Nejnovější epizody oblíbených
Historie vyhledávání - počet posledních vyhledání, které se mají zobrazovat
Čísla kanálů - zobrazení a případně formát čísla kanálů. Standardně se nezobrazuje
Stahovat detaily pořadů - stahují se detailní data k pořadům v kategoriích
Vymazat keš - smaže DB se staženými detailními informacemi o pořadech
Skrýt Nastavení Oneplay v menu - skryje v menu volbu Nastavení Oneplay, která slouží pro správu kanálů a nastavení doplňku

Záložka IPTV Simple Client
Adresář pro playlist a EPG - adresář, kam se bude ukládat playlist a soubor s EPG pro IPTV Simple Clienta. Po nastavení změnu nejdřív uložte kliknutím na tlačítko OK, jinak generování nebude fungovat
Soubor s playlistem - výběr jména souboru s playlistem. Pokud se vám na Androidu playlist nebude vytvářet, můžete změnit jméno na playlist.txt
Automaticky generovat EPG - při spuštění Kodi a pak v zadaném intervalu bude generovat EPG. Standardně vypnuto.
Zobrazovat informace o generování EPG - zobrazení informací o automatickém generování EPG
Interval pro generování EPG (hod.) - interval, v kterém se bude generovat EPG pro IPTV Simple Clienta. Standardně 12 hodin
Počet dnů pro stahovaní EPG zpětně - počet dnů, pro které se bude zpětně stahovat EPG. Standardně 1 den
Počet dnů pro stahovaní EPG dopředu - počet dnů, pro které se bude dopředu stahovat EPG. Standardně 1 den
Catchup mod - způsob, jakým se do playlistu přidávají informace pro catchup. Výchozí je append
Generovat playlist - vygeneruje playlist do zadaného adresáře do souboru playlist.m3u
Generovat EPG - vygeneruje EPG do zadaného adresáře do souboru o2tv_epg.xml

InputStream Helper/Widevine
Používat InputStream Helper - povoluje volání InputStream Helperu pro automatickou instalaci a aktualizaci Widevine CDM knihovny
Zobrazení informací - zobrazení informace o instalaci Widevine CDM knihovny
Nastavení InputStream Helper - nastavení InputStream Helper
(Re)instalovat Widevine CDM - instalace Widevine CDM knihovny
Odstranit Widevine CDM... - odinstalace Widevine CDM knihovny

Záložka Logování
Logování požadavků - URL - budou se logovat adresy požadavků na servery Oneplay
Logování odpovědí - budou se logovat odpovědi, které vrací servery Oneplay
Nelogovat velké odpovědi - velké odpovědi nebudou logované

Odesláno z iPadu
