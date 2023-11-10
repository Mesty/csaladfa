# csaladfa
Családfa
# Szerző
Név: Mester Ádám  
Elérhetőség: adam.mester87487@gmail.com
# GIT repository
Eddig csak én szerkesztettem a fájlt.  
Így lehet az ide-oda passzolgatni is.  
A párhuzamos szerkesztés és a követhetőség megtartása miatt csináltam neki GIT repót, hogy tudjuk rendesen verziókezelni.
# GenoPro
A \*.ged kiterjesztésű fájlokat a GenoPro alkalmazás tudja kezelni.  
Az alkalmazás és annak dokumentációja megtalálható itt: https://genopro.com/  
Alapvetően ez egy fizetős alkalmazás, de a legtöbb funkciója használható ingyenesen is, csak akkor nem tudsz benne menteni.  
Indításkor a "Regisztráció" ablakban "Cancel"-t kell nyomni, ha nem szeretnél fizetni, és a "visszakérdező" ablakban "Igen"-t nyomni a folytatásra.  
Ekkor megjelenik alapból a főablakban egy ablak három mukalappal (érdemes kinagyítani, mert alapból elég kicsire állítja őket).  
És akkor vagy elkezded egy új munkalapon, vagy a meglévőn Ctrl+A, majd Delete, hogy kitöröld az összes rajta lévő sallangot.  
Fájl-->Importálás, kitallózod a \*.ged fájlt, "Importálás", majd "Bezár".  
Ctrl+G-vel el tudod tüntetni a rácsot, ami nagyobb család kis nagyításánál ajánlott, mert nem skálázza át. Ha kell, ugyanezzel a billentyűkombóval tudot visszarakni.  
Valamint a "Nézet" menüben az "Érzelmi kapcsolatok megjelenítése" mellől is ki szoktam venni a pipát (sajnos nem jegyzi meg az alkalmazás, ezért ezt minden megnyitáskor el kell játszani), mert különben ráteszi a meglévő grafikákra, és kitakarja, ami mögötte van. Majd egyszer ezeket letisztázom, hogy geometriailag is jobban el legyenek helyezve.  
Ha szerkesztesz is bele, akkor a Fájl-->Exportálás-->Exportálás GEDCOM formátumba... menüt szoktam használni, de bármilyen más formátumot is választhatsz (lásd a listát). Én a GEDCOM formátumot szoktam használni, Unicode (UTF-8) karakterkódolással.  
Annyi van vele, hogy az alkalmazás, ha ingyenes verzióban használod, akkor nem enged menteni. Viszont exportálni akkor is enged. Bezáráskor megkérdezi, hogy szeretnéd-e menteni a fájlt, ekkor csak a "Nem"-re nyomhatsz, mert különben a fizetős verzió regisztrációja kéne hozzá.  
De nekem ez nem is hiányzik, hogy a saját formátumát használni tudjam, jó nekem a GEDCOM.  
Elvileg van még egy csomó lehetőség, pl. SVG-t, vagy komplett webportált is lehetne generálni belőle, amiket még nem igazán próbáltam, de lehet vele kísérletezni.
# Workflow
Kapott módosított forrásfájl esetén a fájllal egy, a szereksztője nevével azonos branchen lecseréljük az eredeti forrásfájlt, majd merge a develop branchre.  
Commit logokban a következő TAG-eket találtam ki:

Első TAG:
- [FAM] egy teljes család módosítása, tipikusan akkor használom ha embereket adok hozzá
- [DAT] személy(ek) adata(i)nak módosítása
- [GRA] ábrázolástechnikai módosítások
- [DOC] a leírásban, dokumentációban történő módosítások
- [LOC] a családfához nem kötődő, technikai változások (elsősorban a GIT repositoryhoz köthető, de lehet más is)
- [OUT] valamilyen kimeneti állományok előállítása/változtatása
- ([...] ha olyat csináltok benne, ami egyikhez sem köthető, nyugodtan találjatok ki újat, csak írjátok ide!)

Második TAG:
- [<Családnév>] Melyik családdal kapcsolatos a változtatás

Harmadik TAG:
- [+] hozzáadás
- [/] módosítás
- [*] hibajavítás
# GEDCOM
Szöveges, nyílt fájlformátum, így bármilyen text editorral is bele lehet szerkeszteni, illetve más alkalmazások is ismerik (pl. yEd).  
Bővebben a GEDCOM-ról: https://www.gedcom.org/index.html  
(Azért is előnyös a GEDCOM formátum, mert mivel szöveges, a verziókezelők is viszik).
# yEd Graph Editor
https://www.yworks.com/products/yed  
Az aktuális \*.ged forrást valamilyen oknál fogva nem kezeli, nem tudom, miért. Majd egyszer utánajárok.