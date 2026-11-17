# Корисничке приче

<!-- Самостално написати шест прича према додељеној спецификацији. -->
<!-- За сваку причу навести улогу, могућност, корист, F-ознаку и >= 2 критеријума прихватања. -->

## US-01 (F1)

Kao magacioner, zelim da evidentiram prijem robe od dobavljaca, kako bih imao tacan zapis o robi koja je usla u magacin.

Kriterijumi prihvatanja:
 Kada unesem naziv, opis, sifru artikla, pozitivnu kolicinu i naziv dobavljaca, prijem se cuva i prikazuje mi se dodeljeni ID.
 Ako je naziv, opis ili naziv dobavljaca prazan, ili kolicina nije veca od nule, unos se odbija uz poruku i nista se ne cuva.

## US-02 (F2)

Kao magacioner, zelim da evidentiram izlaz robe sa imenom primaoca, kako bih znao kome je roba izdata.

Kriterijumi prihvatanja:
 Ispravan izlaz koji ne prelazi raspolozivo stanje se cuva i prikazuje se dodeljeni ID.
 Ako je kolicina veca od raspolozivog stanja (npr. stanje 5, izlaz 8), unos se odbija i nista se ne cuva.

## US-03 (F3)

Kao sef magacina, zelim da vidim sve zapise sa tipom, ID-jem i statusom, kao i stanje po artiklu, kako bih imao pregled zaliha.

Kriterijumi prihvatanja:
 Prikaz sadrzi sve zapise sa tipom, ID-jem i statusom, u sazetom ili detaljnom obliku.
 Stanje artikla racuna samo potvrdjene zapise; ako nema zapisa, prikazuje se poruka da nema evidentiranih zapisa.

## US-04 (F4)

Kao magacioner, zelim da pretrazim zapise po sifri artikla, kako bih brzo pronasao promet za odredjeni artikal.

Kriterijumi prihvatanja:
 Pretraga „abc-1" pronalazi zapise sa sifrom „ABC-1" (velika i mala slova se ne razlikuju).
 Ako nijedan zapis nema trazenu sifru, prikazuje se poruka da nema rezultata.

## US-05 (F5)

Kao sef magacina, zelim da potvrdim promet, kako bi on uticao na stanje zaliha.

Kriterijumi prihvatanja:
 Potvrda evidentiranog zapisa mijenja status u „Potvrdjen" i stanje se azurira.
 Potvrda koja bi dovela do negativnog stanja, kao i potvrda nepostojeceg ID-ja, odbija se bez ikakve promjene.

## US-06 (F6)

Kao sef magacina, zelim da ponistim pogresno potvrdjen promet, kako bi stanje zaliha bilo tacno.

Kriterijumi prihvatanja:
 Ponistavanje potvrdjenog zapisa mijenja status u „Ponisten" i stanje se vraca na vrednost pre tog prometa.
 Ako bi ponistavanje dovelo do negativnog stanja (npr. primljeno 10, a izdato 8), operacija se odbija i stanje ostaje isto.
