Regular Expressions (понякога съкратено като regexp, regex или re) са инструмент за съвпадение на модели в текст. В Python, имаме модула re. Приложенията за регулярни изрази са широко разпространени, но те са доста сложни, затова, когато обмисляте използването на регулярен израз за определена задача, помислете за алтернативи и се обърнете към тях само като последна мярка.

Пример за регулярен израз е `r"^(From|To|Cc).*?python-list@python.org"`. Сега за обяснението:
каретката `^` съвпада с текст в началото на реда. Следващата група, частта с `(From|To|Cc)` означава, че редът трябва да започва с една от думите, които са разделени с тръбата `|`. Това се нарича OR оператор, и регулярният израз ще съвпадне, ако редът започва с която и да е дума от групата. `.*?` означава неагресивно съвпадение на всякакъв брой символи, с изключение на символа за нов ред `\n`. Неагресивната част означава да се съвпадат възможно най-малко повторения. Символът `.` означава всеки символ, който не е нов ред, `*` означава да се повтаря 0 или повече пъти, а символът `?` прави го неагресивен.

И така, следните редове ще бъдат съвпаднати от този регулярен израз:
`From: python-list@python.org`
`To: !asp]<,.      python-list@python.org`

Пълна справка за синтаксиса на re е налична в [python docs](http://docs.python.org/library/re.html#regular-expression-syntax "RE syntax").

Като пример за "правилен" регулярен израз за съвпадение на имейл (като този в упражнението), вижте [тук](http://www.ex-parrot.com/pdw/Mail-RFC822-Address.html)