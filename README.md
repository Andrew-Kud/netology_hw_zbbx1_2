# Домашнее задание к занятию "`Система мониторинга Zabbix. Часть 2`" - `Кудряшов Андрей`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1

<img width="2554" height="788" alt="1" src="https://github.com/user-attachments/assets/8311b3af-b086-4a2b-8975-8c56751d0eca" />



---

### Задание 2-3

<img width="2548" height="658" alt="2" src="https://github.com/user-attachments/assets/971b1e80-6db6-4238-ad7a-e0b4be57394a" />



---

### Задание 4

<img width="1164" height="1120" alt="3" src="https://github.com/user-attachments/assets/acf793d2-fbdc-458e-a518-9b4780cbb6e0" />



---

### Задание 5

<img width="1550" height="1096" alt="4" src="https://github.com/user-attachments/assets/dc3f5bef-d8c6-4633-96c5-3c7044c70d44" />



---

### Задание 6

<img width="2043" height="306" alt="5" src="https://github.com/user-attachments/assets/6e33bd4f-5834-4053-9b32-23fcf6b41581" />

```
#!/bin/bash


if [ -z "$1" ]; then
  exit 1
fi

case "$1" in
  1)
    echo "Kudryashov Andrey Sergeevich"
    ;;
  2)
    echo $(date)
    ;;
esac

```



---

### Задание 7

<img width="2501" height="630" alt="6" src="https://github.com/user-attachments/assets/5f4f50ae-0bce-49b7-93f8-1f5a03b5a475" />

<img width="2188" height="367" alt="7" src="https://github.com/user-attachments/assets/8c39703d-c3a5-41ae-9263-ea4d5e06744a" />

```
import sys
import os
import re
from datetime import datetime

if (sys.argv[1] == '-ping'):
    result=os.popen("ping -c 1 " + sys.argv[2]).read()
    result=re.findall(r"time=(.*) ms", result)
    print(result[0])

elif (sys.argv[1] == '-simple_print'):
    print(sys.argv[2])

elif (sys.argv[1]) == '1':
    print ("Kudryashov Andrey Sergeevich")
elif (sys.argv[1]) == '2':

    print(datetime.now().strftime("%a %b %d %H:%M:%S %Y"))
else: # Во всех остальных случаях
    print(f"unknown input: {sys.argv[1]}")

```



---

### Задание 8

<img width="2560" height="513" alt="8" src="https://github.com/user-attachments/assets/41a6049f-03bb-4009-97bb-d6b0b7143334" />

<img width="2560" height="605" alt="9" src="https://github.com/user-attachments/assets/b8e476b7-be20-4dd8-a470-d3e27beb295c" />

<img width="2560" height="642" alt="10" src="https://github.com/user-attachments/assets/2afa19bd-2c75-4bd8-96b3-641ee84dc42a" />

<img width="2560" height="626" alt="11" src="https://github.com/user-attachments/assets/3d3524e7-ecd1-4353-bc71-ab809e6dc7dd" />


---


