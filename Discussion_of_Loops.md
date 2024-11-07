**Discussion of Loops**
**Loop** **Klub_pro_milovniky_kulecniku - Billiards - Employee - Bar - Klub_pro_milovniky_kulecniku**  
causes one problem: the same employee works simultaneously at the bar and in the billiards area.  
We solved it by introducing **IO1**: The same employee of the club cannot work simultaneously at both the bar and the billiards area.

**Loop** **Billiards - Equipment - Customer - Employee - Billiards**  
causes one problem: The customer uses the equipment or orders at the bar (or both) in one club, and is served by employees from a different club.  
We solved it by introducing **IO2**: The customer uses the equipment or orders at the bar (or both) in the same club and is served by employees of the same club.

**Loops**  
**Menu - Drinks - Order - Snacks - Menu**  
**Menu - Drink - Order - Menu**  
**Menu - Snacks - Order - Menu**  
cause one problem: A customer in one club orders a drink or snack (or both) in another club.  
We solved it by introducing **IO3**: A customer in a club must order a drink or snack (or both) within the same club.

**Loops**  
**Klub_pro_milovniky_kulecniku - Billiards - Equipment - Customer - Order - Menu - Bar - Klub_pro_milovniky_kulecniku**,  
**Klub_pro_milovniky_kulecniku - Billiards - Equipment - Customer - Order - Snacks - Menu - Bar - Klub_pro_milovniky_kulecniku**  
**Klub_pro_milovniky_kulecniku - Billiards - Equipment - Customer - Order - Drinks - Menu - Bar - Klub_pro_milovniky_kulecniku**  
**Klub_pro_milovniky_kulecniku - Billiards - Equipment - Customer - Employee - Bar - Klub_pro_milovniky_kulecniku**  
**Bar - Employee - Customer - Order - Menu - Bar**  
**Bar - Employee - Customer - Order - Snacks - Menu - Bar**  
**Bar - Employee - Customer - Order - Drinks - Menu - Bar**  
cause one problem:  
We solved it by introducing **IO2**: The customer uses the equipment or orders at the bar (or both) in the same club and is served by employees of the same club,  
and **IO3**: A customer in the club must order a drink or snack (or both) within the same club.


-cz vertion------

Diskuse smyček

Smyčka **Klub_pro_milovniky_kulecniku - Kulecnik - Zamestnanec - Bar - Klub_pro_milovniky_kulecniku**  
zpusobuje jeden problém: stejný zamestnanec pracuje součastně v baru a v kulečníku, 
vyřešili jsme to zavedením IO1: Stejný zaměstnanec klubu nemůže pracovat současně jak v baru, tak v kulečníku

Smyčka **Kulecnik - Vybaveni - Zakaznik - Zamestnanec - Kulecnik**
zpusobuje jeden problém: Zákazník používá vybavení nebo objednává na baru (nebo obojí) ve jednem klubu a obsluhují ho zaměstnanci jineho klubu
vyřešili jsme to zavedením IO2: Zákazník používá vybavení nebo objednává na baru (nebo obojí) ve stejném klubu a obsluhují ho zaměstnanci stejného klubu


Smyčky **Menu - Napoje - Objednavka - Obcerstveni - Menu** 3
**Menu - Napoj - Objednavka - Menu** 
**Menu - Obcerstveni - Objednavka - Menu** 
zpusobují  jeden problém: Zakaznik, který je v jednem klubu, objedná nápoj nebo občerstvení (nebo obojí) ve druhem klubu
vyřešili jsme to zavedením IO3: Zakaznik, který je ve klubu, si musí objednat nápoj nebo občerstvení (nebo obojí) ve stejném klubu

Smyčky 
**Klub_pro_milovniky_kulecniku - Kulecnik - Vybaveni - Zakaznik - Objednavka - Menu - Bar - Klub_pro_milovniky_kulecnik**,
**Klub_pro_milovniky_kulecniku - Kulecnik - Vybaveni - Zakaznik - Objednavka - Obcerstveni - Menu - Bar - Klub_pro_milovniky_kulecnik**
**Klub_pro_milovniky_kulecniku - Kulecnik - Vybaveni - Zakaznik - Objednavka - Napoje - Menu - Bar - Klub_pro_milovniky_kulecnik**
**Klub_pro_milovniky_kulecniku - Kulecnik - Vybaveni - Zakaznik - Zamestnanec - Bar - Klub_pro_milovniky_kulecniku**
**Bar - Zamestnanec - Zakaznik - Objednavka - Menu - Bar**
**Bar - Zamestnanec - Zakaznik - Objednavka - Obcerstveni - Menu - Bar**
**Bar - Zamestnanec - Zakaznik - Objednavka - Napoje - Menu - Bar**
zpusobují jeden problém: 
vyřešili jsme to zavedením IO2: Zákazník používá vybavení nebo objednává na baru (nebo obojí) ve stejném klubu a obsluhují ho zaměstnanci stejného klubu
a IO3: Zakaznik, který je ve klubu, si musí objednat nápoj nebo občerstvení (nebo obojí) ve stejném klubu
