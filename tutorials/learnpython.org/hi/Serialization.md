Python अंतर्निर्मित JSON पुस्तकालय प्रदान करता है JSON को एन्कोड और डिकोड करने के लिए।

Python 2.5 में, simplejson मॉड्यूल का उपयोग किया जाता है, जबकि Python 2.7 में json मॉड्यूल का उपयोग किया जाता है। चूंकि यह इंटरप्रेटर Python 2.7 का उपयोग करता है, इसलिए हम json का उपयोग करेंगे।

json मॉड्यूल का उपयोग करने के लिए, पहले इसे आयात किया जाना चाहिए:

JSON डेटा के दो बुनियादी प्रारूप हैं। या तो एक स्ट्रिंग में या ऑब्जेक्ट डेटा संरचना में। ऑब्जेक्ट डेटा संरचना, Python में, सूचियों और स्थानों से मिलकर बनी होती है जो एक-दूसरे के अंदर स्थित होती हैं। ऑब्जेक्ट डेटा संरचना एक को पायथन विधियाँ (सूचियों और स्थानों के लिए) का उपयोग करने की अनुमति देती है ताकि डेटा संरचना से तत्त्व जोड़, सूचीबद्ध, खोज और हटाया जा सके। स्ट्रिंग प्रारूप मुख्य रूप से डेटा को किसी अन्य प्रोग्राम में पास करने या डेटा संरचना में लोड करने के लिए उपयोग किया जाता है।

JSON को डेटा संरचना में वापस लोड करने के लिए, "loads" विधि का उपयोग करें। यह विधि एक स्ट्रिंग लेती है और इसे वापस JSON ऑब्जेक्ट डेटा संरचना में बदल देती है:

JSON को डेटा संरचना में एन्कोड करने के लिए, "dumps" विधि का उपयोग करें। यह विधि एक ऑब्जेक्ट लेती है और एक स्ट्रिंग लौटाती है:

Python एक Python स्वामित्व वाले डेटा अनुक्रमण विधि का समर्थन करता है जिसे pickle कहा जाता है (और एक तेज विकल्प जिसे cPickle कहा जाता है)।

आप इसका उपयोग बिल्कुल उसी तरह कर सकते हैं।

इस अभ्यास का उद्देश्य JSON स्ट्रिंग के साथ "Me" : 800 कुंजी-मूल्य जोड़ी जोड़ा गया प्रिंट करना है।