# Kærbyvej 3 (3, 3A, 3B, 3C) + Kærbyvej 5, Låstrup, 8832 Skals – offentlige data

Indsamlet 21.9.2026 (ca. 15 min. tidsboks). Rå tal med kilde pr. datapunkt. Ingen ejer-/personoplysninger.
Blokeringer undervejs: boligsiden.dk, boliga.dk, edc.dk, colliers.com, vurderingsportalen.dk og boligportal.dk gav 403/"domain not allowed" både for WebFetch og i Chrome; dingeo.dk kunne åbnes, men cookie-overlay + script-blokering forhindrede udtræk af BBR-sektionerne. Resights (WebFetch) blev derfor hovedkilde til BBR/vurdering/salg.

## 1. DAWA – adresser, matrikel, koordinater (api.dataforsyningen.dk)

| Datapunkt | Værdi | Kilde |
|---|---|---|
| Adgangsadresse nr. 3 (id) | 0a3f5097-de78-32b8-e044-0003ba298018, "Kærbyvej 3, Låstrup, 8832 Skals", status 1, KVH 07910880___3 | https://api.dataforsyningen.dk/adgangsadresser/0a3f5097-de78-32b8-e044-0003ba298018 |
| Adresser på nr. 3 | 4 adresser, alle uden etage/dør: **3** (0a3f50c5-6e9d-32b8-e044-0003ba298018), **3A** (70d98383-0df3-1b8b-e044-00144f3ead67), **3B** (70d98383-0df4-…), **3C** (70d98383-0df5-…). 3A/3B/3C har egne adgangsadresser (7096f618-6d28/6d29/6d2a-5ed1-e044-00144f3ead67) på samme matrikel | https://api.dataforsyningen.dk/adresser?vejnavn=Kærbyvej&postnr=8832&struktur=flad |
| Matrikel | 6k, ejerlav **V. Låstrup By, Låstrup** (kode 760854) | samme |
| BFE / SFE | **3460203** | https://api.dataforsyningen.dk/jordstykker/760854/6k |
| Matrikelareal | **1.128 m²** (registreret), vejareal 0 m², beregningsmetode "k" | samme |
| Koordinater WGS84 (adgangspunkt) | lon 9,37679505 / lat 56,57491882, højde 3,2 m, nøjagtighed A | adgangsadresse-URL ovenfor |
| Koordinater UTM32 (EPSG:25832) | adgangspunkt **E 523149,77 / N 6270133,02**; vejpunkt E 523122,21 / N 6270133,17 | …/adgangsadresser/0a3f5097-de78-32b8-e044-0003ba298018?srid=25832 |
| Jordstykke bbox (WGS84) | 9,37649–9,37729 / 56,57458–56,57508; visuelt center 9,3767469 / 56,57492401 | jordstykke-URL |
| Sogn / kommune / region | Låstrup Sogn (8530) / Viborg (0791) / Region Midtjylland; landsdel Vestjylland (DK041); retskreds Retten i Viborg; afstemningsområde Skals | adgangsadresse-URL |
| Zone (DAWA-felt) | "Udfaset" (DAWA leverer ikke længere zone – se Plandata under pkt. 8) | samme |
| Kærbyvej 5 | adgangsadresse 0a3f5097-de7a-32b8-e044-0003ba298018; WGS84 9,37656522 / 56,57484375; matrikel **6ai**, samme ejerlav; **BFE 3460227**; areal **967 m²**, vejareal 0 | https://api.dataforsyningen.dk/jordstykker/760854/6ai |
| Naboer (til orientering) | nr. 1 = 6g (2.042 m², BFE 3460200); nr. 2 = 6n; nr. 4 = 6m (900 m²); nr. 6 = 6ae (1.357 m²) | jordstykker?ejerlavkode=760854 |

## 2. BBR – bygninger og enheder

Kilde: Resights (https://resights.dk/ejendom/kaerbyvej-3-lastrup-8832-skals/3460203) læst via WebFetch 21.9.2026. Tallene er Resights' gengivelse af BBR – bør verificeres i BBR/OIS.

| Datapunkt | Kærbyvej 3 | Kærbyvej 5 |
|---|---|---|
| Antal bygninger | 2 | 1 |
| Anvendelse (hovedbygning) | Etageboligbebyggelse / helårsbeboelse ("residential apartment building") | Carport |
| Opførelsesår | **1938** | 1980 |
| Om-/tilbygningsår | **2009** | – |
| Bebygget areal / samlet bygningsareal | **180 m²** | – |
| Udnyttet tagetage | **132 m²** | – |
| Etager | 1 + udnyttet tagetage | – |
| Samlet boligareal | **303 m²** fordelt på **3 boligenheder** | 0 |
| Enheder | 3 enheder registreret; adresser 3, 3A, 3B, 3C findes i DAWA – **m² pr. enhed ikke fundet** | – |
| Ydervæg | Mursten | Træ |
| Tag | Tagpap (hældning) | Andet materiale |
| Bebyggelsesprocent | 28 % | 3 % |
| Varmeinstallation / opvarmningsmiddel | **ikke fundet** | – |
| Energimærke | **ikke fundet** (sparenergi.dk-opslag returnerede 404; EMO-oversigt ikke nået) | – |
| Bevaringsværdi (SAVE) | **ikke fundet** | – |
| Grundareal | 1.128 m² | 967 m² |

Kilde nr. 5: https://resights.dk/ejendom/kaerbyvej-5-lastrup-8832-skals/3460227

## 3. Offentlig vurdering og ejendomsskat

| Datapunkt | Kærbyvej 3 | Kærbyvej 5 | Kilde |
|---|---|---|---|
| Ejendomsværdi (aktuel iflg. Resights, angivet "2025") | **1.800.000 kr.** | 140.000 kr. (Resights angiver dette som "bygning") | Resights-URL'er ovenfor |
| Grundværdi | **219.200 kr.** | 176.700 kr. | samme |
| "Foreløbig grundværdi 2025" (Resights' etiket) | 12.000 kr. | 11.000 kr. | samme – **usikkert**: beløbsstørrelsen ligner snarere foreløbig grundskyld end grundværdi; verificér på vurderingsportalen.dk |
| Ejendomsskat 2023 (ekskl. bidrag/gebyrer) | **4.510 kr.** | **3.828 kr.** | samme |
| Vurdering 2022 / 2024 (foreløbig), tidligere vurderinger, grundskyld 2024-26 | **ikke fundet** – vurderingsportalen.dk blokeret for både WebFetch og browser | – | – |

## 4. Salgshistorik

| Adresse | Dato | Pris | Type | Kilde |
|---|---|---|---|---|
| Kærbyvej 3 | **01.01.2013** | **1.380.000 kr.** | "Anden overdragelse" (ikke alm. fri handel) | https://resights.dk/ejendom/kaerbyvej-3-lastrup-8832-skals/3460203 |
| Kærbyvej 5 | 01.01.2013 | 1.380.000 kr. | "Anden overdragelse" | https://resights.dk/ejendom/kaerbyvej-5-lastrup-8832-skals/3460227 |

Bemærk: Samme dato og beløb på begge ejendomme tyder på én samlet overdragelse af begge matrikler (6k + 6ai) med beløbet registreret på begge. Nøgletal hvis 1,38 mio. dækker begge: 1.380.000 / 303 m² bolig = **4.554 kr./m²** (2013). Ældre tinglyste handler: **ikke fundet** (boligsiden/boliga blokeret).

## 5. Sammenlignelige udlejningsejendomme (Skals/Viborg-området)

| Adresse | Type | Lejemål / m² | Pris | Leje/år | Drift/år | Afkast | Kr./m² | Status | Kilde |
|---|---|---|---|---|---|---|---|---|---|
| Hovedgaden 44A, 8832 Skals | Boligudlejning, opført 1913, renoveret 2011, grund 366 m² | 6 lejemål / 482 m² | **3.995.000 kr.** (udbudspris) | ikke fundet | ikke fundet | ikke fundet | 8.289 kr./m² | **Solgt** (EDC-annonce markeret solgt; salgsdato/-pris ikke fundet) | https://www.edc.dk/erhverv/erhvervsejendomme/boligudlejningsejendom/8832-skals/hovedgaden-44a/75100563/ (via søgeresultat – siden blokerer fetch) |
| Gl. Skolevej 15, 8832 Skals | Boligudlejning, opført 1909, delvis renoveret 2015/16, energimærke C, grund 915 m², 100 m fra skole | 2 lejemål: 93 + 171 m² (=264 m²; Ejendomstorvet angiver dog 153 m² boligareal) | **1.395.000 kr.** | **151.200 kr.** | **52.250 kr.** | **7,3 %** | 5.284 kr./m² (264 m²) / 9.117 kr./m² (153 m², Ejendomstorvets tal) | Til salg (EDC sag 75100497); offentlig vurdering 1,45 mio. kr. | https://www.ejendomstorvet.dk/investering/vestjylland/viborg/boligudlejning/3c328920-d33f-4290-a1b6-76b3f87a58a8 |
| Koldingvej 100, 8800 Viborg | Boligudlejning, opført 1924, energimærke E, grund 1.123 m², 4 p-pladser | 2 lejemål: 84 + 65 m² (=149 m²) + 84 m² kælder | **1.695.000 kr.** | **149.988 kr.** | **43.931 kr.** | **6,39 %** | 11.376 kr./m² | Til salg (EDC sag 751006747) | https://www.edc.dk/erhverv/erhvervsejendomme/boligudlejningsejendom/8800-viborg/koldingvej-100/751006747/ (via søgeresultat) |
| Randersvej, 8800 Viborg | Bolig- + erhvervslejemål (rød mursten; bolig 137 m² + kælder) | 2 lejemål / 233 m² | 1.475.000 kr. | ikke fundet | – | ikke fundet | 6.329 kr./m² | Til salg (Plus Mæglerne) | https://www.lokaleportalen.dk/salg/boligudlejningsejendomme/viborg |
| Øvrige Viborg-udbud (Lokaleportalen, 8 annoncer, adresser ikke vist) | Boligudlejning | 150 m² 2.100.000 kr. (14.000 kr./m²); 265 m² 4.100.000 (15.472); 275 m² 3.250.000 (11.818); 345 m² 6.700.000 (19.420); 590 m² 8.300.000 (14.068); 2.125 m² 31.150.000 (14.659); 4.505 m² 70.500.000 (15.638). Gns. 15.020 kr./m² | | | | | | Til salg | samme |
| Region Midtjylland samlet | 349 boligudlejningsejendomme udbudt, gns. pris 11.358.922 kr., gns. 12.862 kr./m² | | | | | | | | https://www.boligudlejningsejendom.dk/region-midtjylland |

Afkastniveau:
- Investejendomme.dk (søgeresultat-uddrag): investeringsejendomme i Viborg Kommune udbydes med **1.-års afkast ca. 5,83–8,4 %** (https://www.investejendomme.dk/region-midtjylland).
- Konkrete udbud ovenfor: **6,39 % (Viborg by, 2 lejemål)** og **7,3 % (Skals, 2 lejemål)**.
- EDC Erhverv (2026-forventninger): høj investorinteresse forventes at presse afkastkrav ned i de største byer; OMK-ejendomme mere selektiv efterspørgsel (https://www.edc.dk/erhverv/nyheder/cityfact-hvad-driver-efterspoergslen-paa-boligudlejningsejendomme/ og https://kampagne.edc.dk/forventninger2026/ – kun kvalitativt; taltabeller ligger i rapport-PDF, som ikke kunne hentes).
- Nordicals City Foresight Randers: afkastkrav prime/sekundær + markedsleje findes kun som interaktive grafer, ikke udtrækbare (https://nordicals.dk/foresight/city-foresight/randers-cityforesight/).
- **Ikke fundet**: Colliers/EDC-markedsrapporternes konkrete afkastkravs-tabeller (403), tinglyste salg af flerfamiliehuse i Løgstrup/Møldrup/Ulbjerg/Bjerringbro seneste 3 år (boligsiden/boliga blokeret).

## 6. Lejeniveau i 8832 Skals (aktuelle annoncer, sept. 2026)

| Vej | Type | m² | Vær. | Kr./md. | Kr./m²/år | Kilde |
|---|---|---|---|---|---|---|
| Hovedgaden | Lejlighed | 64 | 3 | 4.995 | 937 | https://boligzonen.dk/lejebolig/skals |
| Hovedgaden | Lejlighed | 79 | 2 | 4.995 | 759 | samme |
| Hovedgaden | Lejlighed | 118 | 4 | 6.000 | 610 | https://www.lejebolig.dk/lejeboliger/skals |
| Ejstrupvej | Lejlighed | 78 | 2 | 4.600 | 708 | samme |
| Ejstrupvej | Lejlighed | 113 | 3 | 5.300 | 563 | samme |
| Tværvej | Lejlighed | 99 | 3 | 7.862 | 953 | boligzonen / akutbolig (https://www.akutbolig.dk/skals) |
| Gl. Fjordvej | Hus/rækkehus | 60 | 2 | 5.295 | 1.059 | samme |
| Skovvej | Hus | 220 | 5 | 11.500 | 627 | boligzonen |
| (EDC Lejeindeks) | Lejlighed | 61 | 2 | 4.500 | 885 | https://www.edc.dk/lejebolig/8832-skals/ (via søgeresultat) |
| (EDC Lejeindeks) | Lejlighed | 76 | 2 | 4.700 | 742 | samme |
| (EDC Lejeindeks) | Lejlighed | 33 | 1 | 2.064 | 751 | samme |

Spænd for lejligheder i Skals: **ca. 560–950 kr./m²/år**, typisk **700–900 kr./m²/år** for 60–80 m². EDC angiver 15 boliger til leje i 8832 (11 lejligheder, 5 villaer). Ingen annoncer fundet i selve Låstrup.

## 7. Markedsstatistik – Finans Danmark BM010, parcel-/rækkehuse, Viborg Kommune (realiseret handelspris, kr./m²)

| Kvartal | Kr./m² | Kilde |
|---|---|---|
| 2026K2 | **10.458** | oplyst i opgaven (fra tidligere opslag) – ikke genverificeret i dag (rkr.statistikbank.dk har intet JSON-API; formular-POST gav intet resultat) |
| 2024K3 | 10.673 (op 7 % fra 9.973 i 2024K2); landsgns. 16.713 | https://voresbyviborg.dk/a/huspriserne-gaar-op-i-viborg-kommune/5f01adf0-b0d4-4a7d-a5a2-3ef7be690272 (Finans Danmark/Boliga) |
| 2023K3 | 10.331 (ned 2,3 % fra 10.578 i 2023K2); landsgns. 16.227 | https://voresbyviborg.dk/a/huspriserne-gaar-ned-i-viborg-kommune/4d4382b2-3779-4a7b-827d-5e6bbcb7d677 |
| Tendens 2025K2→2026K2 | Bolius (18.9.2026): huspriser **faldet** i Viborg Kommune det seneste år, mod +9 % på landsplan | https://www.bolius.dk/se-huspriserne-i-din-kommune-siden-1992-20536 |

Tabellen BM010 bekræftet at findes med variabler OMRÅDE=791 (Viborg), EJENDOMSKATEGORI=1 (Parcel-/rækkehus), TAL=REAL, Tid op til 2026K2: https://rkr.statistikbank.dk/statbank5a/SelectVarVal/Define.asp?MainTable=BM010&PLanguage=0
**Ikke fundet**: de seneste 4 kvartaler (2025K3–2026K2) som serie, og postnummer 8832 (tabel BM011).

## 8. Område og planforhold

| Datapunkt | Værdi | Kilde |
|---|---|---|
| Låstrup | landsby, **ca. 200 indb.** (202 i byområdet 2011); ved Simested Å med udsigt over Hjarbæk Fjord; **3 km til Skals** (vej + cykelsti); **bus 67, ca. 22 min. til Viborg**; Kulturcenter Værestedet (gl. skole) m. fitness/internetcafé; del af Fjordklyngen (Låstrup, Nr. Rind, Skals, Skringstrup, Sundstrup, Ulbjerg) | https://fjordklyngen.dk/byerne/lastrup ; https://da.wikipedia.org/wiki/L%C3%A5strup |
| Skals | **1.748 indb. (2026)**; **13 km nord for Viborg**, 11 km SV for Møldrup, 18 km S for Aalestrup; Skals Skole (folkeskole, **321 elever**), Skals Efterskele, Skals Håndarbejdsskole (højskole, 1959); butikker, bager, læge, tandlæge; hal/multihal, svømmehal, skyttecenter, fitness; jernbane nedlagt (persontrafik 1959) → Himmerlandsstien (cykel/vandre) 2006 | https://da.wikipedia.org/wiki/Skals ; https://viborg.dk/om-kommunen/byer-og-landsbyer/skals/ ; https://www.dingeo.dk/kommune/viborg/skole/skals-skole |
| Viborg Kommune | 97.892 indb. (ultimo 2025, +265) | https://viborg.dk/om-kommunen/fakta-og-noegletal/rundt-om-viborg-kommune/ |
| Trafikstøj | Ingen registreret trafikstøj (vej/bane/lufthavn) på Kærbyvej 3 (Miljøstyrelsen 2022) | https://www.dingeo.dk/adresse/8832-skals/k%C3%A6rbyvej-3/ |
| Kommuneplanramme (Plandata WFS) | **LÅST.C2.01 "Låstrup Blandet bolig og erhverv"**, plantype 10.1, anvendelse generel: Blandet bolig og erhverv (anv.spec 2120), **bebyggelsesprocent 40**, max bygningshøjde 8,5 m, **max 1,5 etager**, vedtaget/ikraft **21.05.2025**; dokument: https://dokument.plandata.dk/11_11335193_1788347817391.pdf | https://geoserver.plandata.dk/geoserver/wfs?…typeName=pdk:theme_pdk_kommuneplanramme_vedtaget_v&bbox=523140,6270120,523160,6270140,EPSG:25832 |
| Lokalplan | Ingen vedtaget eller foreslået lokalplan returneret for punktet (WFS-lag svarede tomt/fejl – **ubekræftet**) | samme WFS, lag theme_pdk_lokalplan_vedtaget_v / _forslag_v |
| Zonestatus | **Ikke fundet** (zonekort-laget returnerede tomt; DAWA-feltet er udfaset). Låstrup er en afgrænset landsby med kommuneplanramme – formentlig landzone, skal bekræftes |

## 9. Skråfoto

https://skraafoto.dataforsyningen.dk/?center=523150,6270133&orientation=north
(UTM32 adgangspunkt for Kærbyvej 3; Kærbyvej 5 ligger ca. 15 m sydvest herfor)

## 10. Ikke fundet / udestående

- BBR-enhedsliste: m², værelser, køkken/bad for hver af enhederne 3/3A/3B/3C (kun samlet 303 m² / 3 enheder – bemærk 4 adresser vs. 3 enheder).
- Varmeinstallation og opvarmningsmiddel; energimærke (EMO); bevaringsværdi.
- Vurderingsportalen: 2022-/2024-vurdering (foreløbig), historiske vurderinger, grundskyld 2024-2026.
- Tinglyste handler før 2013 og evt. ejerskifte-detaljer; boligsiden.dk/boliga.dk/dingeo BBR-sektioner (blokeret).
- Solgte flerfamiliehuse i Skals/Løgstrup/Møldrup/Ulbjerg/Bjerringbro med faktiske salgspriser (kun udbudspris for Hovedgaden 44A).
- Konkrete afkastkravstabeller fra EDC Market Update Q1/Q2 2026, Colliers markedsrapport, Nordicals (PDF/interaktive grafer bag 403).
- Finans Danmark BM010 serie 2025K3–2026K1 og postnr.-tal (BM011) for 8832.
- Zonestatus og evt. lokalplan bekræftet via Plandata.
