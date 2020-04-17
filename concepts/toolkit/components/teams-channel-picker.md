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
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ea550-103">Компонент выбора каналов Microsoft Teams в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ea550-103">Microsoft Teams Channel Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ea550-104">Вы можете использовать `mgt-teams-channel-picker` компонент, чтобы включить поиск каналов Microsoft Teams, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="ea550-104">A you can use the `mgt-teams-channel-picker` component to enable searches for Microsoft Teams channels associated with a user.</span></span> <span data-ttu-id="ea550-105">Компонент может выполнять поиск во всех командах, присоединенных к пользователю, и каждому каналу в этих командах.</span><span class="sxs-lookup"><span data-stu-id="ea550-105">The component can search all teams the user has joined, and each channel in those teams.</span></span> 

## <a name="example"></a><span data-ttu-id="ea550-106">Пример</span><span class="sxs-lookup"><span data-stu-id="ea550-106">Example</span></span>

<span data-ttu-id="ea550-107">В приведенном ниже примере `mgt-teams-channel-picker` показан компонент.</span><span class="sxs-lookup"><span data-stu-id="ea550-107">The following example shows the `mgt-teams-channel-picker` component.</span></span> <span data-ttu-id="ea550-108">Чтобы просмотреть результаты, запустите поиск канала или группы.</span><span class="sxs-lookup"><span data-stu-id="ea550-108">Start searching for a channel or team to see the results render.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="ea550-109">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="ea550-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a><span data-ttu-id="ea550-110">Извлечение выбранного канала</span><span class="sxs-lookup"><span data-stu-id="ea550-110">Getting the selected channel</span></span>

<span data-ttu-id="ea550-111">Используйте `selectedItem` свойство, чтобы получить текущий выбранный канал и родительскую группу.</span><span class="sxs-lookup"><span data-stu-id="ea550-111">Use the `selectedItem` property to retrieve the currently selected channel and parent team.</span></span> <span data-ttu-id="ea550-112">Это значение будет равно null, если канал не выбран.</span><span class="sxs-lookup"><span data-stu-id="ea550-112">This value will be null if no channel has been selected.</span></span> <span data-ttu-id="ea550-113">`selectedItem`содержит два свойства: `channel` ([MicrosoftGraph. Channel](/graph/api/resources/channel?view=graph-rest-1.0)) и `team` ([MicrosoftGraph. Team](/graph/api/resources/team?view=graph-rest-1.0)).</span><span class="sxs-lookup"><span data-stu-id="ea550-113">`selectedItem` contains two properties: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel?view=graph-rest-1.0)) and `team` ([MicrosoftGraph.Team](/graph/api/resources/team?view=graph-rest-1.0)).</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a><span data-ttu-id="ea550-114">Выбор канала</span><span class="sxs-lookup"><span data-stu-id="ea550-114">Selecting a channel</span></span>

<span data-ttu-id="ea550-115">Используйте `selectChannelById(channelId: string)` метод для программного выбора канала.</span><span class="sxs-lookup"><span data-stu-id="ea550-115">Use the `selectChannelById(channelId: string)` method to programmatically select a channel.</span></span>

> <span data-ttu-id="ea550-116">**Note:** выбор канала Teams поддерживает только один канал.</span><span class="sxs-lookup"><span data-stu-id="ea550-116">**Note:** the Teams channel picker only supports single channel selection.</span></span>

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> <span data-ttu-id="ea550-117">**Примечание:** Указанный канал (и следующий идентификатор) должен принадлежать к группе, к которой был присоединен пользователь, прошедшему проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="ea550-117">**Note:** The provided channel (and subsequent ID) must belong to a team that the authenticated user has joined.</span></span> 


## <a name="css-custom-properties"></a><span data-ttu-id="ea550-118">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="ea550-118">CSS custom properties</span></span>

<span data-ttu-id="ea550-119">`mgt-teams-channel-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="ea550-119">The `mgt-teams-channel-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="events"></a><span data-ttu-id="ea550-120">События</span><span class="sxs-lookup"><span data-stu-id="ea550-120">Events</span></span>
| <span data-ttu-id="ea550-121">Событие</span><span class="sxs-lookup"><span data-stu-id="ea550-121">Event</span></span> | <span data-ttu-id="ea550-122">Сведения</span><span class="sxs-lookup"><span data-stu-id="ea550-122">Detail</span></span> | <span data-ttu-id="ea550-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ea550-123">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ea550-124">selectionChanged</span><span class="sxs-lookup"><span data-stu-id="ea550-124">selectionChanged</span></span> | <span data-ttu-id="ea550-125">Сведения содержит выделенный в данный момент элемент `{channel : ` [MicrosoftGraph. Channel](/graph/api/resources/channel?view=graph-rest-1.0)`, team: `[MicrosoftGraph. Team](/graph/api/resources/team?view=graph-rest-1.0)`}`</span><span class="sxs-lookup"><span data-stu-id="ea550-125">The detail contains the currently selected item  of `{channel : `[MicrosoftGraph.Channel](/graph/api/resources/channel?view=graph-rest-1.0)`, team: `[MicrosoftGraph.Team](/graph/api/resources/team?view=graph-rest-1.0)`}`</span></span> | <span data-ttu-id="ea550-126">Возникает, когда пользователь вносит изменения в выбор канала.</span><span class="sxs-lookup"><span data-stu-id="ea550-126">Fired when user makes a change in selection of a channel.</span></span> |

## <a name="templates"></a><span data-ttu-id="ea550-127">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="ea550-127">Templates</span></span>

 <span data-ttu-id="ea550-128">`mgt-teams-channel-picker`поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="ea550-128">`mgt-teams-channel-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="ea550-129">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="ea550-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="ea550-130">Тип данных</span><span class="sxs-lookup"><span data-stu-id="ea550-130">Data type</span></span> | <span data-ttu-id="ea550-131">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="ea550-131">Data context</span></span> | <span data-ttu-id="ea550-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea550-132">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ea550-133">загрузки</span><span class="sxs-lookup"><span data-stu-id="ea550-133">loading</span></span> | <span data-ttu-id="ea550-134">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="ea550-134">null: no data</span></span> | <span data-ttu-id="ea550-135">Шаблон, используемый для отображения состояния элемента управления "выбор" во время выполнения запроса к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ea550-135">The template used to render the state of the picker while the request to Microsoft Graph is being made.</span></span> |
| <span data-ttu-id="ea550-136">error</span><span class="sxs-lookup"><span data-stu-id="ea550-136">error</span></span> | <span data-ttu-id="ea550-137">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="ea550-137">null: no data</span></span>| <span data-ttu-id="ea550-138">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="ea550-138">The template used if user search returns no users.</span></span> |


<span data-ttu-id="ea550-139">В приведенном ниже примере показано, как `error` использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="ea550-139">The following example shows how to use the `error` template.</span></span>

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ea550-140">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ea550-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="ea550-141">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ea550-141">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="ea550-142">API</span><span class="sxs-lookup"><span data-stu-id="ea550-142">API</span></span>                                                                                                              | <span data-ttu-id="ea550-143">Разрешение</span><span class="sxs-lookup"><span data-stu-id="ea550-143">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="ea550-144">/ме/жоинедтеамс</span><span class="sxs-lookup"><span data-stu-id="ea550-144">/me/joinedTeams</span></span>](/graph/api/user-list-joinedteams?view=graph-rest-1.0)                    | <span data-ttu-id="ea550-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea550-145">User.Read.All</span></span>        |
| [<span data-ttu-id="ea550-146">/Teams/$ {ID}/чаннелс</span><span class="sxs-lookup"><span data-stu-id="ea550-146">/teams/${id}/channels</span></span>](/graph/api/channel-list?view=graph-rest-1.0) | <span data-ttu-id="ea550-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea550-147">Group.Read.All</span></span>        |

## <a name="authentication"></a><span data-ttu-id="ea550-148">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="ea550-148">Authentication</span></span>

<span data-ttu-id="ea550-149">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="ea550-149">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="ea550-150">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="ea550-150">Extend for more control</span></span>

<span data-ttu-id="ea550-151">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов:</span><span class="sxs-lookup"><span data-stu-id="ea550-151">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions:</span></span>

| <span data-ttu-id="ea550-152">Метод</span><span class="sxs-lookup"><span data-stu-id="ea550-152">Method</span></span> | <span data-ttu-id="ea550-153">Описание</span><span class="sxs-lookup"><span data-stu-id="ea550-153">Description</span></span> |
| - | - |
| <span data-ttu-id="ea550-154">рендерселектед</span><span class="sxs-lookup"><span data-stu-id="ea550-154">renderSelected</span></span> | <span data-ttu-id="ea550-155">Отрисовывает выбранную группу и канал в поле ввода.</span><span class="sxs-lookup"><span data-stu-id="ea550-155">Renders the selected team and channel in the input box.</span></span> |
| <span data-ttu-id="ea550-156">рендеринпут</span><span class="sxs-lookup"><span data-stu-id="ea550-156">renderInput</span></span> | <span data-ttu-id="ea550-157">Отрисовывает поле ввода.</span><span class="sxs-lookup"><span data-stu-id="ea550-157">Renders the input box.</span></span> |
| <span data-ttu-id="ea550-158">рендердропдовн</span><span class="sxs-lookup"><span data-stu-id="ea550-158">renderDropdown</span></span> | <span data-ttu-id="ea550-159">Отрисовывает раскрывающийся список.</span><span class="sxs-lookup"><span data-stu-id="ea550-159">Renders the dropdown.</span></span> |
| <span data-ttu-id="ea550-160">рендердропдовнлист</span><span class="sxs-lookup"><span data-stu-id="ea550-160">renderDropdownList</span></span> | <span data-ttu-id="ea550-161">Рекурсивно отображает элементы в раскрывающемся меню.</span><span class="sxs-lookup"><span data-stu-id="ea550-161">Renders the items in the dropdown recursively.</span></span> |
| <span data-ttu-id="ea550-162">рендеритем</span><span class="sxs-lookup"><span data-stu-id="ea550-162">renderItem</span></span> | <span data-ttu-id="ea550-163">Отрисовывает группу или канал в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="ea550-163">Renders a team or a channel in the dropdown list.</span></span> |
| <span data-ttu-id="ea550-164">рендерхигхлигхтедтекст</span><span class="sxs-lookup"><span data-stu-id="ea550-164">renderHighlightedText</span></span> | <span data-ttu-id="ea550-165">Отрисовывает текст канала, выделяя входной запрос.</span><span class="sxs-lookup"><span data-stu-id="ea550-165">Renders the channel text, highlighting the input query.</span></span> |
| <span data-ttu-id="ea550-166">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="ea550-166">renderLoading</span></span> | <span data-ttu-id="ea550-167">Отображает состояние раскрывающегося меню загрузки.</span><span class="sxs-lookup"><span data-stu-id="ea550-167">Renders the loading dropdown state.</span></span> |
| <span data-ttu-id="ea550-168">renderError</span><span class="sxs-lookup"><span data-stu-id="ea550-168">renderError</span></span> | <span data-ttu-id="ea550-169">Отображает состояние ошибки раскрывающегося меню.</span><span class="sxs-lookup"><span data-stu-id="ea550-169">Renders the dropdown error state.</span></span> |
