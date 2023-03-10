< [на главную](./readme.md)
___

## **Git commit**

___


Команда **git commit** - это точка фиксации изменений.

### **Как сделать коммит**
Представим, что нам нужно добавить пару новых блоков в html-разметку (index.html) и стилизовать их в файле style.css. Для сохранения изменений, их необходимо закоммитить. Но сначала, мы должны обозначить эти файлы для Гита, при помощи команды **git add**, добавляющей (или подготавливающей) их к коммиту.

```bash=
git add index.html
git add css/style.css
```
Или вместе-всё сразу:

```bash=
git add .
```

Конечно добавлять всё сразу удобнее, чем прописывать каждую позицию отдельно. Однако, тут надо быть внимательным, чтобы не добавить по ошибке ненужные элементы. Если же такое произошло изъять оттуда ошибочный файл можно при помощи команды

```bash=
git reset:
git reset css/style.css
```

Теперь создадим непосредственно сам коммит

```bash=
git commit -m 'Add some code'
```
Флажок **-m** задаст ***commit message*** - комментарий разработчика. Он необходим для описания закоммиченных изменений. И здесь работает золотое правило всех комментариев в коде: **«Максимально ясно, просто и содержательно обозначь написанное!»**