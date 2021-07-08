---
title: Компонент выбора каналов Microsoft Teams в Microsoft Graph Toolkit
description: Вы можете использовать компонент mgt-teams-channel-picker, чтобы в Microsoft Graph искать каналы и команды, связанные с пользователем.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: cd27db315de6b46c10c18e300ddb899ea042e428
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334733"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0352b-103">Компонент выбора каналов Microsoft Teams в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="0352b-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0352b-104">Вы также можете использовать компонент `mgt-teams-channel-picker` для разрешения поиска каналов Microsoft Teams, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0352b-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="0352b-105">Этот компонент может выполнять поиск всех команд, к которым присоединился пользователь, и каждого канала в этих командах.</span><span class="sxs-lookup"><span data-stu-id="0352b-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="0352b-106">Пример</span><span class="sxs-lookup"><span data-stu-id="0352b-106">Example</span></span>

<span data-ttu-id="0352b-107">В примере ниже показан компонент `mgt-teams-channel-picker`.</span><span class="sxs-lookup"><span data-stu-id="0352b-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="0352b-108">Начните поиск канала или команды, чтобы увидеть отображение результатов.</span><span class="sxs-lookup"><span data-stu-id="0352b-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="0352b-109">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="0352b-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="0352b-110">Получение выбранного канала</span><span class="sxs-lookup"><span data-stu-id="0352b-110">Getting the selected channel</span></span>

<span data-ttu-id="0352b-111">Используйте свойство `selectedItem`, чтобы получить канал и родительскую команду, выбранные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="0352b-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="0352b-112">Это значение будет равно null, если канал не выбран.</span><span class="sxs-lookup"><span data-stu-id="0352b-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="0352b-113">`selectedItem` содержит два свойства: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) и `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span><span class="sxs-lookup"><span data-stu-id="0352b-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="0352b-114">Выбор канала</span><span class="sxs-lookup"><span data-stu-id="0352b-114">Selecting a channel</span></span>

<span data-ttu-id="0352b-115">Используйте метод `selectChannelById(channelId: string)` для программного выбора канала.</span><span class="sxs-lookup"><span data-stu-id="0352b-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="0352b-116">**Примечание.** Средство выбора канала Teams поддерживает выбор только одного канала.</span><span class="sxs-lookup"><span data-stu-id="0352b-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="0352b-117">**Примечание.** Указанный канал (и соответствующий идентификатор) должен относиться к команде, к которой присоединился прошедший проверку пользователь.</span><span class="sxs-lookup"><span data-stu-id="0352b-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="0352b-118">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="0352b-118">CSS custom properties</span></span>

<span data-ttu-id="0352b-119">Компонент `mgt-teams-channel-picker` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="0352b-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="events"></a><span data-ttu-id="0352b-120">События</span><span class="sxs-lookup"><span data-stu-id="0352b-120">Events</span></span>

<span data-ttu-id="0352b-121">Событие</span><span class="sxs-lookup"><span data-stu-id="0352b-121">Event</span></span> | <span data-ttu-id="0352b-122">Когда он излучается</span><span class="sxs-lookup"><span data-stu-id="0352b-122">When is it emitted</span></span> | <span data-ttu-id="0352b-123">Настраиваемые данные</span><span class="sxs-lookup"><span data-stu-id="0352b-123">Custom data</span></span> | <span data-ttu-id="0352b-124">Отмена</span><span class="sxs-lookup"><span data-stu-id="0352b-124">Cancelable</span></span> | <span data-ttu-id="0352b-125">Пузыри</span><span class="sxs-lookup"><span data-stu-id="0352b-125">Bubbles</span></span> | <span data-ttu-id="0352b-126">Работает с настраиваемой шаблонной</span><span class="sxs-lookup"><span data-stu-id="0352b-126">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | <span data-ttu-id="0352b-127">Увольнение при изменении выбора канала пользователем</span><span class="sxs-lookup"><span data-stu-id="0352b-127">Fired when user makes a change in selection of a channel</span></span> | <span data-ttu-id="0352b-128">Выбранный в настоящее время элемент в `{ channel: ` [качестве группы](/graph/api/resources/channel) `, team: ` [каналов](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="0352b-128">The currently selected item as `{ channel: `[channel](/graph/api/resources/channel)`, team: `[team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="0352b-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0352b-129">No</span></span> | <span data-ttu-id="0352b-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0352b-130">No</span></span> | <span data-ttu-id="0352b-131">Да</span><span class="sxs-lookup"><span data-stu-id="0352b-131">Yes</span></span>

<span data-ttu-id="0352b-132">Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)</span><span class="sxs-lookup"><span data-stu-id="0352b-132">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="0352b-133">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="0352b-133">Templates</span></span>

<span data-ttu-id="0352b-134">Компонент `mgt-teams-channel-picker` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части.</span><span class="sxs-lookup"><span data-stu-id="0352b-134">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="0352b-135">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="0352b-135">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="0352b-136">Тип данных</span><span class="sxs-lookup"><span data-stu-id="0352b-136">Data type</span></span> | <span data-ttu-id="0352b-137">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="0352b-137">Data context</span></span> | <span data-ttu-id="0352b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0352b-138">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="0352b-139">загрузка</span><span class="sxs-lookup"><span data-stu-id="0352b-139">loading</span></span> | <span data-ttu-id="0352b-140">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="0352b-140">null: no data</span></span> | <span data-ttu-id="0352b-141">Шаблон, используемый для отображения состояния средства выбора при выполнении запроса к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0352b-141">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="0352b-142">ошибка</span><span class="sxs-lookup"><span data-stu-id="0352b-142">error</span></span> | <span data-ttu-id="0352b-143">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="0352b-143">null: no data</span></span>| <span data-ttu-id="0352b-144">Шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="0352b-144">The template used if user search returns no users.</span></span> |

<span data-ttu-id="0352b-145">В следующем примере показано, как использовать шаблон `error`.</span><span class="sxs-lookup"><span data-stu-id="0352b-145">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="0352b-146">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0352b-146">Microsoft Graph permissions</span></span>

<span data-ttu-id="0352b-147">В этом компоненте по умолчанию используются следующие API Graph Microsoft и разрешения.</span><span class="sxs-lookup"><span data-stu-id="0352b-147">This component uses the following Microsoft Graph APIs and permissions by default.</span></span>

| <span data-ttu-id="0352b-148">API</span><span class="sxs-lookup"><span data-stu-id="0352b-148">API</span></span>                                                                                                              | <span data-ttu-id="0352b-149">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0352b-149">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="0352b-150">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="0352b-150">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="0352b-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0352b-151">User.Read.All</span></span>        |
| [<span data-ttu-id="0352b-152">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="0352b-152">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="0352b-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0352b-153">Group.Read.All</span></span>        |

<span data-ttu-id="0352b-154">В версии 2.2 необходимые разрешения были обновлены до менее Teams разрешений на основе Teams.</span><span class="sxs-lookup"><span data-stu-id="0352b-154">In version 2.2, the required permissions have been updated to the less restrictive Teams-based permissions.</span></span> <span data-ttu-id="0352b-155">Чтобы избежать изменений, необходимо выбрать новые разрешения с помощью глобальной конфигурии.</span><span class="sxs-lookup"><span data-stu-id="0352b-155">To avoid a breaking change, you need to opt in to the new permissions via a global config.</span></span>

```ts
import {MgtTeamsChannelPicker} from "@microsoft/mgt-components";

MgtTeamsChannelPicker.config.useTeamsBasedScopes = true;
```

<span data-ttu-id="0352b-156">При `useTeamsBasedScopes` наборе Teams каналов будет использовать следующие `true` области.</span><span class="sxs-lookup"><span data-stu-id="0352b-156">With `useTeamsBasedScopes` set to `true`, the Teams Channel Picker will use the following scopes.</span></span> 

| <span data-ttu-id="0352b-157">API</span><span class="sxs-lookup"><span data-stu-id="0352b-157">API</span></span>                                                                                                              | <span data-ttu-id="0352b-158">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0352b-158">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="0352b-159">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="0352b-159">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="0352b-160">Team.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="0352b-160">Team.ReadBasic.All</span></span>        |
| [<span data-ttu-id="0352b-161">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="0352b-161">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="0352b-162">Channel.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="0352b-162">Channel.ReadBasic.All</span></span>        |

<span data-ttu-id="0352b-163">Это будут разрешения по умолчанию в следующем крупном обновлении.</span><span class="sxs-lookup"><span data-stu-id="0352b-163">These will be the default permissions in the next major update.</span></span>

## <a name="authentication"></a><span data-ttu-id="0352b-164">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="0352b-164">Authentication</span></span>

<span data-ttu-id="0352b-165">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="0352b-165">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="0352b-166">Кэш</span><span class="sxs-lookup"><span data-stu-id="0352b-166">Cache</span></span>

<span data-ttu-id="0352b-167">Компонент `mgt-teams-channel-picker` не кэшет данных.</span><span class="sxs-lookup"><span data-stu-id="0352b-167">The `mgt-teams-channel-picker` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="0352b-168">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="0352b-168">Extend for more control</span></span>

<span data-ttu-id="0352b-169">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="0352b-169">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="0352b-170">Метод</span><span class="sxs-lookup"><span data-stu-id="0352b-170">Method</span></span> | <span data-ttu-id="0352b-171">Описание</span><span class="sxs-lookup"><span data-stu-id="0352b-171">Description</span></span> |
| - | - |
| <span data-ttu-id="0352b-172">renderSelected</span><span class="sxs-lookup"><span data-stu-id="0352b-172">renderSelected</span></span> | <span data-ttu-id="0352b-173">Отображает выбранную команду и канал в поле ввода.</span><span class="sxs-lookup"><span data-stu-id="0352b-173">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="0352b-174">renderInput</span><span class="sxs-lookup"><span data-stu-id="0352b-174">renderInput</span></span> | <span data-ttu-id="0352b-175">Отображает поле ввода.</span><span class="sxs-lookup"><span data-stu-id="0352b-175">Renders the input box.</span></span> |
| <span data-ttu-id="0352b-176">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="0352b-176">renderDropdown</span></span> | <span data-ttu-id="0352b-177">Отображает раскрывающийся список.</span><span class="sxs-lookup"><span data-stu-id="0352b-177">Renders the dropdown.</span></span> |
| <span data-ttu-id="0352b-178">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="0352b-178">renderDropdownList</span></span> | <span data-ttu-id="0352b-179">Рекурсивно отображает элементы в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="0352b-179">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="0352b-180">renderItem</span><span class="sxs-lookup"><span data-stu-id="0352b-180">renderItem</span></span> | <span data-ttu-id="0352b-181">Отображает команду или канал в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="0352b-181">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="0352b-182">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="0352b-182">renderHighlightedText</span></span> | <span data-ttu-id="0352b-183">Отображает текст канала, выделяя входной запрос.</span><span class="sxs-lookup"><span data-stu-id="0352b-183">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="0352b-184">renderLoading</span><span class="sxs-lookup"><span data-stu-id="0352b-184">renderLoading</span></span> | <span data-ttu-id="0352b-185">Отображает состояние загрузки раскрывающегося списка.</span><span class="sxs-lookup"><span data-stu-id="0352b-185">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="0352b-186">renderError</span><span class="sxs-lookup"><span data-stu-id="0352b-186">renderError</span></span> | <span data-ttu-id="0352b-187">Отображает состояние ошибки раскрывающегося списка.</span><span class="sxs-lookup"><span data-stu-id="0352b-187">Renders the dropdown error state.</span></span> |
