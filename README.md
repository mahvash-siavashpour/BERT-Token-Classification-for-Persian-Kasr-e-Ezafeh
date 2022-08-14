
# BERT Token Tagger for Persian Kasr-e Ezafeh
Each persion word in a sentance either has a Kasr-e Eafeh or it does not. Kas-e Ezafeh comes in 3 different forms as shown bellow:
- @e
- e 
- ve 
- y 
- ye

Using a BERT token classification model from pretrained ```HooshvareLab/distilbert-fa-zwnj-base``` enables us to train the model on this specific task. The dataset could not be published due to copyright but this is a sample of what it looks like:
```
سلسله	ye
ایرانی	O
در	O
سوادکوه	e
مازندران	O
حکومت	O
می‌کردند	O
.	O
نفوذ	e
برامکه	O
)	O
وزرای	ye
ایرانی	O
(	O
در	O
دربار	e
عباسی	O
```

Each token of the data has a label indicating its Kasr-e Ezafeh. Tokens without a tag are labeled as O .
