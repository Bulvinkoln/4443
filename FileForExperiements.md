Вторая попытка объединить файлы в конфликте

## У меня было </br>
&ensp;&ensp;`*` master </br>
&ensp;&ensp;`|` </br>
&ensp;&ensp;`*` master </br>
`/ | \` </br>
`* | *`&ensp; New_First_Branch `|` New_Second_Branch </br>
`| | |`

## Теперь у меня так <br>
`*` master </br>
`|` </br>
`*` master </br>
`| \` <br>
`| *` New_First_Branch<br>
`| |`<br>
`| *` New_First_Branch <br>
`| | \` <br>
`| | *` New_Second_Branch <br>
`| | |`

А также я планирую добавить вторую запасную ветку, и объединить первую во вторую, т.е. вторая должна перезаписаться. А если она опять убьет моё сохранение, то у меня будет вторая запасная вторая ветка

## Планирую сделать так:
Теперь у меня так <br>
`*` master </br>
`|` </br>
`*` master </br>
`| \` <br>
`| *` New_First_Branch<br>
`| |`<br>
`| *` New_First_Branch <br>
`| | \` <br>
`| | *` New_Second_Branch <br>
`| | |` <br>
`| | *` New_Second_Branch <br>
`| | | \` <br>
`| | | *` New_Second_Branch_Saved <br>
`| |\| |` <br>
`| | * |` ***Conflict*** <br>
`| x/ /` ***deleted New_First_Branch_Saved*** <br>
`| / /` <br>
`* | |` ***master*** <br>
`| * |` ***New_Second_Branch*** <br>
`| | *` ***New_Second_Branch_Saved*** <br>

git merge:
>Этот текст создаст конфликт при объединении двух файлов. При соединении двух веток, хочу оставить это решение, а мб какое-нибудь другое. Я не помню как разрешать конфликты в файлах

>Похоже я неправильно сделал, потому что он удалил мой красивый файл без конфликта =(

### Сработало!