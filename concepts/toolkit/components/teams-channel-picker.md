---
title: Компонент выбора каналов Microsoft Teams в Microsoft Graph Toolkit
description: Вы можете использовать компонент mgt-teams-channel-picker, чтобы в Microsoft Graph искать каналы и команды, связанные с пользователем.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: ad196cc17b70f42cd571bf5805e2aa4eb2cfe90e
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082029"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Компонент выбора каналов Microsoft Teams в Microsoft Graph Toolkit

Вы также можете использовать компонент `mgt-teams-channel-picker` для разрешения поиска каналов Microsoft Teams, связанных с пользователем. Этот компонент может выполнять поиск всех команд, к которым присоединился пользователь, и каждого канала в этих командах. 

## <a name="example"></a>Пример

В примере ниже показан компонент `mgt-teams-channel-picker`. Начните поиск канала или команды, чтобы увидеть отображение результатов.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>Получение выбранного канала

Используйте свойство `selectedItem`, чтобы получить канал и родительскую команду, выбранные в настоящее время. Это значение будет равно null, если канал не выбран. `selectedItem` содержит два свойства: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) и `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a>Выбор канала

Используйте метод `selectChannelById(channelId: string)` для программного выбора канала.

> **Примечание.** Средство выбора канала Teams поддерживает выбор только одного канала.

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> **Примечание.** Указанный канал (и соответствующий идентификатор) должен относиться к команде, к которой присоединился прошедший проверку пользователь. 


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
| `selectionChanged` | Сведения содержат выбранный в настоящее время элемент `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team)`}` | Возникает, когда пользователь изменяет выбор канала. |

Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)

## <a name="templates"></a>Шаблоны

 Компонент `mgt-teams-channel-picker` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| загрузка | null: нет данных | Шаблон, используемый для отображения состояния средства выбора при выполнении запроса к Microsoft Graph. |
| ошибка | null: нет данных| Шаблон, используемый в том случае, если поиск не возвращает пользователей. |


В следующем примере показано, как использовать шаблон `error`.

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

В этом компоненте по умолчанию используются следующие API Graph Microsoft и разрешения.

| API                                                                                                              | Разрешение  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams)                    | User.Read.All        |
| [/teams/${id}/channels](/graph/api/channel-list) | Group.Read.All        |

В версии 2.2 необходимые разрешения были обновлены до менее Teams разрешений на основе Teams. Чтобы избежать изменений, необходимо выбрать новые разрешения с помощью глобальной конфигурии.

```ts
import {MgtTeamsChannelPicker} from "@microsoft/mgt-components";

MgtTeamsChannelPicker.config.useTeamsBasedScopes = true;
```

При `useTeamsBasedScopes` наборе Teams каналов будет использовать следующие `true` области. 

| API                                                                                                              | Разрешение  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams)                    | Team.ReadBasic.All        |
| [/teams/${id}/channels](/graph/api/channel-list) | Channel.ReadBasic.All        |

Это будут разрешения по умолчанию в следующем крупном обновлении.

## <a name="authentication"></a>Проверка подлинности

В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="cache"></a>Кэш

Компонент `mgt-teams-channel-picker` не кэшет данных.

## <a name="extend-for-more-control"></a>Расширение для дополнительного управления

В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.

| Метод | Описание |
| - | - |
| renderSelected | Отображает выбранную команду и канал в поле ввода. |
| renderInput | Отображает поле ввода. |
| renderDropdown | Отображает раскрывающийся список. |
| renderDropdownList | Рекурсивно отображает элементы в раскрывающемся списке. |
| renderItem | Отображает команду или канал в раскрывающемся списке. |
| renderHighlightedText | Отображает текст канала, выделяя входной запрос. |
| renderLoading | Отображает состояние загрузки раскрывающегося списка. |
| renderError | Отображает состояние ошибки раскрывающегося списка. |
