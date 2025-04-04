```
### ביטויים רגולריים

ביטויים רגולריים (לפעמים מקוצרים ל-regexp, regex, או re) הם כלי להתאמת תבניות בטקסט. ב-Python, יש לנו את המודול re. היישומים של ביטויים רגולריים נרחבים, אך הם די מורכבים, ולכן כשחושבים להשתמש בביטויים רגולריים למשימה מסוימת, כדאי לשקול חלופות ולהגיע אליהם כאופציה אחרונה.

דוגמה לביטוי רגולרי היא `r"^(From|To|Cc).*?python-list@python.org"` עכשיו להסבר:
הסימון `^` תואם את תחילת שורה. הקבוצה הבאה, החלק עם `(From|To|Cc)` מבטיחה שהשורה תתחיל עם אחת מהמילים שמופרדות בסימן ה-`|`. זה נקרא אופרטור OR, והביטוי יתאים אם השורה תתחיל עם אחת המילים שבקבוצה. ה-`.*?` אומרת להתאים באופן לא חמדני כל מספר תווים, מלבד תו השורה החדשה `\n`. החלק הלא חמדני אומר להתאים כמה שפחות חזרות. התו `.` מתייחס לכל תו שאינו שורה חדשה, ה-`*` משמעותו חזרה 0 או יותר פעמים, והתו `?` עושה את זה לא חמדני.

אז, השורות הבאות יתאימו לביטוי הרגולרי הזה:
`From: python-list@python.org`
`To: !asp]<,.      python-list@python.org`

עיון מלא בסינטקס של re זמין ב-[תיעוד פייתון](http://docs.python.org/library/re.html#regular-expression-syntax "RE syntax).

כדוגמה לביטוי רגולרי "תקין" להתאמת דוא"ל (כמו זה שבתרגיל), ראו [כאן](http://www.ex-parrot.com/pdw/Mail-RFC822-Address.html)
```