---
title: Википедия
description: Схема транслитерации Википедии
slug: wikipedia
---

Схема транслитерации, которую использует Википедия. Сделана на основе [BGN/PCGN](/bgn-pcdn)со значительными модификациями. Самая продуманная, звучит лучше всех и выглядит приятнее большинства прочих схем. Пожалуй, неудачной вышла только буква `Щ`.

📅 2005 • ✔️ действует • ⚪ без диакритики

Особенности:

-   Нечастое написание `Ё` как `YO`
-   Редчайшее написание `Ъ`, `Ы`, `Ь` как `Y`
-   Множество нюансов, самые сложные правила

<div class="tabs">
<input name="tabs" type="radio" id="text" checked="checked" class="input"/>
<label for="text" class="label"><span>Текст</span></label>
<div class="panel pre-group">
<pre data-ref="source" contenteditable="true" class="editable"><code>Юлия, съешь ещё этих мягких французских булок из Йошкар-Олы, да выпей алтайского чаю</code></pre>
<pre data-ref="target" data-schema="wikipedia"><code>Yuliya, syesh yeshchyo etikh myagkikh frantsuzskikh bulok iz Yoshkar-Oly, da vypey altayskogo chayu</code></pre>
</div>

<input name="tabs" type="radio" id="js" class="input"/>
<label for="js" class="label"><span>JavaScript</span></label>
<pre class="panel"><code>var source = "Юлия, съешь ещё этих мягких французских булок из Йошкар-Олы, да выпей алтайского чаю";
var result = iuliia.translate(source, iuliia.WIKIPEDIA);</code></pre>

<input name="tabs" type="radio" id="python" class="input"/>
<label for="python" class="label"><span>Python</span></label>
<pre class="panel"><code>import iuliia
source = "Юлия, съешь ещё этих мягких французских булок из Йошкар-Олы, да выпей алтайского чаю"
result = iuliia.translate(source, schema=iuliia.WIKIPEDIA)</code></pre>
</div>

## Правила

```
cyr  lat
а    a
б    b
в    v
г    g
д    d
е    ye,e
ё    yo
ж    zh
з    z
и    i
й    y
к    k
л    l
м    m
н    n
о    o
п    p
р    r
с    s
т    t
у    u
ф    f
х    kh
ц    ts
ч    ch
ш    sh
щ    shch
ъ    y
ы    y
ь    y
э    e
ю    yu
я    ya
```

Буква `Е` →

-   `YE` в начале слова (Ельцин → Yeltsin);
-   `YE` после гласных, `Ь`, `Ъ` (Раздольное → Razdolnoye, Юрьев → Yuryev);
-   `E` в остальных случаях (Белкин → Belkin).

Буква `И` → `I`, кроме окончаний на `-ИЙ`

Буква `Й` → `Y`, кроме окончаний на `-ИЙ` и `-ЫЙ` (Бийск → Biysk)

Буква `Ъ` →

-   опускается перед `Е`, `Ё`, `Ю`, `Я` (Подъярский → Podyarsky);
-   `Y` перед `А`, `И`, `О`, `У`, `Ы`, `Э` (Мусийкъонгийкоте → Musiykyongiykote).

Буква `Ы` → `Y`, кроме окончаний на `-ЫЙ` (Давыдов → Davydov)

Буква `Ь` →

-   опускается перед `Е`, `Ё`, `Ю`, `Я` (Усолье → Usolye);
-   опускается в конце слова (Выхухоль → Vykhukhol);
-   опускается перед согласной (Дальнегорск → Dalnegorsk);
-   `Y` перед `А`, `И`, `О`, `У`, `Ы`, `Э` (Ильинский → Ilyinsky).

Окончания:

-   `-ЫЙ` → `-Y` (Красный → Krasny)
-   `-ИЙ` → `-Y` в именах и русских прилагательных (Великий → Veliky)
-   `-ИЙ` → `IY` в существительных и нерусских названиях (Рыркайпий → Ryrkaypiy)
-   `-ЫЕ` → `YE` (Набережные Челны → Naberezhnye Chelny)

ℹ️ [wikipedia.org](https://en.wikipedia.org/wiki/Wikipedia:Romanization_of_Russian)
