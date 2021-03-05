---
title: Компонент "Выбор людей"
description: Веб-компонент mgt-people-picker можно использовать для поиска указанного количества людей и отображать список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c9541130abe8f520b41a0bd4d52de9a167e18c24
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475186"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1c5e8-103">Компонент "Выбор людей" в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1c5e8-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1c5e8-104">Веб-компонент `mgt-people-picker` можно использовать для поиска людей и (или) групп.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="1c5e8-105">По умолчанию компонент ищет всех людей и пользователей в организации, но вы можете изменить его поведение, чтобы также искать группы или только группы.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="1c5e8-106">Вы также можете отфильтровать поиск по определенной группе.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="1c5e8-107">Пример</span><span class="sxs-lookup"><span data-stu-id="1c5e8-107">Example</span></span>

<span data-ttu-id="1c5e8-108">В примере ниже показан компонент `mgt-people-picker`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="1c5e8-109">Начните поиск имени, чтобы отобразить результаты, и используйте редактор кода, чтобы увидеть, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="1c5e8-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="1c5e8-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="1c5e8-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c5e8-111">Properties</span></span>

<span data-ttu-id="1c5e8-112">По умолчанию компонент `mgt-people-picker` извлекает людей из конечных точек `/me/people` и `/users`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="1c5e8-113">Используйте следующие атрибуты, чтобы изменить его поведение.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="1c5e8-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="1c5e8-114">Attribute</span></span> | <span data-ttu-id="1c5e8-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c5e8-115">Property</span></span> | <span data-ttu-id="1c5e8-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1c5e8-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1c5e8-117">show-max</span><span class="sxs-lookup"><span data-stu-id="1c5e8-117">show-max</span></span> | <span data-ttu-id="1c5e8-118">showMax</span><span class="sxs-lookup"><span data-stu-id="1c5e8-118">showMax</span></span>   | <span data-ttu-id="1c5e8-119">Числовое значение, указывающее максимальное количество отображаемых людей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="1c5e8-120">Значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="1c5e8-121">group-id</span><span class="sxs-lookup"><span data-stu-id="1c5e8-121">group-id</span></span>    | <span data-ttu-id="1c5e8-122">groupId</span><span class="sxs-lookup"><span data-stu-id="1c5e8-122">groupId</span></span>     | <span data-ttu-id="1c5e8-123">Значение строки, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="1c5e8-124">type</span><span class="sxs-lookup"><span data-stu-id="1c5e8-124">type</span></span>     | <span data-ttu-id="1c5e8-125">type</span><span class="sxs-lookup"><span data-stu-id="1c5e8-125">type</span></span>      | <span data-ttu-id="1c5e8-126">Тип объектов, которые необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-126">The type of entities to search for.</span></span> <span data-ttu-id="1c5e8-127">Доступные варианты — `person`, `group`, `any`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="1c5e8-128">Значение по умолчанию — `person`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-128">Default value is `person`.</span></span> <span data-ttu-id="1c5e8-129">Этот атрибут не оказывает влияния, если задано свойство `group-id`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="1c5e8-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="1c5e8-130">transitive-search</span></span>     | <span data-ttu-id="1c5e8-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="1c5e8-131">transitiveSearch</span></span>      | <span data-ttu-id="1c5e8-132">Логическое значение для выполнения транзитивного поиска, возвращающего плоский список всех вложенных элементов. По умолчанию транзитивный поиск не используется.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="1c5e8-133">group-type</span><span class="sxs-lookup"><span data-stu-id="1c5e8-133">group-type</span></span>     | <span data-ttu-id="1c5e8-134">groupType</span><span class="sxs-lookup"><span data-stu-id="1c5e8-134">groupType</span></span>      | <span data-ttu-id="1c5e8-135">Тип группы, которую необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-135">The group type to search for.</span></span> <span data-ttu-id="1c5e8-136">Доступные варианты — `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="1c5e8-137">Значение по умолчанию — `any`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-137">Default value is `any`.</span></span> <span data-ttu-id="1c5e8-138">Этот атрибут не оказывает влияния, если для свойства `type` задано значение `person`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="1c5e8-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="1c5e8-139">selected-people</span></span>  | <span data-ttu-id="1c5e8-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="1c5e8-140">selectedPeople</span></span>     | <span data-ttu-id="1c5e8-141">Массив выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-141">An array of selected people.</span></span> <span data-ttu-id="1c5e8-142">Установите это значение, чтобы выбрать людей программным образом.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="1c5e8-143">people</span><span class="sxs-lookup"><span data-stu-id="1c5e8-143">people</span></span>   | <span data-ttu-id="1c5e8-144">people</span><span class="sxs-lookup"><span data-stu-id="1c5e8-144">people</span></span>    | <span data-ttu-id="1c5e8-145">Массив людей, найденных и отображенных в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="1c5e8-146">placeholder</span><span class="sxs-lookup"><span data-stu-id="1c5e8-146">placeholder</span></span>   | <span data-ttu-id="1c5e8-147">placeholder</span><span class="sxs-lookup"><span data-stu-id="1c5e8-147">placeholder</span></span>    | <span data-ttu-id="1c5e8-148">Текст по умолчанию, который объясняет, как использовать компонент.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="1c5e8-149">Значение по умолчанию — `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="1c5e8-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="1c5e8-150">default-selected-user-ids</span></span> | <span data-ttu-id="1c5e8-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="1c5e8-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="1c5e8-152">При предоставлении строки разделенных запятой ИД пользователей Microsoft Graph, компонент отображает соответствующих пользователей как выбранных после инициализации.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="1c5e8-153">selection-mode</span><span class="sxs-lookup"><span data-stu-id="1c5e8-153">selection-mode</span></span> | <span data-ttu-id="1c5e8-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="1c5e8-154">selectionMode</span></span> | <span data-ttu-id="1c5e8-155">Используется, чтобы указать следует ли разрешить выбирать несколько элементов (пользователей или групп) или только один элемент.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="1c5e8-156">Доступные варианты — `single`, `multiple`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="1c5e8-157">Значение по умолчанию — `multiple`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-157">Default value is `multiple`.</span></span>
| <span data-ttu-id="1c5e8-158">отключено</span><span class="sxs-lookup"><span data-stu-id="1c5e8-158">disabled</span></span> | <span data-ttu-id="1c5e8-159">отключено</span><span class="sxs-lookup"><span data-stu-id="1c5e8-159">disabled</span></span> | <span data-ttu-id="1c5e8-160">Задает отключение выборщика людей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-160">Sets whether the people picker is disabled.</span></span> <span data-ttu-id="1c5e8-161">При отключении пользователь не может искать или выбирать людей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-161">When disabled, the user is not able to search or select people.</span></span>

<span data-ttu-id="1c5e8-162">Ниже приведен пример `show-max`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-162">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="1c5e8-163">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="1c5e8-163">Selected people</span></span>

<span data-ttu-id="1c5e8-164">В разделе "Выбранные люди" компонента отображаются люди, выбранные разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-164">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="1c5e8-166">Вы можете заполнить данные о выбранных людях, выполнив одно из следующих действий.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-166">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="1c5e8-167">Задайте свойство `selectedPeople` напрямую, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-167">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="1c5e8-168">Используйте метод `selectUsersById()`, принимающий массив [ИД пользователей](/graph/api/resources/users) Microsoft Graph, чтобы найти сведения о связанных пользователях для выбора.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-168">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="1c5e8-169">**Примечание.** Если пользователь не найден по `id`, данные для этого `id` не будут отображаться.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-169">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="1c5e8-170">События</span><span class="sxs-lookup"><span data-stu-id="1c5e8-170">Events</span></span>

<span data-ttu-id="1c5e8-171">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-171">The following events are fired from the component.</span></span>

| <span data-ttu-id="1c5e8-172">Событие</span><span class="sxs-lookup"><span data-stu-id="1c5e8-172">Event</span></span> | <span data-ttu-id="1c5e8-173">Описание</span><span class="sxs-lookup"><span data-stu-id="1c5e8-173">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="1c5e8-174">Пользователь добавил или удалил человека из списка выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-174">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="1c5e8-175">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="1c5e8-175">CSS custom properties</span></span>

<span data-ttu-id="1c5e8-176">Компонент `mgt-people-picker` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-176">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="1c5e8-177">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="1c5e8-177">Templates</span></span>

 <span data-ttu-id="1c5e8-178">Компонент `mgt-people-picker` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-178">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="1c5e8-179">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-179">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="1c5e8-180">Тип данных</span><span class="sxs-lookup"><span data-stu-id="1c5e8-180">Data type</span></span> | <span data-ttu-id="1c5e8-181">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="1c5e8-181">Data context</span></span> | <span data-ttu-id="1c5e8-182">Описание</span><span class="sxs-lookup"><span data-stu-id="1c5e8-182">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1c5e8-183">default</span><span class="sxs-lookup"><span data-stu-id="1c5e8-183">default</span></span> | <span data-ttu-id="1c5e8-184">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="1c5e8-184">null: no data</span></span> | <span data-ttu-id="1c5e8-185">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-185">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="1c5e8-186">loading</span><span class="sxs-lookup"><span data-stu-id="1c5e8-186">loading</span></span> | <span data-ttu-id="1c5e8-187">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="1c5e8-187">null: no data</span></span> | <span data-ttu-id="1c5e8-188">Шаблон, используемый для отображения состояния средства выбора при выполнении запроса к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-188">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="1c5e8-189">error</span><span class="sxs-lookup"><span data-stu-id="1c5e8-189">error</span></span> | <span data-ttu-id="1c5e8-190">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="1c5e8-190">null: no data</span></span> | <span data-ttu-id="1c5e8-191">Шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-191">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="1c5e8-192">no-data</span><span class="sxs-lookup"><span data-stu-id="1c5e8-192">no-data</span></span> | <span data-ttu-id="1c5e8-193">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="1c5e8-193">null: no data</span></span> | <span data-ttu-id="1c5e8-194">Альтернативный шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-194">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="1c5e8-195">selected-person</span><span class="sxs-lookup"><span data-stu-id="1c5e8-195">selected-person</span></span> | <span data-ttu-id="1c5e8-196">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c5e8-196">person: The person details object</span></span> | <span data-ttu-id="1c5e8-197">Шаблон, отображающий выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-197">The template to render selected people.</span></span> |
| <span data-ttu-id="1c5e8-198">person</span><span class="sxs-lookup"><span data-stu-id="1c5e8-198">person</span></span> | <span data-ttu-id="1c5e8-199">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c5e8-199">person: The person details object</span></span> | <span data-ttu-id="1c5e8-200">Шаблон, отображающий людей в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-200">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="1c5e8-201">В следующих примерах показано, как использовать шаблон `error`.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-201">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1c5e8-202">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c5e8-202">Microsoft Graph permissions</span></span>

<span data-ttu-id="1c5e8-203">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-203">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="1c5e8-204">API</span><span class="sxs-lookup"><span data-stu-id="1c5e8-204">API</span></span>                                                                                                              | <span data-ttu-id="1c5e8-205">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1c5e8-205">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="1c5e8-206">/me/people</span><span class="sxs-lookup"><span data-stu-id="1c5e8-206">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="1c5e8-207">People.Read</span><span class="sxs-lookup"><span data-stu-id="1c5e8-207">People.Read</span></span>        |
| [<span data-ttu-id="1c5e8-208">/users</span><span class="sxs-lookup"><span data-stu-id="1c5e8-208">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="1c5e8-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1c5e8-209">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="1c5e8-210">/groups</span><span class="sxs-lookup"><span data-stu-id="1c5e8-210">/groups</span></span>](/group-list)  | <span data-ttu-id="1c5e8-211">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c5e8-211">Group.Read.All</span></span> |
| [<span data-ttu-id="1c5e8-212">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="1c5e8-212">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="1c5e8-213">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1c5e8-213">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="1c5e8-214">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="1c5e8-214">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="1c5e8-215">User.Read</span><span class="sxs-lookup"><span data-stu-id="1c5e8-215">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="1c5e8-216">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="1c5e8-216">Authentication</span></span>

<span data-ttu-id="1c5e8-217">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="1c5e8-217">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="1c5e8-218">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="1c5e8-218">Extend for more control</span></span>

<span data-ttu-id="1c5e8-219">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-219">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="1c5e8-220">Метод</span><span class="sxs-lookup"><span data-stu-id="1c5e8-220">Method</span></span> | <span data-ttu-id="1c5e8-221">Описание</span><span class="sxs-lookup"><span data-stu-id="1c5e8-221">Description</span></span> |
| - | - |
| <span data-ttu-id="1c5e8-222">renderInput</span><span class="sxs-lookup"><span data-stu-id="1c5e8-222">renderInput</span></span> | <span data-ttu-id="1c5e8-223">Отображает поле ввода.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-223">Renders the input text box.</span></span> |
| <span data-ttu-id="1c5e8-224">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="1c5e8-224">renderSelectedPeople</span></span> | <span data-ttu-id="1c5e8-225">Отображает маркеры выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-225">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="1c5e8-226">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="1c5e8-226">renderSelectedPerson</span></span> | <span data-ttu-id="1c5e8-227">Отображает маркер одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-227">Renders an individual person token.</span></span> |
| <span data-ttu-id="1c5e8-228">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="1c5e8-228">renderFlyout</span></span> | <span data-ttu-id="1c5e8-229">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-229">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="1c5e8-230">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="1c5e8-230">renderFlyoutContent</span></span> | <span data-ttu-id="1c5e8-231">Отображает соответствующее состояние во всплывающем окне результатов.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-231">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="1c5e8-232">renderLoading</span><span class="sxs-lookup"><span data-stu-id="1c5e8-232">renderLoading</span></span> | <span data-ttu-id="1c5e8-233">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-233">Renders the loading state.</span></span> |
| <span data-ttu-id="1c5e8-234">renderNoData</span><span class="sxs-lookup"><span data-stu-id="1c5e8-234">renderNoData</span></span> | <span data-ttu-id="1c5e8-235">Отображает состояние, если для поискового запроса не найдено результатов.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-235">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="1c5e8-236">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="1c5e8-236">renderSearchResults</span></span> | <span data-ttu-id="1c5e8-237">Отображает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-237">Renders the list of search results.</span></span> |
| <span data-ttu-id="1c5e8-238">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="1c5e8-238">renderPersonResult</span></span> | <span data-ttu-id="1c5e8-239">Отображает результаты поиска для одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c5e8-239">Renders an individual person search result.</span></span> |
