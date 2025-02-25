# Домашнее задание к занятию «Основы работы в MasterScada. Настройка OPC»

### Цель задания

Правильная настройка OPC-сервера и настроенная связь со SCADA-системой являются первым этапом к построению системы диспетчеризации и основой корректной работы SCADA-системы.

В результате выполнения задания вы сможете:

1. Изучить настройки OPC-серверов.
2. Изучить методы настройки обмена данными по Modbus протоколу.
3. Научиться определять формат взаимодействия с тегами «чтение/запись».
4. Научиться создавать проект в MasterSCADA.
5. Научиться подключать OPC-сервер к проекту MasterSCADA.

------

### Чеклист готовности к домашнему заданию

1. Доступ к сети Интернет
2. Наличие личного Google Диска

------

### Инструкция к заданию

1. Скачайте эмулятор ПЛК [Modbus Slave](https://www.modbustools.com/download.html) согласно [инструкции](https://docs.google.com/document/d/1I2sjAwapq-BwDyCT3sZbfYhMfNBALL6jJ4c5-oECevU/edit?usp=sharing), проведите установку ПО.
2. Откройте в Modbus Slave [проекты эмуляции ПЛК (4 шт.)](https://drive.google.com/drive/folders/1OXjO8pzdHCP9vEJVN65R6EN0GAurRmCg?usp=sharing) по [инструкции](https://docs.google.com/presentation/d/10vHAmEqL6PK2pcvGtXgm0Kb8tHrJsfkSvUf8jF0qyMQ/edit?usp=sharing).
3. Скачайте [MasterOPC](https://insat.ru/products/?category=1666) согласно [инструкции](https://docs.google.com/document/d/1GyRE9AtVmFUKmTHmrFAUws_D4Via7dIOoihddZAo-qM/edit?usp=sharing), проведите установку ПО.
4. Скачайте [MasterSCADA 4D](https://masterscada.ru/download4) согласно [инструкции](https://docs.google.com/document/d/1lB2ACRR5TrPz_S0To14f7vAOfKgDi3dimUQFa41Zai4/edit?usp=sharing), проведите установку ПО.
5. Выполните задания 1 и 2.
6. Для проверки домашнего задания преподавателем отправьте ссылку на ваш проект OPC-сервера в личном кабинете.
7. Любые вопросы по решению задач задавайте в чате учебной группы.

------

### Инструменты/ дополнительные материалы, которые пригодятся для выполнения задания

1. [Google Drive](https://www.google.com/intl/ru/drive/)
2. Эмулятор ПЛК - Modbus Slave:
- [Modbus Slave Install 64bit](https://www.modbustools.com/download/ModbusSlaveSetup64Bit.exe "ModbusSlave Install 64bit") 
- [Modbus Slave Install 32bit](https://www.modbustools.com/download/ModbusSlaveSetup32Bit.exe "ModbusSlave Install 32bit")
3. [Проекты эмуляции](https://drive.google.com/drive/folders/1OXjO8pzdHCP9vEJVN65R6EN0GAurRmCg?usp=sharing)
4. [MasterOPC](https://insat.ru/products/?category=1666)
5. [MasterSCADA 4D](https://masterscada.ru/download4)
6. Инструкции:
- [Инструкция по загрузке ПО Modbus Slave](https://docs.google.com/document/d/1I2sjAwapq-BwDyCT3sZbfYhMfNBALL6jJ4c5-oECevU/edit?usp=sharing)
- [Инструкция по работе с Modbus Slave](https://docs.google.com/presentation/d/10vHAmEqL6PK2pcvGtXgm0Kb8tHrJsfkSvUf8jF0qyMQ/edit?usp=sharing)
- [Инструкция по загрузке ПО MasterOPC](https://docs.google.com/document/d/1GyRE9AtVmFUKmTHmrFAUws_D4Via7dIOoihddZAo-qM/edit?usp=sharing)
- [Инструкция по загрузке ПО MastersSCADA 4D](https://docs.google.com/document/d/1lB2ACRR5TrPz_S0To14f7vAOfKgDi3dimUQFa41Zai4/edit?usp=sharing)

------

### Задание 1

1. В MasterOPC создайте OPC-сервер с доступом по OPC UA и подключите все теги из проектов Master Slave.
2. Запустите MasterOPC в режиме исполнения и проверьте обмен данными с MasterSlave (8-DI, 8-DO, 8-AI и 8-AO тегов).
3. Для тегов AI  применить функцию пересчета по формулам:
- для адреса 0 - 10*X
- для адреса 1 - 100*X
- для адреса 2 - пересчет по шкале в устройстве 0-100, реальное значение 0-500
- для адреса 3 - пересчет по шкале в устройстве 0-1000, реальное значение -100 - 100


------

### Задание 2

1. Создайте новый проект в MasterSCADA 4D.
1. Настройте связь с OPC UA-сервером, созданном в MasterOPC.
1. Загрузите все теги из OPC-сервера в проект MasterSCADA.
1. Настройте связь с OPC DA-сервером, созданном в MasterOPC.
1. Загрузите все теги из OPC-сервера в проект MasterSCADA.
1. Настройте связь с OPC HDA-сервером, созданном в MasterOPC.
1. Загрузите все теги из OPC-сервера в проект MasterSCADA.
1. Поверьте обмен данными в режиме исполнения MasterSCADA (Master Slave - MasterOPC - MasterSCADA).


------

### Правила приема работы

1. Файлы проектов MasterOPC и MasterSCADA размещены на личном Google Диске.
2. К файлам проектов MasterOPC и MasterSCADA на Google Диске настроены права доступа «Просматривать могут все в Интернете, у кого есть ссылка».
3. Отправлена ссылка на проекты MasterOPC и MasterSCADA (Google Диск) с выполненным заданием в личном кабинете.

------

### Критерии оценки

Зачет ставится, если созданный проект MasterSCADA соответствует следующим критериям:

1. В MasterOPC созданы OPC UA, OPC DA и OPC HDA-серверы.
1. В режиме исполнения MasterOPC отражаются изменения всех тегов из эмулятора ПЛК Modbus Slave согласно типу данных и режиму чтение/запись.
1. В MasterSCADA 4D создан проект.
1. В проекте MasterSCADA 4D настроена связь с OPC UA, DA и HDA MasterOPC.
1. В проекте MasterSCADA 4D загружены все теги из OPC сервера MasterOPC.
1. Для тегов AI применена функция пересчета:
- для адреса 0 - 10*X
- для адреса 1 - 100*X
- для адреса 2 - пересчет по шкале в устройстве 0-100, реальное значение 0-500
- для адреса 3 - пересчет по шкале в устройстве 0-1000, реальное значение -100 - 100

Работа направляется на доработку, если задание выполнено частично или не выполнено, в логике выполнения задания есть противоречия, существенные недостатки, нарушена методология.

