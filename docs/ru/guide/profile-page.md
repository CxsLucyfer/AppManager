---
sidebarDepth: 2
---

# Страница профилей
Страница профиля отображает настройки профиля. Эта страница так же предлагает редактирование профиля(ей).

::: tip Подсказка
При применении профиля некоторые пакеты не соответствуют критериям, они просто игнорируются.
:::

::: details Таблица содержания
[[toc]]
:::

## Меню опций
Три точки в правом верхнем углу открывают меню параметров. Оно содержит несколько параметров, таких как:
- **Применить.**  Эта опция может использоваться для применения профиля. При нажатии появится диалоговое окно, в котором вы можете выбрать [состояние профиля][state]. При выборе одного из параметров профиль будет применяться немедленно.
- **Сохранить.** Позволяет сохранить профиль.
  ::: warning предупреждение
  Изменения никогда не сохраняются автоматически. Вы должны сохранить их вручную.
  :::
- **Отменить.** Отменить любые изменения, сделанные с момента последнего сохранения.
- **Удалить.** Нажатие на удаление удалит профиль немедленно и без предупреждения.
- **Дублировать.** Эта опция может быть использована для дублирования профиля. При нажатии отображается поле ввода, в котором можно указать имя профиля. При нажатии на кнопку "OK" будет создан новый профиль и страница будет перезагружена. Профиль не будет сохранён до тех пор, пока вы не сохраните его вручную.
- **Создать ярлык.** Эта опция может использоваться для создания ярлыка для профиля. При нажатии будут два варианта: _Простые_ и _Расширенные_. Последний вариант позволяет вам установить [состояние профиля][state] перед его применением, в то время как первый вариант использует состояние по умолчанию, которое было настроено при последнем сохранении профиля.

## Вкладка Приложения
На вкладке "Приложения" перечислены пакеты, настроенные под этим профилем. Пакеты могут быть добавлены или удалены с помощью кнопки _плюс_, расположенной в нижней части экрана. Пакеты также могут быть удалены при долгом нажатии на них (в этом случае отображается всплывающее окно с единственным параметром _удалить_).

## Вкладка Конфигурации
Вкладка конфигурации может быть использована для настройки выбранных пакетов. Описание каждого пункта приводится ниже:

### Комментарий
Это текст, который будет отображаться на странице [профили][profiles]. Если не установлено, текущие настройки будут показаны вместо этого.

### Состояние
Определяет как будут действовать определенные настроенные параметры. Например, если включен параметр _Отключить_, приложения будут отключены, если установлено _ВКЛ_ и будут включены, если установлено _ВЫКЛ_. В настоящее время состояние поддерживает только значения _ВКЛ_ и _ВЫКЛ_.

### Компоненты
Это работает так же, как опция [ Блокировать компоненты… ][block_components] на странице Операции в один клик. Однако, это применимо только к выбранным пакетам. Если [ состояние ][state] _ ВКЛ_, компоненты будут заблокированы, а если [состояние][state] _ ВЫКЛ_, компоненты будут разблокированы. Эту опцию можно отключить(независимо от вставленных значений), нажав на кнопку _отключить_ в диалоговом окне ввода.

_Смотрите также: [Что такое компоненты приложения?][what_are_components]_

### Операции приложения
This behaves the same way as the [Deny App Ops…][deny_app_ops] option does in the 1-Click Ops page. Однако, это относится только к выбранным пакетам. Если состояние ВКЛ, операции приложения будут отклонены, а если состояние ВЫКЛ, операции приложения будут разрешены. Эту опцию можно отключить (независимо от вставленных значений), нажав на кнопку _отключить_ в диалоговом окне ввода.

### Разрешения
Эта опция может быть использована для предоставления или отзыва определенных разрешений из выбранных пакетов. Как и в других выше, разрешения должны быть разделены пробелами. Если состояние ВКЛ, разрешения будут отозваны, а если состояние ВЫКЛ - будут разрешены. Эту опцию можно отключить (независимо от вставленных значений), нажав на кнопку _отключить_ в диалоговом окне ввода.

### Резервное копирование/восстановление
Эта опция может быть использована для создания резервной копии выбранных приложений и их данных или их восстановления. Доступны два варианта: _Параметры резервного копирования_ и _Имя резервной копии_.
- **Параметры резервного копирования.** То же самое, что и настройки резервного копирования/восстановления[][backup_options]. Если не установлено, будут использоваться параметры по умолчанию.
- **Имя резервной копии.** Задайте индивидуальное имя для резервной копии. Если установить имя резервной копии, каждый раз при создании резервной копии будет дано уникальное имя с именем резервной копии в качестве суффикса. Это поведение будет исправлено в будущих выпусках. Оставьте это поле пустым для обычного (базового) резервного копирования.

Если [состояние][state] _ВКЛ_, будут созданы резервные копии пакетов, а если [состояние][state] - _ВЫКЛ_, будет произведено восстановление пакетов. Эту опцию можно отключить, нажав на кнопку _отключить_ в диалоговом окне ввода.

### Экспорт правил блокировки
Эта опция позволяет экспортировать правила блокировки.

### Отключить
Включение этой опции включит/отключит выбранные пакеты в зависимости от [состояния][state]. Если [состояние][state] _ВКЛ_, пакеты будут отключены, и если [состояние][state] _ВЫКЛ_, пакеты будут включены.

### Принудительно остановить
Включение этой опции позволит принудительно остановить выбранные пакеты.

### Очистить кеш
Включение этой опции позволит очистить кэш для выбранных пакетов.

### Очистить данные
Включение этой опции включит очистку данных для выбранных пакетов.

### Блокировка трекеров
Включение этой опции будет блокировать/разблокировать компоненты трекера в выбранных пакетах в зависимости от [состояния][state]. Если [состояние][state] _ВКЛ_, трекеры будут заблокированы, а если [состояние][state] _ВЫКЛ_, трекеры будут разблокированы.

### Сохранить APK
Включение этой опции включит резервное копирование APK для выбранных пакетов. Это не то же самое, что описанное здесь [резервное копирование/восстановление][backup_restore].


[state]: #состояние
[profiles]: ./profiles-page.md
[block_components]: ./one-click-ops-page.md#блокировка-компонентов
[what_are_components]: ../faq/app-components.md#что-такое-компоненты-приложения
[deny_app_ops]: ./one-click-ops-page.md#установка-режима-для-операции-приложения
[backup_options]: ./backup-restore.md#параметры-резервного-копирования
[backup_restore]: ./backup-restore.md