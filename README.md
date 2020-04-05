# Как это работает?

Делайте pull request'ы в этот репозиторий и добавляйте информацию из чата, что считаете полезной.

Собрана вся информация до 23 февраля.

# TODO

* Собрать из каждой ссылки картинку
* Объяснить проекты всех участников

# Проекти участников чата

## foo52ru

## Юрий Морозов

https://vk.com/im?msgid=254196&sel=c65&z=video98079552_456239197%2F2d962261c860901246

https://vk.com/im?msgid=254196&sel=c65&z=video98079552_456239198%2Fd1c2768f4b4114d9be

https://vk.com/im?msgid=254196&sel=c65&z=video98079552_456239199%2F036b01ad3eaaf702d6

[](/other/Evo.rar)

https://vk.com/videos192023607?z=video98079552_456239217/6396ba3060b2b458d2

https://vk.com/videos192023607?z=video98079552_456239218/1096f32b39f0d1f9d1

## Артём Яшин (Онигири)

https://www.youtube.com/watch?v=JaPwn-pvHTs

https://youtu.be/v5f6fz3a9Ho

https://vk.com/video170014997_456239211?list=cf0655e468f18b6c16

https://vk.com/im?msgid=254196&sel=c65&z=video170014997_456239212%2F59a99415957e21a34a

https://vk.com/video170014997_456239217?list=d13258b0eb1c1e092d

https://vk.com/video170014997_456239220?list=63c0196faf32e46ff4

![](/img/4.jpg)

https://youtu.be/KLv0Z43ijyQ

## Даниил Редчин

## Илья Шепрут

https://optozorax.github.io/evolved-virtual-creatures

https://github.com/optozorax/crabots

https://vk.com/im?msgid=254196&sel=c65&z=video192023607_456239276%2F27f3152e8f12ade10f


![](/img/2.jpg)

https://optozorax.github.io/crabots/www_28_01_2020/index.html

https://t.me/optozorax_dev/21

https://optozorax.github.io/crabots/www_0.2.1/index.html

https://optozorax.github.io/crabots/www_0.2.2/index.html

https://optozorax.github.io/crabots/www_0.2.2/index.html?help

https://optozorax.github.io/crabots/www_0.2.2/index.html?a=2

https://optozorax.github.io/crabots/www_0.2.2/index.html?p=100000000

https://optozorax.github.io/crabots/www_0.2.2/index.html?t=HorizontalCylinder

https://optozorax.github.io/crabots/www_0.2.2/index.html?t=HorizontalCylinder

https://optozorax.github.io/crabots/www_0.2.2/index.html?w=400&g=100&p=10000000&o=10000000&c=10000000

https://optozorax.github.io/crabots/www_0.2.2/index.html?t=ololo

https://optozorax.github.io/crabots/www_0.2.7/index.html?r=Vec&t=Rect&p=1000000&o=1000000&c=1000000&a=2

https://vk.com/videos192023607?z=video98079552_456239216/e77b6683e5e5a61a98

https://optozorax.github.io/crabots/www_0.2.8/index.html?k=true

## Евгений Барышников

## Владислав Фёдоров

https://github.com/MrOmnomnoshka/Genetic-Algorithms

## Сергей Фирсов
**BacterialSim** - симуляций жизни и развития бактериальной колонии.
Проект преследует следующие цели:
  * Моделирование мутационной изменчивости.
  * Влияние окружающей среды на изменчивость.
  * Построение замкнутой экосистемы.
  * Формирование взаимодействия между клетками.

https://github.com/SergeyFi/BacterialSim


[![](http://img.youtube.com/vi/hW4k6FEcNGk/0.jpg)](http://www.youtube.com/watch?v=hW4k6FEcNGk "")

[![](http://img.youtube.com/vi/tScBNoew2s8/0.jpg)](http://www.youtube.com/watch?v=tScBNoew2s8 "")

![](/img/BacterialSim.jpg)



## Александр Мясников

Исходный код: https://github.com/alexandermyasnikov/genesis

Genesis: краткое описание
* Мир - прямоугольная область, состоящая из клеток.
* В мире генерируются разные ресурсы, необъодимые ботам для жизни.
* В одной клетке может находиться один бот.
* Бот содержит геном, которые определяет его поведение.
* Бот может хранить в себе ресурсы и обмениваться ими с окружающей средой.
* Бот может преобразовывать одни ресурсы в другие.
* Бот может атаковать других ботов.
* Время жизни бота ограничено.

![Genesis. Demo v0.4](/img/amyasnkov_genesis_v0.4.gif)



# Проблемы симуляции ботов

## Изотропность пространства

Допустим, мы хотим, чтобы правила работали одинаково в независимости от направления. Но тут появляется такая ситуация: две клетки хотят переместиться в одну и ту же между ними

![](/img/1.jpg)

Решения:
* Не решать. Тогда будут артефакты в поведении ботов, и желательно обрабатывать их в случайном порядке, а не по порядку расположения на поле.
* Можно давать приоритет той, у которой больше энергии или вообще случайной, но в таком случае нужны дополнительные проверки и возврат к предыдущим клеткам, а это плохо для производительности
* Запрещать обоим, и желательно на какой-то нейрон послать сигнал что произошла такая коллизия.

## Отделение отрисовки от логики

Для визуализации вместо интерфейса можно просто выводить данные в картинку или гифку.

Это отлично подходит на первых этапах разработки.

Только надо заранее заботиться о подключении библиотек для работы с гифками и png'шками.И париться насчёт библиотек, которые рисуют графику в картинку в памяти, а не на экран напрямую.

Кстати, это ещё и позволяет вам организовать вычисления таким образом, чтобы они не зависели от визуализации.

Ведь если бы эта эволюция запускалась в фоне, то она бы работала в 100 раз быстрее, и результат можно было получить в 100 раз быстрее!

Либо можно так не заморачиваться и сделать пропуск кадров.

Ещё плюс такого подхода в том, что если ты рисуешь слишком сложную графику с тысячами ботов, например, то визуализация риалтайм не позволит тебе получить 60 фпс. Если же ты будешь сохранять это в картинки, то тебя может никак не колыхать производительность, ты просто сохраняешь картинки, а потом монтируешь это в 60 фпс.

В любом случае архитектуру надо изначально планировать так, чтобы графика могла быть полностью выключена, и чтобы она не была составной частью эволюции.

## Как рисовать ботов с учётом масштабирования и повторяемости мира?

Можно рисовать наоборот: не рисовать мир на экране, а рисовать экран на мире.

Конкретно:
* Перебираем каждый пиксель
* Пытаемся определить координаты на плоскости мира с учётом масштаба и смещения
* Делим координаты по модулю, и вообще приводим их к ограничениям мира
* Смотрим куда координаты упали в массиве мира
* И рисуем цветом бота, который там находится

Но это дорого по производительности, зато быстро по написанию.

## Публикация видео на ютубе

Перед тем как публиковать видео о эволюции ботов на ютубчик, посмотрите это видео:
https://www.youtube.com/watch?v=r6Rp-uo6HmI

Из него следует, что надо публиковать с максимальным возможным качеством, даже если изначальное было 480р, чтобы сжатие не мешало просмотру.

У foo52ru к сожалению качество 480р, поэтому на видео с ботам много артефактов и сложно что-то рассмотреть.

# Сравнение языков программирования

## Python

pygame - для рисования

> В питоне что плохо:
> Я работал в одной всем известной компании, и там у меня была задача сделать одну штуку на питоне. Эта штука должна была крутиться 24 на 7 и выполнять маленькую работу. Когда я написал эту прогу, я понял что я не могу быть уверенным что она не вылетит на тех ветках ифа, которые я не проверял... В итоге пришлось очень тщательно тестировать её: перебирать все ветки ифа, чтоб быть уверенным, что там не будет ошибки типов. Поэтому в продакшене питон лучше не использовать, а то взорвётся и мало не покажется.
> Это вообще проблема всех динамически типизированных языков: питон, жс.
> Языки со статической типизацией такую проблему решают на этапе компиляции.
> Не зря же вместо js начинают активно юзать typescript с типами данных.

## C/C++

sfml

## C#

## Java

## Rust

## JavaScript

# Мемы

![](/img/3.jpg)

# Интересные ссылки

https://www.youtube.com/watch?v=khWqdZ4Z22Y

https://www.youtube.com/watch?v=aircAruvnKk&list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi&index=1

https://vimeo.com/196269431

https://youtu.be/xP5-iIeKXE8

https://meduza.io/feature/2020/01/16/meduzoid-iz-serdtsa-krysy-i-kiborgi-iz-lyagushachiey-ikry

https://www.reddit.com/r/interestingasfuck/comments/eqtocl/this_formation_allows_fish_to_feed_and_guard_by/?utm_medium=android_app&utm_source=share

https://www.redblobgames.com/grids/hexagons/

http://alife.org/

https://twitter.com/algoritmic/status/1219553552227500032

https://twitter.com/SasaBudimir/status/1221783288731328512

https://twitter.com/SmartBiology3D/status/1229090958706388992
