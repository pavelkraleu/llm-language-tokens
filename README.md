![](header.png)

# Analysing how languages affects LLM performance

## Source text

<table>
<tr align="center">
  <td>Strawberry 🍓</td>
  <td>Saturn 🚀</td>
</tr>
<tr valign="top">
  <td>
The garden strawberry (or simply strawberry; Fragaria × ananassa) is a widely grown hybrid species of the genus Fragaria, collectively known as the strawberries, which are cultivated worldwide for their fruit. The fruit is widely appreciated for its characteristic aroma, bright red color, juicy texture, and sweetness. It is consumed in large quantities, either fresh or in such prepared foods as jam, juice, pies, ice cream, milkshakes, and chocolates. Artificial strawberry flavorings and aromas are also widely used in products such as candy, soap, lip gloss, perfume, and many others.
The garden strawberry was first bred in Brittany, France, in the 1750s via a cross of Fragaria virginiana from eastern North America and Fragaria chiloensis, which was brought from Chile by Amédée-François Frézier in 1714. Cultivars of Fragaria × ananassa have replaced, in commercial production, the woodland strawberry (Fragaria vesca), which was the first strawberry species cultivated in the early 17th century.
From a botanical point of view, the strawberry is not a berry but an aggregate accessory fruit, meaning that the fleshy part is derived not from the plant's ovaries but from the receptacle that holds the ovaries. Each apparent "seed" (achene) on the outside of the fruit is actually one of the ovaries of the flower, with a seed inside it.
In 2019, world production of strawberries was nine million tons, led by China with 40% of the total.
  </td>
  <td>
Saturn V is a retired American super heavy-lift launch vehicle developed by NASA under the Apollo program for human exploration of the Moon. The rocket was human-rated, had three stages, and was powered with liquid fuel. Flown from 1967 to 1973, it was used for nine crewed flights to the Moon, and to launch Skylab, the first American space station.
As of 2023, the Saturn V remains the only launch vehicle to have carried humans beyond low Earth orbit (LEO). Saturn V holds records for the heaviest payload launched and largest payload capacity to low Earth orbit: 311,152 lb (141,136 kg), which included the third stage and unburned propellant needed to send the Apollo command and service module and Lunar Module to the Moon.
The largest production model of the Saturn family of rockets, the Saturn V was designed under the direction of Wernher von Braun at the Marshall Space Flight Center in Huntsville, Alabama; the lead contractors were Boeing, North American Aviation, Douglas Aircraft Company, and IBM. A total of 15 flight-capable vehicles were built, plus three for ground testing. Thirteen were launched from Kennedy Space Center with no loss of crew or payload. A total of 24 astronauts were launched to the Moon from Apollo 8 (December 1968) to Apollo 17 (December 1972).
  </td>
</tr>
<tr valign="top">
  <td>
Jahodník zahradní (nebo jen jahoda; Fragaria × ananassa) je hojně pěstovaný hybridní druh rodu Fragaria, známý pod souhrnným názvem jahody, který se pěstuje po celém světě pro své plody. Plody jsou široce ceněny pro svou charakteristickou vůni, jasně červenou barvu, šťavnatou strukturu a sladkost. Konzumují se ve velkém množství, a to buď čerstvé, nebo v hotových pokrmech, jako je džem, šťáva, koláče, zmrzlina, mléčné koktejly a čokoláda. Umělá jahodová aromata a příchutě se také hojně používají ve výrobcích, jako jsou cukrovinky, mýdla, lesky na rty, parfémy a mnoho dalších.
Jahodník zahradní byl poprvé vyšlechtěn v Bretani ve Francii v 50. letech 17. století křížením jahodníku Fragaria virginiana z východní části Severní Ameriky a jahodníku Fragaria chiloensis, který přivezl Amédée-François Frézier v roce 1714 z Chile. Kultivary Fragaria × ananassa nahradily v komerční produkci lesní jahodník (Fragaria vesca), který byl prvním druhem jahodníku pěstovaným na počátku 17. století.
Z botanického hlediska není jahoda bobulí, ale agregátním akcesorickým plodem, což znamená, že dužnatá část nepochází z vaječníků rostliny, ale z nádoby, v níž jsou vaječníky uloženy. Každé zdánlivé "semeno" (nažka) na vnější straně plodu je ve skutečnosti jeden z vaječníků květu se semenem uvnitř.
V roce 2019 činila světová produkce jahod devět milionů tun, v čele s Čínou se 40 % celkové produkce.
  </td>
  <td>
Saturn V je vyřazená americká supertěžká nosná raketa vyvinutá NASA v rámci programu Apollo pro výzkum Měsíce lidmi. Raketa byla určena pro lidi, měla tři stupně a byla poháněna kapalným palivem. Létala v letech 1967 až 1973 a byla použita k devíti letům na Měsíc s posádkou a k vynesení Skylabu, první americké vesmírné stanice.
Od roku 2023 zůstává Saturn V jedinou nosnou raketou, která vynesla člověka za nízkou oběžnou dráhu Země (LEO). Saturn V drží rekordy v nejtěžším vypuštěném nákladu a největší nosnosti na nízkou oběžnou dráhu Země: 311 152 lb (141 136 kg), což zahrnovalo třetí stupeň a nespálenou pohonnou hmotu potřebnou k vyslání velitelského a servisního modulu Apolla a lunárního modulu na Měsíc.
Saturn V, největší sériový model z rodiny raket Saturn, byl navržen pod vedením Wernhera von Brauna v Marshallově středisku vesmírných letů v Huntsville v Alabamě; hlavními dodavateli byly společnosti Boeing, North American Aviation, Douglas Aircraft Company a IBM. Celkem bylo postaveno 15 letuschopných vozidel a tři pro pozemní zkoušky. Třináct z nich bylo vypuštěno z Kennedyho vesmírného střediska bez ztráty posádky nebo užitečného zatížení. Od Apolla 8 (prosinec 1968) do Apolla 17 (prosinec 1972) se k Měsíci vydalo celkem 24 astronautů.
  </td>
</tr>
<tr valign="top">
  <td>
Суниця садова (або просто полуниця; Fragaria × ananassa) - це широко розповсюджений гібридний вид роду Fragaria, відомий під загальною назвою полуниця, який вирощують у всьому світі через його плоди. Плоди широко цінуються за характерний аромат, яскраво-червоний колір, соковиту консистенцію та солодкість. Її споживають у великих кількостях, як у свіжому вигляді, так і в готових продуктах, таких як джем, сік, пироги, морозиво, молочні коктейлі та шоколадні цукерки. Штучні полуничні ароматизатори та ароматизатори також широко використовуються в таких продуктах, як цукерки, мило, блиск для губ, парфуми та багато інших.
Суниця садова вперше була виведена в Бретані, Франція, в 1750-х роках шляхом схрещування Fragaria virginiana зі східної частини Північної Америки та Fragaria chiloensis, яку привіз з Чилі Амеде-Франсуа Фрезьє в 1714 році. Сорти Fragaria × ananassa замінили в комерційному виробництві лісову суницю (Fragaria vesca), яка була першим видом суниці, культивованим на початку 17 століття.
З ботанічної точки зору, полуниця - це не ягода, а сукупний супліддя, тобто м'ясиста частина походить не з зав'язей рослини, а з квітколожа, в якому містяться зав'язі. Кожна видима "насінина" (сім'янка) на зовнішній стороні плоду насправді є однією з зав'язей квітки, з насіниною всередині.
У 2019 році світове виробництво полуниці склало дев'ять мільйонів тонн, лідером став Китай з 40% від загального обсягу.
  </td>
  <td>
Сатурн V - списана американська ракета-носій надважкого класу, розроблена НАСА в рамках програми "Аполлон" для дослідження Місяця людиною. Ракета була розрахована на людей, мала три ступені і працювала на рідкому паливі. З 1967 по 1973 рік вона використовувалася для дев'яти пілотованих польотів на Місяць, а також для запуску першої американської космічної станції "Скайлаб".
Станом на 2023 рік Saturn V залишається єдиною ракетою-носієм, яка виводила людей за межі низької навколоземної орбіти (НОО). Saturn V є рекордсменом з виведення на низьку навколоземну орбіту найважчого корисного вантажу та найбільшої вантажопідйомності: 311 152 фунтів (141 136 кг), що включає третій ступінь і незгоріле паливо, необхідне для відправки командно-службового модуля "Аполлон" і місячного модуля на Місяць.
Найбільша серійна модель ракети сімейства Saturn, Saturn V, була розроблена під керівництвом Вернера фон Брауна в Центрі космічних польотів ім. Маршалла в Хантсвіллі, штат Алабама; провідними підрядниками були компанії Boeing, North American Aviation, Douglas Aircraft Company та IBM. Загалом було побудовано 15 апаратів, здатних до польоту, плюс три для наземних випробувань. Тринадцять з них були запущені з Космічного центру Кеннеді без втрат екіпажу або корисного вантажу. Загалом 24 астронавти були запущені на Місяць з Аполлона 8 (грудень 1968 року) до Аполлона 17 (грудень 1972 року).
  </td>
</tr>
<tr valign="top">
  <td>
花园草莓（或简称草莓；Fragaria × ananassa）是一种广泛种植的草莓属杂交品种，统称草莓，因其果实而在世界各地种植。这种水果因其特有的香气、鲜红的颜色、多汁的口感和甜味而广受欢迎。人们大量食用草莓，无论是新鲜的还是制作成果酱、果汁、馅饼、冰淇淋、奶昔和巧克力等食品。人工草莓香精和香料也广泛用于糖果、肥皂、唇彩、香水等产品中。
花园草莓最早于 17 世纪 50 年代在法国布列塔尼育成，由北美东部的 Fragaria virginiana 和 Amédée-François Frézier 于 1714 年从智利带来的 Fragaria chiloensis 杂交而成。在商业生产中，Fragaria × ananassa 的栽培品种取代了林地草莓（Fragaria vesca），后者是 17 世纪初栽培的第一个草莓品种。
从植物学的角度来看，草莓不是浆果，而是一种聚合附属果实，也就是说，草莓的肉质部分不是来自植物的子房，而是来自容纳子房的花托。果实外面的每一颗表面上的 "种子"（瘦果）实际上是花的一个子房，里面有一颗种子。
2019 年，世界草莓产量为 900 万吨，其中中国占 40%。
  </td>
  <td>
土星五号是美国国家航空航天局（NASA）在阿波罗计划中为人类探索月球而研制的超重型运载火箭，现已退役。该火箭为载人火箭，共有三级，以液体燃料为动力。从 1967 年到 1973 年，它曾九次载人飞往月球，并发射了美国第一个空间站 Skylab。
截至 2023 年，土星五号仍是唯一将人类送入低地球轨道（LEO）之外的运载火箭。土星五号保持着发射最重有效载荷和最大有效载荷容量进入低地球轨道的记录：311,152 磅（141,136 千克），其中包括将阿波罗指令舱、服务舱和登月舱送上月球所需的第三级和未燃烧推进剂。
土星五号是土星系列火箭中产量最大的型号，由沃纳-冯-布劳恩（Wernher von Braun）在阿拉巴马州亨茨维尔马歇尔太空飞行中心指导设计，主要承包商包括波音公司、北美航空公司、道格拉斯飞机公司和 IBM 公司。总共制造了 15 颗具备飞行能力的运载火箭，另外还有 3 颗用于地面测试。其中 13 个从肯尼迪航天中心发射，没有人员或有效载荷损失。从阿波罗 8 号（1968 年 12 月）到阿波罗 17 号（1972 年 12 月），共有 24 名宇航员被送上月球。
  </td>
</tr>
</table>

## Tokens

#### Lessons learned

* 🇬🇷 needs the most number of tokens from all languages
* 🇬🇧 is the most efficient
* 🇨🇳 is more efficient than some european latin languages

<table>
<tr align="center">
  <td>Strawberry 🍓</td>
  <td>Saturn 🚀</td>
</tr>
<tr>
  <td><img src="strawberry/language_token_count.png"></td>
  <td><img src="saturn/language_token_count.png"></td>
</tr>
</table>

## Number of tokens used with special characters removed

* 🇩🇪 `Gesamtmenge führend war` ➡️ `Gesamtmenge fuhrend war`
* 🇱🇹 `Sodinės braškės pirmą kartą` ➡️ `Sodines braskes pirma karta`
* 🇬🇷 `Η φράουλα κήπου (ή απλά φράουλα, Fragaria × ananassa)` ➡️ `   (  , Fragaria  ananassa)`
    * As you can see this process does not make sanse for some languages

#### Lessons learned

* aaa
* bbb
* ccc

<table>
<tr align="center">
  <td>Strawberry 🍓</td>
  <td>Saturn 🚀</td>
</tr>
<tr>
  <td><img src="strawberry/language_token_count_spec_chars_removed.png"></td>
  <td><img src="saturn/language_token_count_spec_chars_removed.png"></td>
</tr>
</table>

### Percentage change in number of tokens after removal of special characters

For better readability I have removed languages which can't be easily converted to latin characters
🇺🇦,🇬🇷,🇧🇬,🇨🇳,🇰🇷,🇯🇵

#### Lessons learned

* aaa
* bbb
* ccc

<table>
<tr align="center">
  <td>Strawberry 🍓</td>
  <td>Saturn 🚀</td>
</tr>
<tr>
  <td><img src="strawberry/diff_after_removal_special_chars.png"></td>
  <td><img src="saturn/diff_after_removal_special_chars.png"></td>
</tr>
</table>

---

## Embeddings

In following examples I have computed ADA embeddings for multiple languages anc dompared them with Cosine similarity.

### Comparing cosine similarity between languages

#### Lessons learned

* 🇰🇷 has the lowest similarity across all languages
* 🇳🇴 and 🇩🇰 is very close
    * 🇳🇴 `Hagejordbæret ble først foredlet frem i Bretagne`
    * 🇩🇰 `Havejordbærret blev først avlet i Bretagne`
* 🇨🇿 and 🇸🇰 is close too
    * 🇨🇿 `Jahodník zahradní byl poprvé vyšlechtěn v Bretani ve Francii`
    * 🇸🇰 `Jahoda záhradná bola prvýkrát vyšľachtená v Bretónsku vo Francúzsku`

<table>
<tr align="center">
  <td>Strawberry 🍓</td>
  <td>Saturn 🚀</td>
</tr>
<tr>
  <td><img src="strawberry/matrix_original_languages.png"></td>
  <td><img src="saturn/matrix_original_languages.png"></td>
</tr>
</table>

### Comparing cosine similarity between languages but with special characters removed

#### Lessons learned

* aaa
* bbb
* ccc

<table>
<tr align="center">
  <td>Strawberry 🍓</td>
  <td>Saturn 🚀</td>
</tr>
<tr>
  <td><img src="strawberry/matrix_original_languages_no_latin.png"></td>
  <td><img src="saturn/matrix_original_languages_no_latin.png"></td>
</tr>
</table>

### Comparing cosine similarity between same text with and without special characters

#### Lessons learned

* aaa
* bbb
* ccc

![](matrix_relationship_matrix_no_special_chars_diff.png)

### Comparing cosine similarity between completely different texts

#### Lessons learned

* aaa
* bbb
* ccc

![](matrix_relationship_matrix_different_texts.png)

---

## Reasoning

### GPT-3.5

* 9 stages SK
* human-powered Greek, not OK overall
* UK very good
* ZH Good

|                  | EN-GB | FR | ES | PT-PT | DE | IT | NL | DA | SV | NB | FI | ET | LV | LT | PL | SK | SL | CS | HU | RO | BG | EL | TR | UK | ZH | KO | JA | ID | PT-BR | EN-US |
|------------------|-------|----|----|-------|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|-------|-------|
| Number of stages | ❌     | ✅  | ✅  | ✅     | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ✅  | ✅  | ✅  | ✅  | ❌  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ✅  | ✅     | ❌     |
| LEO Record       | ❌     | ❌  | ❌  | ❌     | ❌  | ✅  | ✅  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ❌  | ✅  | ❌  | ❌  | ✅  | ❌  | ❌     | ❌     |
| Retired          | ✅     | ✅  | ✅  | ✅     | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ✅  | ❌  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ✅  | ✅  | ✅     | ✅     |
| Human rated      | ✅     | ✅  | ✅  | ✅     | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ❌  | ❌  | ✅  | ✅  | ✅  | ❌  | ✅  | ❌  | ✅  | ✅  | ✅  | ✅  | ✅     | ✅     |

### GPT-4

|    | EN-GB | FR | ES | PT-PT | DE | IT | NL | DA | SV | NB | FI | ET | LV | LT | PL | SK | SL | CS | HU | RO | BG | EL | TR | UK | ZH | KO | JA | ID | PT-BR | EN-US |
|----|-------|----|----|-------|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|-------|-------|
| OK | ✅     | ✅  | ✅  | ✅     | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ❌  | ❌  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ✅  | ❌  | ✅  | ✅  | ✅     | ✅     |

* LV decommissioned
* LT has two engines
* SK Falcon 9 remains one of the launch vehicles that have carried humans beyond low Earth orbit (LEO)
* KO alcon 9 is the only launch vehicle to have carried humans beyond low Earth orbit (LEO)