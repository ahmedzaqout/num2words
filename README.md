num2words - Convert numbers to words in multiple languages

num2words is a library that converts numbers like 42 to words like forty-two. It supports multiple languages (Arabic,English, French, Spanish, German and Lithuanian) and can even generate ordinal numbers like اثنان وأربعون .

The project is hosted on https://github.com/ahmedzaqout/num2words

Installation

1-The easiest way to install num2words is to use clone:

git clone https://github.com/ahmedzaqout/num2words.git

2- install bidi

pip install python-bidi

3- install reshaper

pip install git+https://github.com/mpcabd/python-arabic-reshaper

Usage

to use:

>>>from bidi.algorithm import get_display

>>>import arabic_reshaper

>>>from bidi.algorithm import get_display

>>>from num2words import num2words

>>>print get_display(arabic_reshaper.reshape(num2words(550,lang='ar')))

خمسمائة وخمسون


>>>print get_display(arabic_reshaper.reshape(num2words(100125,lang='ar')))

مائة ألف ومائة وخمسة وعشرون





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

