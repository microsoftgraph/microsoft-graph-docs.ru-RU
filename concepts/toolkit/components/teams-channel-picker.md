---
title: Компонент "Выбор каналов Microsoft Teams" в microsoft Graph набор средств
description: Вы можете использовать mgt-teams-channel-picker для поиска каналов и команд, связанных с пользователем из Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: c0b6e818f0c9c30314b5342fcfb6ef44978ec830
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660010"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Компонент "Выбор каналов Microsoft Teams" в microsoft Graph набор средств

Компонент можно использовать для поиска каналов `mgt-teams-channel-picker` Microsoft Teams, связанных с пользователем. Компонент может искать все команды, к которых присоединился пользователь, и каждый канал в этих командах. 

## <a name="example"></a>Пример

В следующем примере показан `mgt-teams-channel-picker` компонент. Начните поиск канала или команды для отображения результатов.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>Получение выбранного канала

Используйте это свойство для получения выбранного в данный момент `selectedItem` канала и родительской команды. Это значение будет иметь значение NULL, если канал не выбран. `selectedItem` содержит два свойства: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) и `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a>Выбор канала

Используйте этот `selectChannelById(channelId: string)` метод для выбора канала программным способом.

> **Примечание.** Выбор каналов Teams поддерживает только выбор одного канала.

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> **Примечание.** Предоставленный канал (и последующий ИД) должен принадлежать команде, к ней присоединился пользователь, подлинность пользователя. 


## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-teams-channel-picker` определяет следующие настраиваемые свойства CSS.

```css
mgt-teams-channel-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* channel background color */
    --dropdown-item-hover-background: #333d47; /* channel or team hover background */
    --dropdown-item-selected-background: #0F78D4; /* selected channel background color */

    --color: white; /* input area border focus color */
    --arrow-fill: #ffffff;
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* place holder text focus color */
}
```

## <a name="events"></a>События
| Событие | Сведения | Описание |
| --- | --- | --- |
| selectionChanged | Сведения содержат текущий выбранный элемент `{channel : ` [MicrosoftGraph.Channel](/graph/api/resources/channel) `, team: ` [MicrosoftGraph.Team](/graph/api/resources/team)`}` | Создается, когда пользователь вносит изменения в выбор канала. |

## <a name="templates"></a>Шаблоны

 `mgt-teams-channel-picker` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые можно использовать для замены определенных частей компонента. Чтобы указать шаблон, включив элемент в `<template>` компонент, закажите одно из `data-type` следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| loading | null: нет данных | Шаблон, используемый для отображения состояния picker во время запроса к Microsoft Graph. |
| error | null: нет данных| Шаблон, используемый, если поиск пользователей не возвращает пользователей. |


В следующем примере показано, как использовать `error` шаблон.

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует следующие API Microsoft Graph и разрешения.

| API                                                                                                              | Разрешение  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams)                    | User.Read.All        |
| [/teams/${id}/channels](/graph/api/channel-list) | Group.Read.All        |

## <a name="authentication"></a>Проверка подлинности

Этот контроль использует глобального поставщика проверки подлинности, описанного в [документации по проверке подлинности.](../providers/providers.md)

## <a name="extend-for-more-control"></a>Расширение для большего контроля

Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов:

| Метод | Описание |
| - | - |
| renderSelected | Отрисовка выбранной команды и канала в поле ввода. |
| renderInput | Отрисовка ввода. |
| renderDropdown | Отрисовка выпадаемой области. |
| renderDropdownList | Рекурсивно отрисовка элементов в выпадаемом меню. |
| renderItem | Отрисовка команды или канала в выпадаемом списке. |
| renderHighlightedText | Отрисовка текста канала с выделением входного запроса. |
| renderLoading | Отрисовка состояния выпадания загрузки. |
| renderError | Отрисовка состояния ошибки в dropdown. |
