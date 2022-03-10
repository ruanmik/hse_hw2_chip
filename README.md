# hse_hw2_chip

[Ссылка на колаб]()

Параметры, выбранные на дз:

  * Клеточная линия - Loucy
  * Гистоновая Метка - H3F3A
  * Реплика 1 - ENCFF283SYC
  * Реплика 2 - ENCFF680PUD
  * Контроль -  ENCSR648HLP
---
### №1 FastQC 
#### Sequence length distribution 

type | Реплика 1 | Реплика 2 | Контроль
--- | --- | --- | ---
Not trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_.png)
Trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_tr.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_tr.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_tr.png)

Вывод: видим, что проблем нет ни для одной из реплик, но все ломается, если начинаем подрезать чтения. 

#### Per sequence GC content

type | Реплика 1 | Реплика 2 | Контроль
--- | --- | --- | ---
Not trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_1.png)
Trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_tr_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_tr_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_tr_1.png)

Выводы: Для всех трех чтений распределения близки к теоретическим, подрезание не влияет. 

#### Per base sequence content

type | Реплика 1 | Реплика 2 | Контроль
--- | --- | --- | ---
Not trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_2.png)
Trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_tr_2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_tr2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_tr_2.png)

Вывод: видим разбиение на две группы: тимин, аденин и цитозин, гуанин. Для всех случаев они остаются примерно на одном уровне в пределах нормы. Не меняется в trimmed версиях. 

##### Общий вывод: подрезания и фильтрация не нужны, тк судя по отчетам это не улучшает качество, а в случае с Sequence length distribution даже ухудшает. 

---
### №2 Статистика

type |  Число ридов| Число уникальных | Число не уникальных | Число не выровненных
--- | :---: | :---: | :---: | :---:
Реплика 1 | 50264294 | 2173187 (4.32%) | 4765999 (9.48%) | 43325108 (86.19%)
Реплика 2 | 61180707 | 2651628 (4.33%) | 5870380 (9.60%) | 52658699 (86.07%)
Контроль  | 13562825 | 613198 (4.52%) | 1817305 (13.40%) | 11132322 (82.08%)

Низкий процент уникольных риидов, объясняется тем, что выравниваем только на 1 хромосому

---
### №3 Диаграммы Вена
Реплика 1 | Реплика 2
--- | ---
![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/SYC1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/PUB.png)
![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/SYC2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/PUB2.png)

Различие в пересечениях связано с неуникальными позициями пиков. Пересечения небольшие, тк выравниваем на 1 хромосому
