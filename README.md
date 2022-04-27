- 👋 Hi, I’m @RafaelSaf2022
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
RafaelSaf2022/RafaelSaf2022 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
print('Генерация случайной последовательности')
import numpy as np
my_list = np.random.randint(0, 32, 10)
print(my_list)
lat = 'АБВГДЕЖЗИЙКЛМНОПРСТУФХЦЧШЩЪЫЬЭЮЯ'
text = str(my_list)
i = 0
s = ""
for a in text:
    if "0" <= a <= "9":
        s += a
        continue
    elif s != "":
        text = text.replace(s, lat[int(s) - 1])
    s = ""
print('Замена цифр буквами')
print(text)

def listsum(my_list):
    theSum = 0
    for i in my_list:
        theSum = theSum + i
    return theSum
print('Подчсет общей суммы случайной последовательности')
print(listsum(my_list))
