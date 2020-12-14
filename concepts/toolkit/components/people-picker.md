---
title: People-Picker компонента
description: Веб-компонент mgt-people-picker можно использовать для поиска указанного количества людей и отображения списка результатов через Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: be72a31bd9e831f6584e2a7dfac9dea50892762a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659272"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>People-Picker компонента в microsoft Graph набор средств

Веб-компонент `mgt-people-picker` можно использовать для поиска людей и/или групп. По умолчанию компонент будет искать всех людей и пользователей в организации, но вы можете изменить поведение, чтобы также искать группы или только группы. Вы также можете отфильтровать поиск по определенной группе.

## <a name="example"></a>Пример

В следующем примере показан `mgt-people-picker` компонент. Начните поиск имени для отображения результатов и используйте [](#properties) редактор кода, чтобы увидеть, как свойства изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Свойства

По умолчанию компонент `mgt-people-picker` получает людей из конечных `/me/people` `/users` точек и конечных точек. Чтобы изменить это поведение, используйте следующие атрибуты.

| Атрибут | Свойство | Описание                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | Значение числа, чтобы указать максимальное количество людей для показа. Значение по умолчанию — 6.                                                                                             |
| group-id    | groupId     | Строка, которая принадлежит определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.                                                                            |
| type     | type      | Тип сущностями, которые необходимо найти. Доступные варианты: `person` , `group` , `any` . Значение по умолчанию: `person`. Этот атрибут не влияет, если `group-id` заданной является свойство.         
| transitive-search     | transitiveSearch      | Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.|
| group-type     | groupType      | Тип группы для поиска. Доступные варианты: `unified` , , , `security` `mailenabledsecurity` `distribution` `any` . Значение по умолчанию: `any`. Этот атрибут не действует, если `type` для свойства за установлено его `person` свойство.                                                                           |
|  selected-people  | selectedPeople     | Массив выбранных людей. Установите это значение, чтобы выбрать людей программным путем.|
| people   | people    | Массив людей, найденных и отрисовки в результатах поиска |
| placeholder   | placeholder    | Строка, представляющая замещая текст ввода. Значение по умолчанию: "Начать вводить имя".
| selection-mode   | selectionMode   | Строка, которая позволяет указать, поддерживает ли компонент несколько выбранных людей или только одного. Значение по `multiple` умолчанию— `single` это другой вариант.
| default-selected-user-ids | defaultSelectedUserIds | Если предоставляется строка разделенных запятой пользовательских ИД Microsoft Graph, компонент отрисовка соответствующих пользователей, выбранных после инициализации.
| selection-mode | selectionMode | Используется для того, чтобы указать, следует ли выбирать нескольких пользователей или только одного пользователя. Доступные варианты: `single` , `multiple` . Значение по умолчанию: `multiple`.
| placeholder | placeholder | Текст по умолчанию, который объясняет, как использовать компонент. Значение по умолчанию: `Start typing a name`.

Ниже приводится `show-max` пример.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>Выбранные люди

В разделе выбранных людей компонента отрисовка каждого пользователя, выбранного разработчиком или пользователем. 

![mgt-people-picker](./images/selected-people.png)

Вы можете заполнить выбранные данные пользователей, выступая одним из следующих пунктов:

- Настройка свойства `selectedPeople` напрямую, как показано в следующем примере.  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- Использование метода, который принимает массив пользовательских ид Microsoft Graph для поиска связанных сведений `selectUsersById()` о пользователе для выбора. [](/graph/api/resources/users)

     >**Примечание.** Если для пользователя не найдено ни один пользователь, данные для этого не будут `id` отрисовки. `id`

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a>События

Из компонента и происходят следующие события.

| Событие | Описание |
| --- | --- |
| `selectionChanged` | Пользователь добавил или удалил пользователя из списка выбранных или выбранных людей.|

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-people-picker` определяет следующие настраиваемые свойства CSS.

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --color: white; /* input area border focus color */
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a>Шаблоны

 `mgt-people-picker` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые можно использовать для замены определенных частей компонента. Чтобы указать шаблон, включив элемент в компонент, закажите одно из `<template>` `data-type` следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| default | null: нет данных | Шаблон, используемый для переопределения отрисовки всего компонента.
| loading | null: нет данных | Шаблон, используемый для отображения состояния picker во время запроса графа. |
| error | null: нет данных | Шаблон, используемый, если поиск пользователей не возвращает пользователей. |
| no-data | null: нет данных | Альтернативный шаблон, используемый, если поиск пользователей не возвращает пользователей. |
| selected-person | person: объект сведений о человеке | Шаблон для отображения выбранных людей. |
| person | person: объект сведений о человеке | Шаблон для отображения людей в выпадаемом меню. |

В следующих примерах показано, как использовать `error` шаблон.

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует следующие API Microsoft Graph и разрешения.

| API                                                                                                              | Разрешение  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](/graph/api/user-list-people)                    | People.Read        |
| [/users](/graph/api/user-list)  | User.ReadBasic.All |
| [/groups](/group-list)  | Group.Read.All |
| [/groups/ \$ {groupId}/members](/graph/api/group-list-members) | User.ReadBasic.All        |
| [/users/${userPrincipleName} ](/graph/api/user-get)  | User.Read |

## <a name="authentication"></a>Проверка подлинности

Этот контроль использует глобального поставщика проверки подлинности, описанного в [документации по проверке подлинности.](../providers/providers.md)

## <a name="extend-for-more-control"></a>Расширение для большего контроля

Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов.

| Метод | Описание |
| - | - |
| renderInput | Отрисовка текстового окна ввода. |
| renderSelectedPeople | Отрисовка выбранных маркеров людей. |
| renderSelectedPerson | Отрисовка маркера отдельного человека. |
| renderFlyout | Отрисовка хрома во весь экран. |
| renderFlyoutContent | Отрисовка соответствующего состояния во flyout результатов. |
| renderLoading | Отрисовка состояния загрузки. |
| renderNoData | Отрисовка состояния, когда результаты для поискового запроса не найдены. |
| renderSearchResults | Отрисовка списка результатов поиска. |
| renderPersonResult | Отрисовка результата поиска отдельного человека. |
