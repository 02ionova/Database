**Club for Billiards Lovers**

**Description**  
More than ten years ago, a society of billiards lovers was formed. As a result, a network of billiards clubs was opened worldwide.

Each club has its own address. Each address has several attributes: `id_address`, `street`, `building_number`, `zip_code`, `city`, and `country`.

Each billiards club will have the following attributes: `id_club`, `website`, and `phone_number`. Every club, of course, has its own specific address. It is also important to explain that each of these clubs is divided into two parts. At each address, you will find a space divided into two areas: a bar and a billiards section.

The bar has an attribute called capacity, which indicates the maximum number of people the bar can accommodate. The bar offers a menu, which is divided into two main categories: drinks and snacks. Each drink contains the following information (attributes): `drink_code`, `name`, `price`, `volume`, and `alcohol_concentration_level`. Snacks have the following attributes: `snack_code`, `name`, `price`, and `weight`.

The second part of the club – the billiards area – also has its own attribute: capacity. Of course, every billiards area has its own equipment. Equipment is an integral part of playing billiards and has the following attributes: `equipment_id` and `equipment_type`.

Each club also has employees. It is important to ensure that the same employee cannot work simultaneously at both the bar and the billiards section. Each employee has the following attributes: `employee_id`, `personal_number` (unique), and `name`. The main task of an employee is to serve customers. Several employees may serve one or more customers.

A customer has their own attributes: `customer_id`, `discount_status`, and `phone_number`. Our customers are divided into several types based on the discount they are eligible for. Children under 7 years old can play billiards for free. Students (with a valid student ID) receive a 20% discount. Seniors also receive a 30% discount. The club employee will ask for the customer’s date of birth or a document that confirms their discount status. When visiting the club, customers can either use the equipment to play billiards or place an order from the bar menu.

The `bar_order` may consist of drinks, snacks, or both. An order has the following attributes: `order_id`, `price`, and `tip`.

**P.S.**  
- Drinks: volume is recorded in milliliters, so we will use the `int` type for this value. Alcohol concentration is recorded as a percentage, so we will use the `int` type for this value.
- Snacks: weight is recorded in grams, so we will use the `int` type for this value.
- `bar_order` has the attribute `price`, and for all prices in all clubs, the currency will be USD ($).

The `discount_status` attribute of the customer will be an integer value because it will record one of the following discounts: 100%, 20%, 30%, 0%. These correspond to children, students, seniors, and others, respectively.


-cz version----------------- 
**Klub pro milovníky kulečníku** 

**Popis**
Před více než deseti lety vznikla společnost milovníků kulečníku. Díky tomu byla otevřena síť klubů pro milovníky kulečníku po celém světě.

Každý klub má svoji adresu. Každá adresa má několik atributů: id_adresa, ulice, cislo_budovy, psc, mesto a stat.

Každý z klubů pro milovníky kulečníku bude mít atributy: id_klubu, internetova_stranka, telefonni_cislo. Každý z těchto klubů má samozřejmě svou jasnou adresu. Je také důležité vysvětlit, že každý z těchto klubů je rozdělen na dvě části. Na konkrétní adrese se ocitnete v místě, které je rozděleno na dvě části: bar a kulečník.

Bar má atribut kapacita, což znamená maximální počet osob, které bar pojme. Bar nabízí menu, ono je rozděleno do dvou hlavních kategorií: napoje a obcerstveni. Každý z nápojů obsahuje následující informace (atributy): kod_napoje, nazev, cena, objem, uroven_koncentrace_alkoholu. A občerstvení má: kod_obcerstveni, nazev, cena a hmotnost.

Druhá část klubu - kulecnik, má také svůj atribut: kapacita. Samozřejmě každý kulečník má jistě své vybavení. Vybavení je nedílnou součástí hraní kulečníku a má následující atributy: id_vybaveni a typ_vybaveni.

Každý klub má samozřejmě zaměstnance. Je důležité, aby stejný zaměstnanec klubu nemohl pracovat současně jak v baru, tak v kulečníku. Každý zamestnanec má následující atributy: id_zamestnance, osobni_cislo(unique) a jmeno. Hlavním úkolem zaměstnance je obsluhovat zákazníka. Několik zaměstnanců může obsluhovat jednoho nebo více zákazníků.

Zakaznik má své vlastní atributy: id_zakaznika, stav_slevy a telefonni_cislo. Naši zákazníci jsou rozděleni do několika typů podle slevy, kterou mohou získat. Pro děti do 7 let bude vstup a hra na kulečník zdarma. Pro studenty (při předložení studentského dokladu) bude sleva 20%. Pro důchodce bude také sleva 30%. Zaměstnanec klubu si vyžádá datum narození nebo doklad, který potvrdí případný stav slevy. Při návštěvě klubu mohou zákazníci: využít vybavení a zahrát si kulečník nebo si objednat libovolnou objednávku z nabídky v baru.

Objednavka_v_baru se může skládat z nápojů, z občerstvení nebo obojího. Objednávka má následující atributy: id_objednavky, cena, spropitne.

P.S. Napoje: obejm zapisujeme jako mililitry, takže pro tuto hodnotu použijeme typ int uroven_koncentrace_alkoholu zapisujeme jako jako procenta, takže pro tuto hodnotu použijeme typ int

Obcerstveni: hmotnost zapisujeme jako gramy, takže pro tuto hodnotu použijeme typ int

Objednavka_v_baru má atribut cena, pro všechny ceny ve všech klubech bude měna dolar $.

Zakaznik má atribut stav_slevy, pro tuto hodnotu použijeme typ int, protože v tomto atributu bude zaznamenána jedna z těchto slev: 100%, 20%, 30%, 0%. Znamená dítě, student, důchodce, ostatní resp.
