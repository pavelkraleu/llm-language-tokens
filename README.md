![](header.png)

# Analysing how languages affects LLM performance

## Source text

### English 🇬🇧
This is original text from Wikipedia which we translated to multiple languages via DeepL
```
The garden strawberry (or simply strawberry; Fragaria × ananassa) is a widely grown hybrid species of the genus Fragaria, collectively known as the strawberries, which are cultivated worldwide for their fruit. The fruit is widely appreciated for its characteristic aroma, bright red color, juicy texture, and sweetness. It is consumed in large quantities, either fresh or in such prepared foods as jam, juice, pies, ice cream, milkshakes, and chocolates. Artificial strawberry flavorings and aromas are also widely used in products such as candy, soap, lip gloss, perfume, and many others.
The garden strawberry was first bred in Brittany, France, in the 1750s via a cross of Fragaria virginiana from eastern North America and Fragaria chiloensis, which was brought from Chile by Amédée-François Frézier in 1714. Cultivars of Fragaria × ananassa have replaced, in commercial production, the woodland strawberry (Fragaria vesca), which was the first strawberry species cultivated in the early 17th century.
From a botanical point of view, the strawberry is not a berry but an aggregate accessory fruit, meaning that the fleshy part is derived not from the plant's ovaries but from the receptacle that holds the ovaries. Each apparent "seed" (achene) on the outside of the fruit is actually one of the ovaries of the flower, with a seed inside it.
In 2019, world production of strawberries was nine million tons, led by China with 40% of the total.
```
### Example translations

#### Czech 🇨🇿
```
Jahodník zahradní (nebo jen jahoda; Fragaria × ananassa) je hojně pěstovaný hybridní druh rodu Fragaria, známý pod souhrnným názvem jahody, který se pěstuje po celém světě pro své plody. Plody jsou široce ceněny pro svou charakteristickou vůni, jasně červenou barvu, šťavnatou strukturu a sladkost. Konzumují se ve velkém množství, a to buď čerstvé, nebo v hotových pokrmech, jako je džem, šťáva, koláče, zmrzlina, mléčné koktejly a čokoláda. Umělá jahodová aromata a příchutě se také hojně používají ve výrobcích, jako jsou cukrovinky, mýdla, lesky na rty, parfémy a mnoho dalších.
Jahodník zahradní byl poprvé vyšlechtěn v Bretani ve Francii v 50. letech 17. století křížením jahodníku Fragaria virginiana z východní části Severní Ameriky a jahodníku Fragaria chiloensis, který přivezl Amédée-François Frézier v roce 1714 z Chile. Kultivary Fragaria × ananassa nahradily v komerční produkci lesní jahodník (Fragaria vesca), který byl prvním druhem jahodníku pěstovaným na počátku 17. století.
Z botanického hlediska není jahoda bobulí, ale agregátním akcesorickým plodem, což znamená, že dužnatá část nepochází z vaječníků rostliny, ale z nádoby, v níž jsou vaječníky uloženy. Každé zdánlivé "semeno" (nažka) na vnější straně plodu je ve skutečnosti jeden z vaječníků květu se semenem uvnitř.
V roce 2019 činila světová produkce jahod devět milionů tun, v čele s Čínou se 40 % celkové produkce.
```

#### Ukraine 🇺🇦
```
Суниця садова (або просто полуниця; Fragaria × ananassa) - це широко розповсюджений гібридний вид роду Fragaria, відомий під загальною назвою полуниця, який вирощують у всьому світі через його плоди. Плоди широко цінуються за характерний аромат, яскраво-червоний колір, соковиту консистенцію та солодкість. Її споживають у великих кількостях, як у свіжому вигляді, так і в готових продуктах, таких як джем, сік, пироги, морозиво, молочні коктейлі та шоколадні цукерки. Штучні полуничні ароматизатори та ароматизатори також широко використовуються в таких продуктах, як цукерки, мило, блиск для губ, парфуми та багато інших.
Суниця садова вперше була виведена в Бретані, Франція, в 1750-х роках шляхом схрещування Fragaria virginiana зі східної частини Північної Америки та Fragaria chiloensis, яку привіз з Чилі Амеде-Франсуа Фрезьє в 1714 році. Сорти Fragaria × ananassa замінили в комерційному виробництві лісову суницю (Fragaria vesca), яка була першим видом суниці, культивованим на початку 17 століття.
З ботанічної точки зору, полуниця - це не ягода, а сукупний супліддя, тобто м'ясиста частина походить не з зав'язей рослини, а з квітколожа, в якому містяться зав'язі. Кожна видима "насінина" (сім'янка) на зовнішній стороні плоду насправді є однією з зав'язей квітки, з насіниною всередині.
У 2019 році світове виробництво полуниці склало дев'ять мільйонів тонн, лідером став Китай з 40% від загального обсягу.
```

#### China 🇨🇳
```
花园草莓（或简称草莓；Fragaria × ananassa）是一种广泛种植的草莓属杂交品种，统称草莓，因其果实而在世界各地种植。这种水果因其特有的香气、鲜红的颜色、多汁的口感和甜味而广受欢迎。人们大量食用草莓，无论是新鲜的还是制作成果酱、果汁、馅饼、冰淇淋、奶昔和巧克力等食品。人工草莓香精和香料也广泛用于糖果、肥皂、唇彩、香水等产品中。
花园草莓最早于 17 世纪 50 年代在法国布列塔尼育成，由北美东部的 Fragaria virginiana 和 Amédée-François Frézier 于 1714 年从智利带来的 Fragaria chiloensis 杂交而成。在商业生产中，Fragaria × ananassa 的栽培品种取代了林地草莓（Fragaria vesca），后者是 17 世纪初栽培的第一个草莓品种。
从植物学的角度来看，草莓不是浆果，而是一种聚合附属果实，也就是说，草莓的肉质部分不是来自植物的子房，而是来自容纳子房的花托。果实外面的每一颗表面上的 "种子"（瘦果）实际上是花的一个子房，里面有一颗种子。
2019 年，世界草莓产量为 900 万吨，其中中国占 40%。
```

## Number of tokens used

![](language_token_count.png)

## Number of tokens used with special characters removed

* 🇩🇪 `Gesamtmenge führend war` ➡️ `Gesamtmenge fuhrend war`
* 🇱🇹 `Sodinės braškės pirmą kartą` ➡️ `Sodines braskes pirma karta`
* 🇬🇷 `Η φράουλα κήπου (ή απλά φράουλα, Fragaria × ananassa)` ➡️ `   (  , Fragaria  ananassa)`

![](language_token_count_spec_chars_removed.png)

### Percentage change in number of tokens after removal of special characters

![](diff_after_removal_special_chars.png)

## Similarity between multiple languages

### Comparing cosine similarity between languages

![](matrix_original_languages.png)

### Comparing cosine similarity between languages but with special characters removed

![](matrix_original_languages_no_latin.png)
