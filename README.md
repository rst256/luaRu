# lua
Lua Ru 5.3.4 Русификация Lua, русские переменные, имена функций и операторы

https://тхаб.рф/wiki/Учебник_по_LuaRu - Учебник в процессе перевода!! по LuaRu

http://plana.mybb.ru/viewtopic.php?id=576 Обсуждение LuaRu 

исправленные файлы lctype.h и llex.c

== Русские синонимы англоязычных ключевых слов ==
(в скобках не реализованные варианты)

and - и

break - стоп 

do - начало (делать ?)

else - иначе

elseif - иначеесли (либо)

end - всё (конец ?)

false - ложь (+ нет) 

for - для

function - функция

goto - идина (посыл, перейти_к, выполнить_с ?)

if - если 

in - в 

local - локал

nil - нуль (пусто ?) 

not - не 

or - или

repeat - повторять (повторить)

return - возврат (вернутся)

then - тогда

true - истина (да)

until - покуда (?)

while - пока

--- Из llex.c---
* ORDER RESERVED */
static const char *const luaX_tokens [] = {
    "and", "break", "do", "else", "elseif",
    "end", "false", "for", "function", "goto", "if",
    "in", "local", "nil", "not", "or", "repeat",
    "return", "then", "true", "until", "while",
    "//", "..", "...", "==", ">=", "<=", "~=",
    "<<", ">>", "::", "<eof>",
    "<number>", "<integer>", "<name>", "<string>"
};
static const char *const luaX_tokens_cyr [] = {
    "и", "стоп", "начало", "иначе", "иначеесли",
    "все", "ложь", "для", "функция", "идина", "если",
    "в", "локал", "нуль", "не", "или", "повторять",
    "возврат", "тогда", "истина", "покуда", "пока"
};

==Как скомпилировать исходники==
