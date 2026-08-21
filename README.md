# Хранилище CV

## Info
- Исходный источник резюме формата `.tex`: https://github.com/sb2nov/resume
- Редактор Overleaf: https://www.overleaf.com

## Структура

- `.tex/` — исходники резюме с разделением на `General/`, `Java/` и `.NET/`.
- `.pdf/` — готовые PDF с таким же разделением на `General/`, `Java/` и `.NET/`.
- `Other/` — прочие материалы, которые не относятся к форматам `.tex` и `.pdf`.
- `.tex/cvstyle.sty` — общие пакеты, геометрия страницы и команды форматирования для всех версий.

Файл `cvstyle.sty` находится в корне `.tex/` как общая зависимость и подключается из резюме через `../cvstyle`. Для локальной сборки перейдите в папку нужного направления, например:

```sh
cd .tex/Java
pdflatex -output-directory=../../.pdf/Java CV_Java.tex
pdflatex -output-directory=../../.pdf/Java CV_Rus_Java.tex

cd ../.NET
pdflatex -output-directory=../../.pdf/.NET CV_DotNet.tex
pdflatex -output-directory=../../.pdf/.NET CV_Rus_DotNet.tex
```

При загрузке проекта в Overleaf сохраняйте эту структуру и выбирайте нужный `.tex`-файл как Main document.
