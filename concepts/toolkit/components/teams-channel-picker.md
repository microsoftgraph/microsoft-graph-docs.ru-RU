---
title: Компонент выбора каналов Microsoft Teams в наборе инструментов Microsoft Graph
description: Для поиска каналов и команд, связанных с пользователем, из Microsoft Graph можно использовать средство управления "упр. Teams".
localization_priority: Normal
author: vogtn
ms.openlocfilehash: c8ade0fdfd41bde4d4a2ec643950b3faa8d24d98
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144398"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Компонент выбора каналов Microsoft Teams в наборе инструментов Microsoft Graph

Вы можете использовать `mgt-teams-channel-picker` компонент, чтобы включить поиск каналов Microsoft Teams, связанных с пользователем. Компонент может выполнять поиск во всех командах, присоединенных к пользователю, и каждому каналу в этих командах. 

## <a name="example"></a>Пример

В приведенном ниже примере `mgt-teams-channel-picker` показан компонент. Чтобы просмотреть результаты, запустите поиск канала или группы.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[Откройте этот пример в меню упр. dev.](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>Извлечение выбранного канала

Используйте `selectedItem` свойство, чтобы получить текущий выбранный канал и родительскую группу. Это значение будет равно null, если канал не выбран. `selectedItem`содержит два свойства: `channel` ([MicrosoftGraph. Channel](/graph/api/resources/channel?view=graph-rest-1.0)) и `team` ([MicrosoftGraph. Team](/graph/api/resources/team?view=graph-rest-1.0)).

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a>Выбор канала

Используйте `selectChannelById(channelId: string)` метод для программного выбора канала.

> **Note:** выбор канала Teams поддерживает только один канал.

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> **Примечание:** Указанный канал (и следующий идентификатор) должен принадлежать к группе, к которой был присоединен пользователь, прошедшему проверку подлинности. 


## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

`mgt-teams-channel-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.

```css
mgt-teams-channel-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* channel background color */
    --dropdown-item-hover-background: #333d47; /* channel or team hover background */
    --dropdown-item-selected-background: #0F78D4; /* selected channel background color */

    --font-color: white; /* input area border focus color */
    --arrow-fill: #ffffff;
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* place holder text focus color */
}
```

## <a name="events"></a>Мероприятия
| Событие | Detail (Сведения) | Описание |
| --- | --- | --- |
| selectionChanged | Сведения содержит выделенный в данный момент элемент `{channel : ` [MicrosoftGraph. Channel](/graph/api/resources/channel?view=graph-rest-1.0)`, team: `[MicrosoftGraph. Team](/graph/api/resources/team?view=graph-rest-1.0)`}` | Возникает, когда пользователь вносит изменения в выбор канала. |

## <a name="templates"></a>Шаблоны

 `mgt-teams-channel-picker`поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента. Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| загрузки | NULL: нет данных | Шаблон, используемый для отображения состояния элемента управления "выбор" во время выполнения запроса к Microsoft Graph. |
| error | NULL: нет данных| Шаблон, используемый, если поиск пользователей не возвращает пользователей. |


В приведенном ниже примере показано, как `error` использовать шаблон.

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует указанные ниже API и разрешения Microsoft Graph.

| API                                                                                                              | Разрешение  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/ме/жоинедтеамс](/graph/api/user-list-joinedteams?view=graph-rest-1.0)                    | User.Read.All        |
| [/Teams/$ {ID}/чаннелс](/graph/api/channel-list?view=graph-rest-1.0) | Group.Read.All        |

## <a name="authentication"></a>Проверка подлинности

Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).

## <a name="extend-for-more-control"></a>Расширение для дополнительных элементов управления

Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов:

| Метод | Описание |
| - | - |
| рендерселектед | Отрисовывает выбранную группу и канал в поле ввода. |
| рендеринпут | Отрисовывает поле ввода. |
| рендердропдовн | Отрисовывает раскрывающийся список. |
| рендердропдовнлист | Рекурсивно отображает элементы в раскрывающемся меню. |
| рендеритем | Отрисовывает группу или канал в раскрывающемся списке. |
| рендерхигхлигхтедтекст | Отрисовывает текст канала, выделяя входной запрос. |
| рендерлоадинг | Отображает состояние раскрывающегося меню загрузки. |
| renderError | Отображает состояние ошибки раскрывающегося меню. |
