num2words - Convert numbers to words in multiple languages

num2words is a library that converts numbers like 42 to words like forty-two. It supports multiple languages (English, French, Spanish, German and Lithuanian) and can even generate ordinal numbers like forty-second (altough this last feature is a bit buggy at the moment).

The project is hosted on https://github.com/ahmedzaqout/num2words

Installation

The easiest way to install num2words is to use clone:

git clone https://github.com/ahmedzaqout/num2words.git

Usage

There's only one function to use:


>>>from bidi.algorithm import get_display
>>>import arabic_reshaper
>>>from bidi.algorithm import get_display
>>>from num2words import num2words
>>>print get_display(arabic_reshaper.reshape(num2words(550,lang='ar')))
خمسمائة وخمسون



lang: The language in which to convert the number. Supported values are:
    
    en (English, default)
    ar(Arabic)
    fr (French)
    de (German)
    es (Spanish)
    lt (Lithuanian)
    lv (Latvian)
    en_GB (British English)
    en_IN (Indian English)
    no (Norwegian)
    pl (Polish)
    ru (Russian)
    dk (Danish)
    pt_BR (Brazilian Portuguese)
    he (Hebrew)
    it (Italian)

