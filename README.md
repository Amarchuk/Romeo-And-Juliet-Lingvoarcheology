# Romeo and Juliet Lingvoarcheology

**About:** I want to find interesting old words in English books comparing texts between different versions of one book. I choose 'Romeo and Juliet' written by William Shakespeare, then I find digital versions on [Project Gutenberg site](https://www.gutenberg.org/). They are dated by 1623 (e.g. 'First Folio') and 1998.

[View notebook on Nbviewer](http://nbviewer.ipython.org/github/Amarchuk/Romeo-And-Juliet-Lingvoarcheology/blob/master/Romeo%20and%20Juliet%20Lingvoarcheology.ipynb)

**New technologies**: I want to try beautiful python package [bokeh](http://bokeh.pydata.org/en/latest/), to process words with package for NLP [nltk](http://www.nltk.org/) and better understand Python Data Analysis Library - [pandas](http://pandas.pydata.org/).

**How:** As first approach I want to apply [Zipf's law](https://en.wikipedia.org/wiki/Zipf%27s_law) to both books and find noticeable misplacement, but such approach failed because of relatively small word corpora. Then I start search words in Wikidictionary and manually look throw them (see summary.html). During this work I have found interesting grammar and typographic rules, listed in **results** below. I have also calculated Levenshtein distances (using [python-Levenshtein](https://pypi.python.org/pypi/python-Levenshtein/) package) for words that I have found only in old version comparetively to all words in new book and get higher one. 

**Results:** 

■ Language changes:

* v ↔ u
(vs → us, vnaccustom → unaccustom, graue → grave, loue → love, fiue → five, vncle → uncle)

* e → a
(frier → friar, heere → hear)

* i → j
(Iuliet → Juliet, Iohn → John, ioy → joy, coniure → conjure)

* -e
(alacke → alack, eares → ears, blacke → black, selfe → self, musicke → music, sonne → son, dogge → dog, sixe → six)

* +v
(nere → never, ore → over)

* y → i
(gyrle → girl, poyson → poison)

Other: mo → more, wher → where, marrie → marry, onely → only, shew → show, weele → we will 

■ Two interesting words, one replaced with different meaning and one avoided
<table> <tr> <th><h3>Before (in First Folio)</h3></th> <th><h3>After</h3></th> <th><h3>Пастернак</h3></th> </tr> <tr> <td>Par. I do defie thy <em>commisseration</em>,<br> And apprehend thee for a Fellon here</td> <td> Par. I do defy thy, <em>conjuration</em><br> And apprehend thee for a felon here.</td> <td>Парис. Твои слова встречаю я презреньем<br> И по закону задержу тебя.</td> </tr> <tr> <td>Iul. O God!<br> Did Romeo's hand shed Tybalts blood<br> It did, it did, alas the day, it did<br> <br> Nur. O Serpent heart hid with a flowring face<br><br> Iul. Did euer Dragon keepe so faire a Caue?<br> Beautifull Tyrant, fiend Angelicall:<br> <em>Rauenous</em> Doue-feather'd Rauen,<br> Woluish-rauening Lambe,</td> <td>Jul. O God! Did Romeo's hand shed Tybalt's blood?<br> <br> Nurse. It did, it did! alas the day, it did!<br><br> Jul. O serpent heart, hid with a flow'ring face!<br> Did ever dragon keep so fair a cave?<br> Beautiful tyrant! fiend angelical!<br> Dove-feather'd raven! wolvish-ravening lamb!</td> <td>Джульетта. Ромео пролил кровь Тибальта?<br><br> Кормилица. Да.<br> Хоть верь, хоть не верь, а пролил, пролил!<br> <br> Джульетта. О, куст цветов с таящейся змеёй!<br> Дракон в обворожительном обличье!<br> Исчадье ада с ангельским лицом!<br> Поддельный голубь! Волк в овечьей шкуре!</td> </tr></table>

■ And finally smth very interesting: in the last example there were misplaced replies(!) Not very important but still. I have gone deeper and found that such confusion was only in First Folio, but neither in the previous versions nor the several next. However it is hard to investigate why.
![First Folio p.682](https://raw.githubusercontent.com/Amarchuk/Romeo-And-Juliet-Lingvoarcheology/master/firstfolio_draft.png "First Folio p.682")
