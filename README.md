# Хранилище CV

## Info
- Исходный источник резюме формата `.tex`: https://github.com/sb2nov/resume
- Редактор Overleaf: https://www.overleaf.com

## Структура

- `CV_Java.tex` — английская Java-версия.
- `CV_DotNet.tex` — английская .NET-версия.
- `CV_Rus_Java.tex` — русская Java-версия.
- `CV_Rus_DotNet.tex` — русская .NET-версия.
- `cvstyle.sty` — общие пакеты, геометрия страницы и команды форматирования.

Файл `cvstyle.sty` должен находиться рядом с основными `.tex`-файлами, в том числе при загрузке проекта в Overleaf.

## Сборка

Документы рассчитаны на компиляцию с помощью pdfLaTeX:

```sh
pdflatex CV_Java.tex
pdflatex CV_DotNet.tex
pdflatex CV_Rus_Java.tex
pdflatex CV_Rus_DotNet.tex
```
