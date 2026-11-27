# M490K · Input Pre Amps

Ward-Beck Systems M490K, 1983|16. Wiki page: [M490K on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M490K.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 24 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 11 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 5 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 205 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 0 |
| [SOFTWARE/](SOFTWARE/) | program listings, firmware, the plugin | 0 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 7 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 34 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [1 topic](FORUM.md): what owners and technicians said about it.

## Specifications

From the technical data sheet: [1983 - M490K - Line Input Module (2).pdf](MANUALS/1983%20-%20M490K%20-%20Line%20Input%20Module%20(2).pdf) page 3 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Sourc** | e Impedance: 600 ohms, ba lanced/unbal an ced. |
| **Input impedance** |  |
| &nbsp;&nbsp;Output impedances | 30,000 oh m&quot;, balanced (Pr&quot;O!ilr am cin;u ll &quot;). 60,000 oh m&quot;, balanced leue ci n;u il s). 1,000 ohm&quot;, balanced (po SI di r ecl). |
| &nbsp;&nbsp;Output level | o dBm nominal, +24 dBm ma&quot; imum. (eq u iva lent vol lage 600 ohm,,). |
| **Phasing** | Input and o u tp u l te,.mln al s de signaled by numbers a,.e in phase, Q&quot; low e&quot; number of numb er-e d p a i,. Is in phase wll h lower numbe&quot; of Olh e,. numbe,.ed pair. |
| **Logic** | Input Level,,: t re &lt;&gt;pe,.ale CH ON, CH OFF I;, CUE). |
| &nbsp;&nbsp;Logic | 0: 0 10 +13 vol l&quot;. |
| &nbsp;&nbsp;Logic | 1: +16 10 +24 vens, |

## Circuit description

From [1983 - M490K - Line Input Module (2).pdf](MANUALS/1983%20-%20M490K%20-%20Line%20Input%20Module%20(2).pdf) pages 5-10 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

The M490K provides complete I&quot;emote lIne input f.c ili ties, as requ i~d fOI&quot; • m i.. ing &lt;;Onsale. Included.... source se lec lo l&quot;, pl&quot;OSll&quot;. m bus ass lg nmen l. swell. s the ch. nn e l ml.. l n g allen uatOl&quot;.

Input.nd P l&quot;e.. m~

Th a mu&quot;,a lly inter locked INPUT SELECTOR switches SWI and SW2 allow I hes election of one oft wo available lines our ce s. An add i t io n.. 1 con l. c t iss u p plied on each switCh for control purposes. The resi stive ne l works Rl_R8, RI54.. n d R1SS present e 600 on m input Impedance to Ih eli n e sources.

The $l!!Cond.ry of TI i s &lt;;Onn ec ted tot he pre.. mplif ie r cons l sling of Ql t h.-ou g h Q7 and Zl. Input sensi tlvl lY oft he module m.. y b e v.. r-ie d b y.djuS lmen t oft he SENSITIVITY co. H ro l R2S, cov.... ing • range of 30 d B. The b.. l.. oee e p..e e mp l ifi e.. OUlpU I.. pp e.. r s.. t module conn e&lt;:to.. P2, pins 6 /F.

Two se.. te s-ccooec rec, bela nced in se.. t points e r-e m.. de av.l l able e t P2, pins 6/F, 8!J, S!E.. nd 7!H, ope.... ting. 1 a nomin.. ' level of o dBm. They.. llow the l n$l!!.. ti ono f.. ncill a.. y processing equip men l InlO them i.. lng channel sIgnal pa lh suCh a s.. com p..essee-, equalizer 01&quot; filler. The provision oft wo se.. ies con ne&lt;:lor in$l!!&quot; 1 points perm il s I he u tlliz a l lon of l he module ins tereo systems such.. s the was model Rl200!R2000 consoles. Int he se.nd s i mi I......pp ll c.. tion s, the functions a s $QClated with the lef land r lg hl In$l!!rt ion Se le&lt;:tor s I M499) may bolh be ins e.. ted into the channel, with Ih e left channel In a.... 1 function p..eced ing the.. i ght Channel lunCllon.

FI&quot;OI'I'l the Inse.. t points, Ihe sign. 1 i s routed ' 0 ATTI,.. balanced slide att en u.. to.. reeru.. l n g a conli nu ou s mi.. l...g r.... ge of more Ih.. n

70 d B p.. io.. 10 cutoff. The CUE ch.... ne l feed I. laken f l&quot;Ol'l'l lhe inpul

side oft he.. ll enU.. lor.

M490K LINE iNPUT MOOUL E

Program Channel Switch.

Z 2 i s a CMOS analogs witch, serving as thea clive switching element of the PROGRAM channel. The control volt llge to operate Z2 I s derived from the logic circuitry within the module and i s coupled to ZI via CR1. to switch the channel ON, this control voltage I sIn the order o f 10 volts. When the control volt llge drops to 0 volts, the s w il c h will b e OFF, resulting ina signal allenu ation of more than 100 dB.

Following Z2, integrated c irc u its Z3 and Z4 amplify thea u d ios i g n alto a nominal level o f 0 dBm (equiv al ent volt ag e). From the amplifier output, the signal is routed tot h e PROGRAM ASSIGN switches SW4 and SW5 via PANs witch SW3 and PAN Control R65 to R6B.

Both PROGRAM outputs Plan d P 2 are designed to feed into stereo buses and each i s divided into a left and aright output. Op e r lltion of ASSIGNMENT SWITCHES SW4 or SWS will result ins i mu l ta neo us assign m&quot; n t to both I&quot; f tan d right channels oft heap prop r ia t&quot; mixing buses. With the atd oft h ePA N control, th&quot; signal distribution between the left and right output buses c &quot;n be continuously &quot;djus t&quot;d.

The CUEs i g n a l origin &quot; tes from abridging takeoff a t the Input of th &quot; slide a tt en ua tor. Owing to th &quot; high Input Impedance of the CUE channel, its operation has noe ffee ton the main PROGRAM channel. ZS r&quot; presents th &quot; audio switCh fort he CUE channel. Similarly to Z2. the control voltage for Z 5 i s generated int h e logic circuitry &quot;5 described further on. The output of Z5 is followed by t h &quot; booster amplifier Z6, whteh in turn feeds the cue bus mixing network RIO I throug hR I04.

Post Direct Output

The output of booster amplifier Z 3 _Z4 i s taken before the PANs witch

and routed to the POST DIRECT output a t PI _ZO,ZI. The output level

i s 0 dBm (vo l tag e r,,: 600 ohms) under nominal conditions.

M49Ol(LINE INPUT MODULE

F oldba c:k Ouipui s

The FQl.D8ACI(outpul&amp;. like Ihe POST DIRECT OUIP UI, er-e l a ken fl&quot;Otn l he eeeer ee amplifier OUtp u l via level c:onlt'Ols RISO_R ISI (FBI I.. nd R1S2_R 1SJ (F B2 1. FBI and FB2 e ppee r.. I c:onnK tOl' PI _ Il,12.. nd P I _13, 14 r-espec:ti vely.

The c:onlrol lIo llages required 10 operate Ihe PROGRAMs wit c:h l2 end the CUEs wit c:h lS.. regenerated with the aid of logic: c:1..c:ui l.. y utilizing int eg.. ate d c:ircuit s l 7 through l10.

lS Is CMOS dual flip _fl ops e r ll ing as a 1.. Ic:h tome ln l e ln the status o f l2 end lS, once they h &quot; v e been set toe i the.. the ONo r the OFF position.

A number of indill idua l Input f unc:tions go ve..n the s t e I US oft h e du.. 1 flip_flop lS. A de s c:riptlon of eac:h input funC:l ion follows:

When power is ln l t l.. l l y.. pplled tot hes y stem. Ihe comb lna llen of CR 9, CR to, CRI I and C40 will pull down both..d e.... &quot; Inputs of ZS until C40 is fully c:h....ged. thuS ensu.. ing Ih al s w h cnes l 2 and lS ar-e int h e OFF posit ion.

Channel ON

Momentary op e r.. ll on of the CIiAN NEL ON s w i lc:n SW9 will p..o(h ••ce a nll'g.. rave going pulse at z a, pin 2 and &quot; p.. eset&quot; Ihe Asect ion of lS. Alle,..&quot;ali v el y,.. momentary ground do su..e of the EXTERNAL CHANNEL ON c:ontrol input at P2, pin N will &quot;es ull int h e same condItion.

Onc:e the flip flop i s &quot;p..e set&quot;, its OUl put Isp in 15 changes from 0 10 1 (approxlmalely 10 lIolls).

Tni swill c:au set heP ROGRAM s wit c n l 2 10 s wll e nON. Fu.. lhe..

more, QI2 will sat u rate re su lling int he CHANNEL ON indiea to.. lamp OS3 10 s wit e non. With Q12 saturated, the &quot;c:on trot

eommon &quot; pOle nt l ala p p e.... sat the em l l1e r s of QI3 and Q14.

Apo sitiv e base potential i s applied to etth e.. 013 and 0 14, depending on whel her INPUT SELECTORs wi l Ch SWI or SWZ i s depressed. Effectively, 01 3 end 0 14 operates i mil a.. ly 10 two AND g.. les. The colleclors oft h e Iw o tr.. n ststc.. s rep r e sen l the outputs o f the AND 9 ales.

They e Ppe.... a t PZ, pin 13 and P. These terminals a..e cape ble of sinK ing a m.. ximum current of 40 mA each f..om a 24 volt SOuN:e and me y b e used fo.. mUling purposes.

When op e r.. ting me CHANNEL ON swilCh SW9, a sep e r-e l eco n t ac i i s closed, e ce e sstet e a l PZ, pin &quot; 15/5. This cont acl me y b e used for control or sign e llng p u..po ses.

Pin R of P2 i s isolated t h..ough diode CR3. When connecl ed i n per all el with Ihe same ou tpul of o th e.. modules, i t provides 8conv en i en tOR get e config u..a ti on, suit able 10.. esel e common li me.. e.. c h lime a CHANNEL ON button i s d ep..e ssed.

Moment.... y op er&quot;tion oft he CHANNEL OFF swi l ch swe or mom enl e r-y g..ound c1osu..e of the EXTERNAL CHANNEL OFF conlrol inpul a t PZ, pin 12 will result ina negative going pulse.. I za, pin 3.. nd &quot;cl ear &quot; I h e A_s ection of ze, producing o volts a t ze, pin I S. Con sequen lly, Z 2 will swilCh OFF, Q1Z wills top conducting, causing 053 10 e &quot; ting u i sh, and Ihe muting control oulpu ts e I P2, pins 13 and P will b e disabled.

A se pa.. ate conlac t i s a v.. ilable On swe end is accessible et PZ, pins 17jU. I I me y b e used for &quot;m a chin e &quot; lOp &quot;.

A sep a.. ale CHANNEL OFF tally lamp is built into 51'18 and is connected to PZ, p,n s 18/ V.

Thea eec uce o f Z8 i s used to control the solids tate cue switch ZS. The flip-f lop will change state each time..

negative going I r.. n silion lakes place e t pin 6 o f Z8. Con se

qu en tly, with each inpu l pulse, the CUE c h.. nnel will ane r -. n.. te between ON and OFF.

Tnl s cn ang e of ' Ia le can be brough l about by anyone of three different melhods:

a) Mom e n l ary operation of I h e CUEs...i lCh SW12 (0). bl Momenlary ground clo,u~ oft h e EXTERNAL CUE Inpul atP 2, pin 11.

c) Opera lloro of lhe &quot;overpre• • &quot;.... i ICh SW11, located. Ii d e allet'luatOf'&quot; beyond the &quot; Infi ni te&quot; posi lion.

Tha OW Sl a i U. of the CUE Channel is ind ica led by DS2,... hich Is driven by 01 1.

Ana d di l io nal feature ensures that I h e CUE channel willa l ways switch to OFF when ever Ih e lIt ide e uen ue rc rIII moved onto Of'&quot; away from the &quot; Infinite &quot; position, regard less 0 1 Its prior Sla le. The controls i g na l forth i saC lion is initiated b y Ih e chan g&quot; of Sla leo f I heAT TENUATQR CUTs wil c h SW10. There sultan l level chan ge, being e i lher p o s l live Of'&quot; neg all ve going. i s proce. sed I h rough 27.29 and 2 10. The OUlpul produced '&quot; pin 4 o r 21 0 will always be a negal lve goIng pulse o f approx lmalely 500 milliseconds duration. CR1 2 passes thIs puille 10 28, pin 8, thereby &quot; c l&quot; a ri n 5l&quot; l he esec uco of the flip _flOP. and resul ling In pin 1 1 of 28 to lIwi tch 10 Ieeremain at) 0 vollS, i n l urns w l l chin g lhe CUEs witch 25 to

All logic con l r o l i npulS are buffered to guard a Slain st spurious noise and switch bounce.

Power Supply Decoupllns

Po...e r supply dec ouplin 51 is provided b y R146 10 RUg and C50 10 CSJ. CR I 6 and CR I 7 s eve 10 pre v et'lt amplifier damage Int h e ev..... t of supply vol lag &quot; rever s.al. The decoupli ng network drops the +/-25 volt supply rail. 10 a nomInal vo llage o f +/ _ 18 veu s • QI5 dec ou p les and fi lt&quot;r s Ihe posit i v e.up ply rail. resu lling Ina n

OUlpul o f +12 vol lS 10 operate I h e CMOS c lr-cullry. In addllon, 2J

and 2 4 are fur the r decoupled by R54, RS5, C21 and C 22.

**M. 9OK LINE INPUT MQOULE**

DESCRIPTION MFG PART NUMBER

All enu lI lor, c /w eeee ee re e I 5SO!AH3 S! 100

ct C Il P ~ clIO &quot; 0.01 of &quot;'110 1&lt;;0 C0 92Mel 03M ca 560 p F Philips 222 2_6 30 _0 3 56 1 CJ 47p F 2222-638-70479 4.7 u F/2S V

C5 4.7 u F/ 25 V Kemel 1 39OC475 M025A5

CO 2.2 pF Philips 2222-638-03228 C1 3.9 p F 2222_638--09398 C8 150 uF / 6 V Kernel T39OE157MOO6AS C, 10 u F/ 25 V 139OC 106,&quot;,0251&lt;5 C&gt;O 220 uF /10 V T J9OF227M0 1Q.\S

en 150 pF Philips 2222 _638_70151 CO2 4.7pF 2222-638-09478 m 220 u f /lO V K_, T39Of227M010AS W 4.1 uf /lO V T390847SMOIOAS cis • • 7 u F flO V

ere 0.33 u F/15 V T390AJJ4MOJ5AS W 10 uF / 25 V T3 9OC1Q6MOZ5AS C&gt;8 10 uF /2 5 V cis 10pF Philips C20 10 pF

ca 47 u F/25 V 4Z6 E TF 4 7 C22 47 u Ft25 V C2J 33 u F ! I O V cas 33 u F{ to V C25 6800 pF

C&quot; 2.2 uF / 2S V K_, T39OB225M025AS C21 4.7 uF jlO V T390B47SMOIOAS C28 '.7 u F flO V C29 6.8 uF / 16 V T3908685MOI6AS

CJO 6.8 uF j 16 V

CJ&lt; 4.7 uF /l O V

CJ2 4.7 u F/ to V

</details>

<!-- /module data -->

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVWhFR0szbEE4bU0/view?resourcekey=0-mj2MnpAcSmAIQ2825q1xWQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVWhFR0szbEE4bU0&resourcekey=0-mj2MnpAcSmAIQ2825q1xWQ" width="240" alt="1983 - M490K - 490-04-022 - CHANNEI ELONALE EIRORKE IHE APOROORLALE POM PURE.jpg"></a><br><sub>1983|16 · 490-04-022 - CHANNEI ELONALE EIRORKE IHE APOROORLALE POM PURE · <a href="MECHANICAL/1983%20-%20M490K%20-%20490-04-022%20-%20CHANNEI%20ELONALE%20EIRORKE%20IHE%20APOROORLALE%20POM%20PURE%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQkVvNk9NaUtnYWs/view?resourcekey=0-Gb10E8nYeg506UM1PBCVgQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQkVvNk9NaUtnYWs&resourcekey=0-Gb10E8nYeg506UM1PBCVgQ" width="240" alt="1983 - M490K - 490-04-022 - WAIUR THLE LICH EII ALO IURN CUE OFP.jpg"></a><br><sub>1983|16 · 490-04-022 - WAIUR THLE LICH EII ALO IURN CUE OFP · <a href="MECHANICAL/1983%20-%20M490K%20-%20490-04-022%20-%20WAIUR%20THLE%20LICH%20EII%20ALO%20IURN%20CUE%20OFP%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/1n4IYRzv2ttWsj_-qGcmytb_fwK4rxAr6/view" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=1n4IYRzv2ttWsj_-qGcmytb_fwK4rxAr6" width="240" alt="19xx - M490K - DOC - 490-03-033 - SCRATCHES LSE SELF-CLINCHING PEM FASTERNER.jpg"></a><br><sub>19xx - M490K - DOC - 490-03-033 - SCRATCHES LSE SELF-CLINCHING PEM FASTERNER</sub></td></tr>
</table>

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbmVmQ0lhcDlHZ3c/view?resourcekey=0-AUirLfzEDxvtyqOu6e7QuA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbmVmQ0lhcDlHZ3c&resourcekey=0-AUirLfzEDxvtyqOu6e7QuA" width="240" alt="1983 - M490K - 490-01-011 - ENG SCLIBENT LINE INPUT MODULE.jpg"></a><br><sub>1983|16 · 490-01-011 - ENG SCLIBENT LINE INPUT MODULE · <a href="SCHEMATICS/1983%20-%20M490K%20-%20490-01-011%20-%20ENG%20SCLIBENT%20LINE%20INPUT%20MODULE%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSFRlOHdmWG0ycG8/view?resourcekey=0-y7bxRNkXxZmaLp1kvJ0bsQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSFRlOHdmWG0ycG8&resourcekey=0-y7bxRNkXxZmaLp1kvJ0bsQ" width="240" alt="1983 - M490K - 490-01-011 - OFF ONISTART TIMER RESET OFF TALLY OFF STOP.jpg"></a><br><sub>1983|16 · 490-01-011 - OFF ONISTART TIMER RESET OFF TALLY OFF STOP · <a href="SCHEMATICS/1983%20-%20M490K%20-%20490-01-011%20-%20OFF%20ONISTART%20TIMER%20RESET%20OFF%20TALLY%20OFF%20STOP%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdXRPaVp0dlB3N0E/view?resourcekey=0-XyXv7T6BH-5sKtF-_M-7Lw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdXRPaVp0dlB3N0E&resourcekey=0-XyXv7T6BH-5sKtF-_M-7Lw" width="240" alt="1983 - M490K - 490-02-011 - ASSIGH HIZLD SSIIO CZO RCE.jpg"></a><br><sub>1983|16 · 490-02-011 - ASSIGH HIZLD SSIIO CZO RCE · <a href="SCHEMATICS/1983%20-%20M490K%20-%20490-02-011%20-%20ASSIGH%20HIZLD%20SSIIO%20CZO%20RCE%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNFlQRlpfVW1QNHM/view?resourcekey=0-kyoRlHY4DG-9QC9Ee0-63g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNFlQRlpfVW1QNHM&resourcekey=0-kyoRlHY4DG-9QC9Ee0-63g" width="240" alt="1983 - M490K - 490-02-011 - CMON CUE JOR.jpg"></a><br><sub>1983|16 · 490-02-011 - CMON CUE JOR · <a href="SCHEMATICS/1983%20-%20M490K%20-%20490-02-011%20-%20CMON%20CUE%20JOR%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcDFqX0xJd2l1akE/view?resourcekey=0-Qq1MLuGrLzosuYdmnMwEZg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcDFqX0xJd2l1akE&resourcekey=0-Qq1MLuGrLzosuYdmnMwEZg" width="240" alt="1983 - M490K - 490-06-021 - WED LACX OOTED.jpg"></a><br><sub>1983|16 · 490-06-021 - WED LACX OOTED · <a href="SCHEMATICS/1983%20-%20M490K%20-%20490-06-021%20-%20WED%20LACX%20OOTED%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOWhUVl9uRnludDg/view?resourcekey=0-1Kw86Q3CRvXk2H9piIqt-g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOWhUVl9uRnludDg&resourcekey=0-1Kw86Q3CRvXk2H9piIqt-g" width="240" alt="1983 - M490K - 490-06-021.jpg"></a><br><sub>1983|16 · 490-06-021 · <a href="SCHEMATICS/1983%20-%20M490K%20-%20490-06-021%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

Not on Google Drive yet: `M490K - RTO-144 Connections.pdf`

## RTO-144 pinout

20 contacts (P1), 21 contacts (P2). Every contact, with where it was read: [`RTO.json`](RTO.json).

| Pin | Signal | Kind | Pair | Confidence |
|---|---|---|---|---|
| 1 | LEFT PGRM 1 | audio | A3 + | high |
| 1 | MIC IN A | in | A1 + | high |
| 2 | LEFT PGRM 1 | audio | A3 - | high |
| 3 | RIGHT PGRM 1 | audio | A4 + | high |
| 3 | MIC IN B | in | A2 + | high |
| 4 | RIGHT PGRM 1 | audio | A4 - | high |
| 4 |  | unread |  | low |
| 6 | INSERT SEND | out | B1 + | high |
| 7 | INSERT RETURN | in | B2 + | high |
| 13 |  | unread |  | low |
| 13 | -25V | power |  | low |
| 17 |  | unread |  | low |
| 19 | -25 V | power |  | high |
| 20 | POST DIRECT OUTPUT | out |  | low |
| 20 | COMMON | ground |  | high |
| 21 | +25 V | power |  | high |
| A | MIC IN A | in | A1 - | high |
| C | MIC IN B | in | A2 - | high |
| F | INSERT SEND | out | B1 - | high |
| H | INSERT RETURN | in | B2 - | high |
| R |  | unread |  | low |
| Y |  | unread |  | low |

**Straps:** Insert: JMP.6.7 · Insert: JMP.F.H

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOTl1VXNxaGZYRTA/view?resourcekey=0-t1al9tdU_Ckv4PamO0zakQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOTl1VXNxaGZYRTA&resourcekey=0-t1al9tdU_Ckv4PamO0zakQ" width="240" alt="1983 - M490K - Line Input Module (2).pdf"></a><br><sub>1983|16 · Line Input Module (2)</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZmpyU0JobFNsNDA/view?resourcekey=0-mNBNdd_o5ru7_rcsVIGfUw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZmpyU0JobFNsNDA&resourcekey=0-mNBNdd_o5ru7_rcsVIGfUw" width="240" alt="1983 - M490K - Line Input Module.pdf"></a><br><sub>1983|16 · Line Input Module</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZ2l1YWFaMXVzYzA/view?resourcekey=0-Gzzd792_ieNJIbyIXVyGog" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZ2l1YWFaMXVzYzA&resourcekey=0-Gzzd792_ieNJIbyIXVyGog" width="240" alt="1983 - M490K - P001 - Title Page.jpg"></a><br><sub>1983|16 · P001 - Title Page</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTERvY3JsU18tYXM/view?resourcekey=0-LaODLYNUwk4t8nlMrTttiw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTERvY3JsU18tYXM&resourcekey=0-LaODLYNUwk4t8nlMrTttiw" width="240" alt="1983 - M490K - P002.jpg"></a><br><sub>1983|16 · P002</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRl8wSG54WWllajg/view?resourcekey=0-bZtXmEYrJDXflyLjST9TGw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRl8wSG54WWllajg&resourcekey=0-bZtXmEYrJDXflyLjST9TGw" width="240" alt="1983 - M490K - P003 - 1-1.jpg"></a><br><sub>1983|16 · P003 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSm5EeVRHdXpnUGM/view?resourcekey=0-nUVLdXr90p8sfjr78q0X4Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSm5EeVRHdXpnUGM&resourcekey=0-nUVLdXr90p8sfjr78q0X4Q" width="240" alt="1983 - M490K - P004 - 1-2.jpg"></a><br><sub>1983|16 · P004 - 1-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZWdIdnJjSXdPbm8/view?resourcekey=0-LXWt7xG9iODPhtmKa69Qtw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZWdIdnJjSXdPbm8&resourcekey=0-LXWt7xG9iODPhtmKa69Qtw" width="240" alt="1983 - M490K - P005 - 2-1.jpg"></a><br><sub>1983|16 · P005 - 2-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKakFiYUZ4VXdIQTg/view?resourcekey=0-G8H6ODJLxZNjw7kjohvcQA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKakFiYUZ4VXdIQTg&resourcekey=0-G8H6ODJLxZNjw7kjohvcQA" width="240" alt="1983 - M490K - P006 - 2-2.jpg"></a><br><sub>1983|16 · P006 - 2-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVUhfcUVsSWI0YlU/view?resourcekey=0-IOd9WX_nbV5Lalrc1vFuRg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVUhfcUVsSWI0YlU&resourcekey=0-IOd9WX_nbV5Lalrc1vFuRg" width="240" alt="1983 - M490K - P007 - 2-3.jpg"></a><br><sub>1983|16 · P007 - 2-3</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQnFpd09yNUZMN0E/view?resourcekey=0-ta1OUhcMnWrI5WPXd_egcA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQnFpd09yNUZMN0E&resourcekey=0-ta1OUhcMnWrI5WPXd_egcA" width="240" alt="1983 - M490K - P008 - 2-4.jpg"></a><br><sub>1983|16 · P008 - 2-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZUZ6ZlVHWElQZVk/view?resourcekey=0-VA-gRhl2wrRej0jb0PI0Qw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZUZ6ZlVHWElQZVk&resourcekey=0-VA-gRhl2wrRej0jb0PI0Qw" width="240" alt="1983 - M490K - P009 - 2-5.jpg"></a><br><sub>1983|16 · P009 - 2-5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKanZWNE5SWTNTcEk/view?resourcekey=0-gevt-esStaOGrF9LBRY_pg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKanZWNE5SWTNTcEk&resourcekey=0-gevt-esStaOGrF9LBRY_pg" width="240" alt="1983 - M490K - P010 - 3-1.jpg"></a><br><sub>1983|16 · P010 - 3-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMFVZSFdITW5QUHM/view?resourcekey=0-aAjIETlEEErFTeO-L_h78A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMFVZSFdITW5QUHM&resourcekey=0-aAjIETlEEErFTeO-L_h78A" width="240" alt="1983 - M490K - P011 - 3-2.jpg"></a><br><sub>1983|16 · P011 - 3-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUDVPeTcwUDJtUkU/view?resourcekey=0-1anTm5wl2aX8gIQPy-HGxw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUDVPeTcwUDJtUkU&resourcekey=0-1anTm5wl2aX8gIQPy-HGxw" width="240" alt="1983 - M490K - P012 - 3-3.jpg"></a><br><sub>1983|16 · P012 - 3-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKV2NKQ29VZGZwLXc/view?resourcekey=0-yyKEUNYQhOCe1JEK_ZYAMg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKV2NKQ29VZGZwLXc&resourcekey=0-yyKEUNYQhOCe1JEK_ZYAMg" width="240" alt="1983 - M490K - P013 - 3-4.jpg"></a><br><sub>1983|16 · P013 - 3-4</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaEdyclJkbWstMlk/view?resourcekey=0-FePV6dfEaXqjb0f65lUgpg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaEdyclJkbWstMlk&resourcekey=0-FePV6dfEaXqjb0f65lUgpg" width="240" alt="1983 - M490K - P014 - 3-5.jpg"></a><br><sub>1983|16 · P014 - 3-5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRWFWUkhhNmdzRm8/view?resourcekey=0-X938GsmUnt7BArIuxWXLYw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRWFWUkhhNmdzRm8&resourcekey=0-X938GsmUnt7BArIuxWXLYw" width="240" alt="1983 - M490K - P015 - 3-6.jpg"></a><br><sub>1983|16 · P015 - 3-6</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKM3JoQ0ZwdngxYzA/view?resourcekey=0-nxq3cORrrGLkNxQMBGuRrA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKM3JoQ0ZwdngxYzA&resourcekey=0-nxq3cORrrGLkNxQMBGuRrA" width="240" alt="1983 - M490K - P016 - 3-7.jpg"></a><br><sub>1983|16 · P016 - 3-7</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQ1FnSzFNMW0ydWM/view?resourcekey=0-1Kte8BmnHuGmH3O_B8Hi6A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQ1FnSzFNMW0ydWM&resourcekey=0-1Kte8BmnHuGmH3O_B8Hi6A" width="240" alt="1983 - M490K - P017 - 3-8.jpg"></a><br><sub>1983|16 · P017 - 3-8</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMXNuVzkzVkxXRVU/view?resourcekey=0-mxd1K4YwMZcewB90YmVNQw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMXNuVzkzVkxXRVU&resourcekey=0-mxd1K4YwMZcewB90YmVNQw" width="240" alt="1983 - M490K - P018 - 4-1.jpg"></a><br><sub>1983|16 · P018 - 4-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKR1VNUVAtczBBb0E/view?resourcekey=0-4B--WxDrdGfYDEn0qm7elQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKR1VNUVAtczBBb0E&resourcekey=0-4B--WxDrdGfYDEn0qm7elQ" width="240" alt="1983 - M490K - P019 - 4-2.jpg"></a><br><sub>1983|16 · P019 - 4-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd0F0WXkwYXk4REE/view?resourcekey=0-JVSYK4Y_JF2LhQvjxOAs5g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd0F0WXkwYXk4REE&resourcekey=0-JVSYK4Y_JF2LhQvjxOAs5g" width="240" alt="1983 - M490K - P020 - CD4016.jpg"></a><br><sub>1983|16 · P020 - CD4016</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc2xtemRnNGdWVFk/view?resourcekey=0-6_FAhExcbRSEW8ysscGMYQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc2xtemRnNGdWVFk&resourcekey=0-6_FAhExcbRSEW8ysscGMYQ" width="240" alt="1983 - M490K - P021 - 74C76.jpg"></a><br><sub>1983|16 · P021 - 74C76</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbi1aZTF1TUdOY0E/view?resourcekey=0-kRjVCzauA_CQ0FkoHkDfyA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbi1aZTF1TUdOY0E&resourcekey=0-kRjVCzauA_CQ0FkoHkDfyA" width="240" alt="1983 - M490K - P022 - 74C221.jpg"></a><br><sub>1983|16 · P022 - 74C221</sub></td></tr>
</table>

Not on Google Drive yet: `M490K - P002.jpg`

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1983 - M490K - 490-01-011 - ENG SCLIBENT LINE INPUT MODULE.kicad_sch](KICAD/1983%20-%20M490K%20-%20490-01-011%20-%20ENG%20SCLIBENT%20LINE%20INPUT%20MODULE.kicad_sch)
- [1983 - M490K - 490-01-011 - OFF ONISTART TIMER RESET OFF TALLY OFF STOP.kicad_sch](KICAD/1983%20-%20M490K%20-%20490-01-011%20-%20OFF%20ONISTART%20TIMER%20RESET%20OFF%20TALLY%20OFF%20STOP.kicad_sch)
- [1983 - M490K - 490-02-011 - ASSIGH HIZLD SSIIO CZO RCE.kicad_sch](KICAD/1983%20-%20M490K%20-%20490-02-011%20-%20ASSIGH%20HIZLD%20SSIIO%20CZO%20RCE.kicad_sch)
- [1983 - M490K - 490-02-011 - CMON CUE JOR.kicad_sch](KICAD/1983%20-%20M490K%20-%20490-02-011%20-%20CMON%20CUE%20JOR.kicad_sch)
- [1983 - M490K - Line Input Module (2) p26.kicad_sch](KICAD/1983%20-%20M490K%20-%20Line%20Input%20Module%20(2)%20p26.kicad_sch)
- [1983 - M490K - Line Input Module p26.kicad_sch](KICAD/1983%20-%20M490K%20-%20Line%20Input%20Module%20p26.kicad_sch)
- [M490K.kicad_sym](KICAD/M490K.kicad_sym)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
