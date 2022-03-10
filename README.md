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

#### Per sequence GC content

type | Реплика 1 | Реплика 2 | Контроль
--- | --- | --- | ---
Not trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_1.png)
Trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_tr_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_tr_1.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_tr_1.png)

#### Per base sequence content

type | Реплика 1 | Реплика 2 | Контроль
--- | --- | --- | ---
Not trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_2.png)
Trimmed | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/1_tr_2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/2_tr2.png) | ![](https://github.com/ruanmik/hse_hw2_chip/blob/main/images/3_tr_2.png)

Указать, если была необходима фильтрация или подрезание чтений (и если это было сделано и как).

---
### №2 Статистика

type |  Число ридов| Число уникальных | Число не уникальных | Число не выровненных
--- | :---: | :---: | :---: | :---:
Реплика 1 | 50264294 | 43325108 (86.19%) | 2173187 (4.32%) | 4765999 (9.48%)
Реплика 2 | 61180707 | 2651628 (4.33%) | 5870380 (9.60%) | 52658699 (86.07%)
Контроль  | 13562825 | 613198 (4.52%) | 1817305 (13.40%) | 11132322 (82.08%)

---
### №3 Диаграммы Вена

