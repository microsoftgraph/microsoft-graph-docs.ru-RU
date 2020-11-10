---
title: Компонент People-Picker
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 9f47824d62ee5ffcf57884af5e68b255756d5478
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975779"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>People-Picker компонент в наборе инструментов Microsoft Graph

Вы можете использовать `mgt-people-picker` веб-компонент для поиска людей и/или групп. По умолчанию компонент будет выполнять поиск всех людей и пользователей в Организации, но вы можете изменить поведение, чтобы также выполнить поиск групп или только групп. Вы также можете отфильтровать поиск в определенной группе.

## <a name="example"></a>Пример

В приведенном ниже примере показан `mgt-people-picker` компонент. Начните поиск имени, чтобы увидеть результаты, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Откройте этот пример в меню упр. dev.](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Свойства

По умолчанию `mgt-people-picker` компонент получает пользователей из `/me/people` `/users` конечных точек и. Используйте следующие атрибуты, чтобы изменить это поведение.

| Атрибут | Свойство | Описание                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Show — Max | шовмакс   | Числовое значение, указывающее максимальное число людей для отображения. значение по умолчанию — 6.                                                                                             |
| Идентификатор группы    | groupId     | Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.                                                                            |
| type     | type      | Тип сущностей для поиска. Доступные параметры: `person` , `group` , `any` . Значение по умолчанию: `person`. Этот атрибут не оказывает никакого действия `group-id` , если свойство задано.                                                                            |
| Тип группы     | groupType      | Тип группы для поиска. Доступные варианты: `unified` ,, `security` `mailenabledsecurity` , `distribution` , `any` . Значение по умолчанию: `any`. Этот атрибут не оказывает никакого действия, если `type` свойство имеет значение `person` .                                                                           |
|  Выбранные пользователи  | селектедпеопле     | Массив выбранных пользователей. Задайте это значение для программного выбора людей.|
| people   | people    | Массив людей, найденных и визуализированных в результатах поиска |
| по умолчанию — выбранные: Users ID | дефаултселектедусеридс | При указании строки с разделителями, разделенными запятыми, компонент отрисовывает соответствующих пользователей, как выбрано при инициализации.
| Выбор режима | selectionMode | Указывает, следует ли разрешить выбор нескольких пользователей или только одного пользователя. Доступны следующие параметры: `single` , `multiple` . Значение по умолчанию: `multiple`.
| нагляд | нагляд | Текст по умолчанию, поясняющий, как использовать компонент. Значение по умолчанию: `Start typing a name`.

Ниже приведен `show-max` пример.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>Выбранные люди

В разделе выбранные люди компонента отображается каждый пользователь, выбранный разработчиком или пользователем. 

![Центр управления "Выбор людей"](./images/selected-people.png)

Вы можете заполнить выбранные данные о людях, выполнив одно из следующих действий:

- `selectedPeople`Непосредственное задание свойства, как показано в следующем примере.  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- С помощью `selectUsersById()` метода, который принимает массив [идентификаторов пользователей](/graph/api/resources/users?view=graph-rest-1.0) Microsoft Graph, чтобы найти сведения о пользователе для выбора.

     >**Примечание:** Если для пользователя не найдено ни одного пользователя `id` , данные не будут отображены `id` .

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a>События

Из компонента порождаются следующие события.

| Событие | Описание |
| --- | --- |
| `selectionChanged` | Пользователь добавил или удалил пользователя из списка выбранных/выбранных пользователей.|

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

`mgt-people-picker`Компонент определяет следующие настраиваемые свойства CSS.

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a>Шаблоны

 `mgt-people-picker` поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента. Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| умолчани | NULL: нет данных | Шаблон, используемый для переопределения отображения всего компонента.
| загрузки | NULL: нет данных | Шаблон, используемый для отображения состояния средства выбора при запросе к Graph. |
| error | NULL: нет данных | Шаблон, используемый, если поиск пользователей не возвращает пользователей. |
| нет данных | NULL: нет данных | Альтернативный шаблон, используемый в случае, если поиск пользователей не возвращает пользователей. |
| выбранное лицо | Person: объект сведений о лице | Шаблон для отображения выбранных пользователей. |
| person | Person: объект сведений о лице | Шаблон для отображения людей в раскрывающемся меню. |

В приведенных ниже примерах показано, как использовать `error` шаблон.

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует указанные ниже API и разрешения Microsoft Graph.

| API                                                                                                              | Разрешение  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/ме/пеопле](/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read        |
| [/Users](/graph/api/user-list?view=graph-rest-1.0)  | User.ReadBasic.All |
| [/граупс](/group-list?view=graph-rest-beta)  | Group.Read.All |
| [/граупс/ \$ {groupId}/мемберс](/graph/api/group-list-members?view=graph-rest-1.0) | User.ReadBasic.All        |
| [/Users/$ {УсерпринЦипленаме} ](/graph/api/user-get?view=graph-rest-1.0)  | User.Read |

## <a name="authentication"></a>Проверка подлинности

Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).

## <a name="extend-for-more-control"></a>Расширение для дополнительных элементов управления

Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected render*` способов переопределения в расширениях компонентов.

| Метод | Описание |
| - | - |
| рендеринпут | Отрисовывает текстовое поле ввода. |
| рендерселектедпеопле | Отрисовывает выбранные маркеры людей. |
| рендерселектедперсон | Отрисовывает маркер отдельного человека. |
| рендерфлйоут | Отрисовывает всплывающий хром. |
| рендерфлйоутконтент | Отображает соответствующее состояние в всплывающем окне результаты. |
| рендерлоадинг | Отображает состояние загрузки. |
| рендернодата | Отображает состояние, если результаты поискового запроса не найдены. |
| рендерсеарчресултс | Отрисовывает список результатов поиска. |
| рендерперсонресулт | Отображает результат поиска отдельного человека. |
