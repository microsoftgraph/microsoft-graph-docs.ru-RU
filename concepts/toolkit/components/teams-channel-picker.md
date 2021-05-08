---
title: Компонент выбора каналов Microsoft Teams в Microsoft Graph Toolkit
description: Вы можете использовать компонент mgt-teams-channel-picker, чтобы в Microsoft Graph искать каналы и команды, связанные с пользователем.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 086ce7085f1802e40195fca9f54f2af460291fda
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266796"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="344cf-103">Компонент выбора каналов Microsoft Teams в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="344cf-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="344cf-104">Вы также можете использовать компонент `mgt-teams-channel-picker` для разрешения поиска каналов Microsoft Teams, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="344cf-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="344cf-105">Этот компонент может выполнять поиск всех команд, к которым присоединился пользователь, и каждого канала в этих командах.</span><span class="sxs-lookup"><span data-stu-id="344cf-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="344cf-106">Пример</span><span class="sxs-lookup"><span data-stu-id="344cf-106">Example</span></span>

<span data-ttu-id="344cf-107">В примере ниже показан компонент `mgt-teams-channel-picker`.</span><span class="sxs-lookup"><span data-stu-id="344cf-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="344cf-108">Начните поиск канала или команды, чтобы увидеть отображение результатов.</span><span class="sxs-lookup"><span data-stu-id="344cf-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="344cf-109">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="344cf-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="344cf-110">Получение выбранного канала</span><span class="sxs-lookup"><span data-stu-id="344cf-110">Getting the selected channel</span></span>

<span data-ttu-id="344cf-111">Используйте свойство `selectedItem`, чтобы получить канал и родительскую команду, выбранные в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="344cf-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="344cf-112">Это значение будет равно null, если канал не выбран.</span><span class="sxs-lookup"><span data-stu-id="344cf-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="344cf-113">`selectedItem` содержит два свойства: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) и `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span><span class="sxs-lookup"><span data-stu-id="344cf-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="344cf-114">Выбор канала</span><span class="sxs-lookup"><span data-stu-id="344cf-114">Selecting a channel</span></span>

<span data-ttu-id="344cf-115">Используйте метод `selectChannelById(channelId: string)` для программного выбора канала.</span><span class="sxs-lookup"><span data-stu-id="344cf-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="344cf-116">**Примечание.** Средство выбора канала Teams поддерживает выбор только одного канала.</span><span class="sxs-lookup"><span data-stu-id="344cf-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="344cf-117">**Примечание.** Указанный канал (и соответствующий идентификатор) должен относиться к команде, к которой присоединился прошедший проверку пользователь.</span><span class="sxs-lookup"><span data-stu-id="344cf-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="344cf-118">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="344cf-118">CSS custom properties</span></span>

<span data-ttu-id="344cf-119">Компонент `mgt-teams-channel-picker` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="344cf-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="events"></a><span data-ttu-id="344cf-120">События</span><span class="sxs-lookup"><span data-stu-id="344cf-120">Events</span></span>
| <span data-ttu-id="344cf-121">Событие</span><span class="sxs-lookup"><span data-stu-id="344cf-121">Event</span></span> | <span data-ttu-id="344cf-122">Сведения</span><span class="sxs-lookup"><span data-stu-id="344cf-122">Detail</span></span> | <span data-ttu-id="344cf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="344cf-123">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="344cf-124">selectionChanged</span><span class="sxs-lookup"><span data-stu-id="344cf-124">selectionChanged</span></span> | <span data-ttu-id="344cf-125">Сведения содержат выбранный в настоящее время элемент `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team)`}`</span><span class="sxs-lookup"><span data-stu-id="344cf-125">The detail contains the currently selected item  of `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team)`}`</span></span> | <span data-ttu-id="344cf-126">Возникает, когда пользователь изменяет выбор канала.</span><span class="sxs-lookup"><span data-stu-id="344cf-126">Fired when user makes a change in selection of a channel.</span></span> |

## <a name="templates"></a><span data-ttu-id="344cf-127">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="344cf-127">Templates</span></span>

 <span data-ttu-id="344cf-128">Компонент `mgt-teams-channel-picker` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части.</span><span class="sxs-lookup"><span data-stu-id="344cf-128">`mgt-teams-channel-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="344cf-129">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="344cf-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="344cf-130">Тип данных</span><span class="sxs-lookup"><span data-stu-id="344cf-130">Data type</span></span> | <span data-ttu-id="344cf-131">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="344cf-131">Data context</span></span> | <span data-ttu-id="344cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="344cf-132">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="344cf-133">загрузка</span><span class="sxs-lookup"><span data-stu-id="344cf-133">loading</span></span> | <span data-ttu-id="344cf-134">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="344cf-134">null: no data</span></span> | <span data-ttu-id="344cf-135">Шаблон, используемый для отображения состояния средства выбора при выполнении запроса к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="344cf-135">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="344cf-136">ошибка</span><span class="sxs-lookup"><span data-stu-id="344cf-136">error</span></span> | <span data-ttu-id="344cf-137">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="344cf-137">null: no data</span></span>| <span data-ttu-id="344cf-138">Шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="344cf-138">The template used if user search returns no users.</span></span> |


<span data-ttu-id="344cf-139">В следующем примере показано, как использовать шаблон `error`.</span><span class="sxs-lookup"><span data-stu-id="344cf-139">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="344cf-140">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="344cf-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="344cf-141">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="344cf-141">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="344cf-142">API</span><span class="sxs-lookup"><span data-stu-id="344cf-142">API</span></span>                                                                                                              | <span data-ttu-id="344cf-143">Разрешение</span><span class="sxs-lookup"><span data-stu-id="344cf-143">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="344cf-144">/me/joinedTeams</span><span class="sxs-lookup"><span data-stu-id="344cf-144">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams)                    | <span data-ttu-id="344cf-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="344cf-145">User.Read.All</span></span>        |
| [<span data-ttu-id="344cf-146">/teams/${id}/channels</span><span class="sxs-lookup"><span data-stu-id="344cf-146">/teams/${id}/channels</span></span>](/graph/api/channel-list) | <span data-ttu-id="344cf-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="344cf-147">Group.Read.All</span></span>        |

## <a name="authentication"></a><span data-ttu-id="344cf-148">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="344cf-148">Authentication</span></span>

<span data-ttu-id="344cf-149">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="344cf-149">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="344cf-150">Кэш</span><span class="sxs-lookup"><span data-stu-id="344cf-150">Cache</span></span>

<span data-ttu-id="344cf-151">Компонент `mgt-teams-channel-picker` не кэшет данных.</span><span class="sxs-lookup"><span data-stu-id="344cf-151">The `mgt-teams-channel-picker` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="344cf-152">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="344cf-152">Extend for more control</span></span>

<span data-ttu-id="344cf-153">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="344cf-153">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="344cf-154">Метод</span><span class="sxs-lookup"><span data-stu-id="344cf-154">Method</span></span> | <span data-ttu-id="344cf-155">Описание</span><span class="sxs-lookup"><span data-stu-id="344cf-155">Description</span></span> |
| - | - |
| <span data-ttu-id="344cf-156">renderSelected</span><span class="sxs-lookup"><span data-stu-id="344cf-156">renderSelected</span></span> | <span data-ttu-id="344cf-157">Отображает выбранную команду и канал в поле ввода.</span><span class="sxs-lookup"><span data-stu-id="344cf-157">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="344cf-158">renderInput</span><span class="sxs-lookup"><span data-stu-id="344cf-158">renderInput</span></span> | <span data-ttu-id="344cf-159">Отображает поле ввода.</span><span class="sxs-lookup"><span data-stu-id="344cf-159">Renders the input box.</span></span> |
| <span data-ttu-id="344cf-160">renderDropdown</span><span class="sxs-lookup"><span data-stu-id="344cf-160">renderDropdown</span></span> | <span data-ttu-id="344cf-161">Отображает раскрывающийся список.</span><span class="sxs-lookup"><span data-stu-id="344cf-161">Renders the dropdown.</span></span> |
| <span data-ttu-id="344cf-162">renderDropdownList</span><span class="sxs-lookup"><span data-stu-id="344cf-162">renderDropdownList</span></span> | <span data-ttu-id="344cf-163">Рекурсивно отображает элементы в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="344cf-163">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="344cf-164">renderItem</span><span class="sxs-lookup"><span data-stu-id="344cf-164">renderItem</span></span> | <span data-ttu-id="344cf-165">Отображает команду или канал в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="344cf-165">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="344cf-166">renderHighlightedText</span><span class="sxs-lookup"><span data-stu-id="344cf-166">renderHighlightedText</span></span> | <span data-ttu-id="344cf-167">Отображает текст канала, выделяя входной запрос.</span><span class="sxs-lookup"><span data-stu-id="344cf-167">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="344cf-168">renderLoading</span><span class="sxs-lookup"><span data-stu-id="344cf-168">renderLoading</span></span> | <span data-ttu-id="344cf-169">Отображает состояние загрузки раскрывающегося списка.</span><span class="sxs-lookup"><span data-stu-id="344cf-169">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="344cf-170">renderError</span><span class="sxs-lookup"><span data-stu-id="344cf-170">renderError</span></span> | <span data-ttu-id="344cf-171">Отображает состояние ошибки раскрывающегося списка.</span><span class="sxs-lookup"><span data-stu-id="344cf-171">Renders the dropdown error state.</span></span> |
