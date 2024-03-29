# Умник. Заявка. Черновик.
## Направление заявки
Н1. Информационные технологии

## Полуфинал
Полуфинал программы УМНИК ТЕХНЕТ

## Приоритетное направление
Информационно-телекоммуникационные системы

## Критическая технология федерального уровня
???

## Название проекта
Электронный ультразвуковой стетоскоп

## Ключевые слова
Информационная система, автоматизированная медицинская диагностика, машинное обучение, цифровая обработка сигналов.

## Участие в других проектах
Медтех хакатон, разработка сайта-агрегатора для медицинских товаров

## Цель выполнения НИР
Создание цифрового стетоскопа, который позволяет регистрировать не только слышимый звук, но и ультразвук до 50-60 кГц.

## Назначение научно-технического продукта (изделия и т.п.)
- частные мед. учреждения
- государственные 
- глав врачи
- мед вузы
- использование самими пациентами в рамках телемедицины
Продукт предназначен для частных медицинских учреждений. Стетоскоп позволит врачам работать с более объективной информацией по сравнению с обычным прослушиванием. (решает проблему субъективности в постановке диагноза)

## Научная новизна предлагаемых в проекте решений
Написать впервые тут везде.
Аналоги на рынке регистрируют звук максимум до 10кГц. (плюс они имеют высокую цену) Также малоизучено применение машинного обучения для сигналов стетоскопа. Хорошая модель нейронной сети позволит значительно упростить медицинскую диагностику некоторых заболеваний.

## Обоснование необходимости проведения НИР
5/10 причин смерти по данным ВОЗ - заболевания сердца и легких. Необходимы исследования и новые решения в области диагностики этих заболеваний.

## Основные технические параметры, определяющие количественные, качественные и стоимостные характеристики продукции (в сопоставлении с существующими аналогами, в т.ч. мировыми)
- Цифровой стетоскоп, позволяющий регистрировать и обрабатывать сигнал от 16 до 40кГц. (ультразвук). 
- Прибор построен на базе Arduino Due (цена $37.40) и операционного усилителя MCP6022
- кроссплатформенное ПО для устройства (Python, PyQt, pyqtgraph, Numpy, Scipy, Matplotlib, pyFFTW, pyCUDA)

### характеристики микрофона SWEN MK-200
- Чувствительность, дБ           -60 ± 3                    
- Диапазон частот, Гц            50 – 16 000               
- Размер микрофонного модуля, мм 9×7                       
- Тип разъема                    мини-джек Ø 3,5 мм (3 pin)
- Длина кабеля, м                1,8                       
- Вес, г                         63          

### Технические характеристики операционного усилителя MCP6022
- Полоса частот           10МГц           
- Уровень шума            8.7 нВ/√Гц      
- Количество каналов      2               
- Напряжение питания      2.5В --- 5.5В   
- Напряжение смещения     $\pm500\mu V $  
- Гармонические искажения 0.00053\%       
- Температурный диапазон  -40°C --- +85°C 
- Тип корпуса             SO-8 

### Технические характеристики АЦП Arduino Due
- Число аналоговых входов            12                   
- Максимальная частота дискретизации 1МГц                 
- Объем буффера памяти               512 KB 
- Разрядность                        12бит (4096 значений)
- Рабочее напряжение                 3.3V                 
- Диапазоны входного напряжения      7-12V                
- Защита по входному напряжению      6-16V                
- Интерфейс                          USB
- Микроконтроллер                    AT91SAM3X8E
- Масса                              36г                 

## Область применения
Медицинская диагностика. Аускультация. обучение диагностике в медицинских ВУЗах, среднее медицинское образование, медицинские исследования

## План реализации
- пока хз??? уже ведь что-то есть
**8 пунктов / 2 года / 4 квартала**

изучить
разработать
протестирвать
напр. Изучение спектр хар-к дыхательных шумов
- разработка и тестирование фильтров
- тестирование на пациентах/добровольцах
