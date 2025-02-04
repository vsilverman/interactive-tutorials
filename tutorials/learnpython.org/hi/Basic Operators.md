यह अनुभाग बताता है कि Python में बेसिक ऑपरेटर्स का उपयोग कैसे करें।

### गणितीय ऑपरेटर        

जैसे कि अन्य प्रोग्रामिंग भाषाओं में, जोड़, घटाव, गुणा, और भाग ऑपरेटरों का उपयोग संख्याओं के साथ किया जा सकता है।<br>

    number = 1 + 2 * 3 / 4.0
    print(number)

अनुमान लगाएँ कि उत्तर क्या होगा। क्या पायथन ऑपरेशन्स के क्रम का पालन करता है?

एक अन्य ऑपरेटर है मोड्यूलो (%) ऑपरेटर, जो भाग के पूर्णांक बचे हुए को लौटाता है। भाजक % भाजक = शेषफल।

    remainder = 11 % 3
    print(remainder)

दो गुणन चिन्हों का उपयोग एक घात्क संबंध बनाता है।

    squared = 7 ** 2
    cubed = 2 ** 3
    print(squared)
    print(cubed)

### स्ट्रिंग्स के साथ ऑपरेटर का उपयोग करना

Python संयोजित करने के लिए स्ट्रिंग्स के साथ जोड़ ऑपरेटर का समर्थन करता है:

    helloworld = "hello" + " " + "world"
    print(helloworld)

Python स्ट्रिंग्स को गुणा करके बार-बार आने वाला अनुक्रम बनाने के लिए समर्थन करता है:

    lotsofhellos = "hello" * 10
    print(lotsofhellos)

### सूचियों के साथ ऑपरेटर का उपयोग करना

सूचियों को जोड़ ऑपरेटर के साथ जोड़ा जा सकता है:

    even_numbers = [2,4,6,8]
    odd_numbers = [1,3,5,7]
    all_numbers = odd_numbers + even_numbers
    print(all_numbers)

जैसे कि स्ट्रिंग्स में, Python समर्थन करता है एक नए सूची बनाने के लिए पुनरावृत्ति वाले अनुक्रम के साथ गुणा ऑपरेटर का उपयोग करना:

    print([1,2,3] * 3)

Exercise
--------

इस अभ्यास का उद्देश्य `x_list` और `y_list` नामक दो सूचियाँ बनाना है,
जो `x` और `y` वेरिएबल्स की 10 बार उपस्थितियों को शामिल करती हैं।
आपको एक `big_list` नामक सूची भी बनानी है, जो 
आपकी बनाई गई दो सूचियों को जोडकर `x` और `y` वेरिएबल्स को 10 बार प्रत्येक को शामिल करती है।