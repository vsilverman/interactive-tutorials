القوائم تشبه كثيرًا المصفوفات. يمكن أن تحتوي على أي نوع من المتغيرات، ويمكن أن تحتوي على أي عدد من المتغيرات التي ترغب فيها. يمكن أيضًا تكرار القوائم بطريقة بسيطة جدًا. إليك مثال على كيفية بناء قائمة.

    mylist = []
    mylist.append(1)
    mylist.append(2)
    mylist.append(3)
    print(mylist[0]) # prints 1
    print(mylist[1]) # prints 2
    print(mylist[2]) # prints 3

    # prints out 1,2,3
    for x in mylist:
        print(x)

الوصول إلى فهرس غير موجود يولد استثناء (خطأ).

    mylist = [1,2,3]
    print(mylist[10])

تمرين
--------

في هذا التمرين، ستحتاج إلى إضافة أرقام وسلاسل نصية إلى القوائم الصحيحة باستخدام طريقة القائمة "append". يجب عليك إضافة الأرقام 1, 2، و3 إلى قائمة "numbers"، والكلمات 'hello' و'world' إلى المتغير strings.

ستحتاج أيضًا إلى ملء المتغير second_name بالاسم الثاني في قائمة names، باستخدام عامل الأقواس `[]`. لاحظ أن الفهرس يبدأ من الصفر، لذا إذا كنت تريد الوصول إلى العنصر الثاني في القائمة، سيكون الفهرس 1.