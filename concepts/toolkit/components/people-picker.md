---
title: Компонент "Выбор людей"
description: Веб-компонент mgt-people-picker можно использовать для поиска указанного количества людей и отображать список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: dd3956e39450946a381b0b90851f248d7cf07b64
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52580024"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="3083f-103">Компонент "Выбор людей" в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="3083f-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3083f-104">Веб-компонент `mgt-people-picker` можно использовать для поиска людей и (или) групп.</span><span class="sxs-lookup"><span data-stu-id="3083f-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="3083f-105">По умолчанию компонент ищет всех людей и пользователей в организации, но вы можете изменить его поведение, чтобы также искать группы или только группы.</span><span class="sxs-lookup"><span data-stu-id="3083f-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="3083f-106">Вы также можете отфильтровать поиск по определенной группе.</span><span class="sxs-lookup"><span data-stu-id="3083f-106">You can also filter the search to a specific group.</span></span> <span data-ttu-id="3083f-107">Кроме того, вы можете разрешить пользователю вводить и выбирать любой адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3083f-107">Additionally, you can allow the user to enter and select any email address.</span></span>

## <a name="example"></a><span data-ttu-id="3083f-108">Пример</span><span class="sxs-lookup"><span data-stu-id="3083f-108">Example</span></span>

<span data-ttu-id="3083f-109">В примере ниже показан компонент `mgt-people-picker`.</span><span class="sxs-lookup"><span data-stu-id="3083f-109">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="3083f-110">Начните поиск имени, чтобы отобразить результаты, и используйте редактор кода, чтобы увидеть, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="3083f-110">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="3083f-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="3083f-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="3083f-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="3083f-112">Properties</span></span>

<span data-ttu-id="3083f-113">По умолчанию компонент `mgt-people-picker` извлекает людей из конечных точек `/me/people` и `/users`.</span><span class="sxs-lookup"><span data-stu-id="3083f-113">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="3083f-114">Используйте следующие атрибуты, чтобы изменить его поведение.</span><span class="sxs-lookup"><span data-stu-id="3083f-114">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="3083f-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="3083f-115">Attribute</span></span> | <span data-ttu-id="3083f-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="3083f-116">Property</span></span> | <span data-ttu-id="3083f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3083f-117">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3083f-118">show-max</span><span class="sxs-lookup"><span data-stu-id="3083f-118">show-max</span></span> | <span data-ttu-id="3083f-119">showMax</span><span class="sxs-lookup"><span data-stu-id="3083f-119">showMax</span></span>   | <span data-ttu-id="3083f-120">Числовое значение, указывающее максимальное количество отображаемых людей.</span><span class="sxs-lookup"><span data-stu-id="3083f-120">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="3083f-121">Значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="3083f-121">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="3083f-122">group-id</span><span class="sxs-lookup"><span data-stu-id="3083f-122">group-id</span></span>    | <span data-ttu-id="3083f-123">groupId</span><span class="sxs-lookup"><span data-stu-id="3083f-123">groupId</span></span>     | <span data-ttu-id="3083f-124">Значение строки, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="3083f-124">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="3083f-125">transitive-search</span><span class="sxs-lookup"><span data-stu-id="3083f-125">transitive-search</span></span>     | <span data-ttu-id="3083f-126">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="3083f-126">transitiveSearch</span></span>      | <span data-ttu-id="3083f-127">Логическое значение для выполнения транзитивного поиска, возвращающего плоский список всех вложенных элементов. По умолчанию транзитивный поиск не используется.</span><span class="sxs-lookup"><span data-stu-id="3083f-127">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="3083f-128">type</span><span class="sxs-lookup"><span data-stu-id="3083f-128">type</span></span>     | <span data-ttu-id="3083f-129">type</span><span class="sxs-lookup"><span data-stu-id="3083f-129">type</span></span>      | <span data-ttu-id="3083f-130">Тип объектов, которые необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="3083f-130">The type of entities to search for.</span></span> <span data-ttu-id="3083f-131">Доступные варианты — `person`, `group`, `any`.</span><span class="sxs-lookup"><span data-stu-id="3083f-131">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="3083f-132">Значение по умолчанию — `person`.</span><span class="sxs-lookup"><span data-stu-id="3083f-132">Default value is `person`.</span></span> <span data-ttu-id="3083f-133">Этот атрибут не оказывает влияния, если задано свойство `group-id`.</span><span class="sxs-lookup"><span data-stu-id="3083f-133">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="3083f-134">тип пользователя</span><span class="sxs-lookup"><span data-stu-id="3083f-134">user-type</span></span>     | <span data-ttu-id="3083f-135">userType</span><span class="sxs-lookup"><span data-stu-id="3083f-135">userType</span></span>      | <span data-ttu-id="3083f-136">Тип пользователя, для поиска.</span><span class="sxs-lookup"><span data-stu-id="3083f-136">The type of user to search for.</span></span> <span data-ttu-id="3083f-137">Доступные параметры: `any` для пользователей организации или для `user` `contact` контактов.</span><span class="sxs-lookup"><span data-stu-id="3083f-137">Available options are: `any`, `user` for organizational users, or `contact` for contacts.</span></span> <span data-ttu-id="3083f-138">Значение по умолчанию — `any`.</span><span class="sxs-lookup"><span data-stu-id="3083f-138">Default value is `any`.</span></span> |
| <span data-ttu-id="3083f-139">group-type</span><span class="sxs-lookup"><span data-stu-id="3083f-139">group-type</span></span>     | <span data-ttu-id="3083f-140">groupType</span><span class="sxs-lookup"><span data-stu-id="3083f-140">groupType</span></span>      | <span data-ttu-id="3083f-141">Тип группы, которую необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="3083f-141">The group type to search for.</span></span> <span data-ttu-id="3083f-142">Доступные варианты — `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span><span class="sxs-lookup"><span data-stu-id="3083f-142">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="3083f-143">Значение по умолчанию — `any`.</span><span class="sxs-lookup"><span data-stu-id="3083f-143">Default value is `any`.</span></span> <span data-ttu-id="3083f-144">Этот атрибут не оказывает влияния, если для свойства `type` задано значение `person`.</span><span class="sxs-lookup"><span data-stu-id="3083f-144">This attribute has no effect if the `type` property is set to `person`.</span></span>  |
| <span data-ttu-id="3083f-145">selected-people</span><span class="sxs-lookup"><span data-stu-id="3083f-145">selected-people</span></span>  | <span data-ttu-id="3083f-146">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="3083f-146">selectedPeople</span></span>     | <span data-ttu-id="3083f-147">Массив выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="3083f-147">An array of selected people.</span></span> <span data-ttu-id="3083f-148">Установите это значение, чтобы выбрать людей программным образом.</span><span class="sxs-lookup"><span data-stu-id="3083f-148">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="3083f-149">people</span><span class="sxs-lookup"><span data-stu-id="3083f-149">people</span></span>   | <span data-ttu-id="3083f-150">people</span><span class="sxs-lookup"><span data-stu-id="3083f-150">people</span></span>    | <span data-ttu-id="3083f-151">Массив людей, найденных и отображенных в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="3083f-151">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="3083f-152">placeholder</span><span class="sxs-lookup"><span data-stu-id="3083f-152">placeholder</span></span>   | <span data-ttu-id="3083f-153">placeholder</span><span class="sxs-lookup"><span data-stu-id="3083f-153">placeholder</span></span>    | <span data-ttu-id="3083f-154">Текст по умолчанию, который объясняет, как использовать компонент.</span><span class="sxs-lookup"><span data-stu-id="3083f-154">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="3083f-155">Значение по умолчанию — `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="3083f-155">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="3083f-156">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="3083f-156">default-selected-user-ids</span></span> | <span data-ttu-id="3083f-157">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="3083f-157">defaultSelectedUserIds</span></span> | <span data-ttu-id="3083f-158">При предоставлении строки разделенных запятой ИД пользователей Microsoft Graph, компонент отображает соответствующих пользователей как выбранных после инициализации.</span><span class="sxs-lookup"><span data-stu-id="3083f-158">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="3083f-159">по умолчанию выбранные группы-ids</span><span class="sxs-lookup"><span data-stu-id="3083f-159">default-selected-group-ids</span></span> | <span data-ttu-id="3083f-160">defaultSelectedGroupIds</span><span class="sxs-lookup"><span data-stu-id="3083f-160">defaultSelectedGroupIds</span></span> | <span data-ttu-id="3083f-161">Как и в случае с ids, выбранными по умолчанию, при выделении строки разделенных запятой ID microsoft Graph, компонент предоставляет соответствующие группы, выбранные после инициализации.</span><span class="sxs-lookup"><span data-stu-id="3083f-161">Similar to default-selected-user-ids, when provided a string of comma-separated Microsoft Graph group IDs, the component renders the respective groups as selected upon initialization.</span></span>
| <span data-ttu-id="3083f-162">selection-mode</span><span class="sxs-lookup"><span data-stu-id="3083f-162">selection-mode</span></span> | <span data-ttu-id="3083f-163">selectionMode</span><span class="sxs-lookup"><span data-stu-id="3083f-163">selectionMode</span></span> | <span data-ttu-id="3083f-164">Используется, чтобы указать следует ли разрешить выбирать несколько элементов (пользователей или групп) или только один элемент.</span><span class="sxs-lookup"><span data-stu-id="3083f-164">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="3083f-165">Доступные варианты — `single`, `multiple`.</span><span class="sxs-lookup"><span data-stu-id="3083f-165">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="3083f-166">Значение по умолчанию — `multiple`.</span><span class="sxs-lookup"><span data-stu-id="3083f-166">Default value is `multiple`.</span></span>
| <span data-ttu-id="3083f-167">отключено</span><span class="sxs-lookup"><span data-stu-id="3083f-167">disabled</span></span> | <span data-ttu-id="3083f-168">отключено</span><span class="sxs-lookup"><span data-stu-id="3083f-168">disabled</span></span> | <span data-ttu-id="3083f-169">Задает отключение выборщика людей.</span><span class="sxs-lookup"><span data-stu-id="3083f-169">Sets whether the people picker is disabled.</span></span> <span data-ttu-id="3083f-170">При отключении пользователь не может искать или выбирать людей.</span><span class="sxs-lookup"><span data-stu-id="3083f-170">When disabled, the user is not able to search or select people.</span></span>
| <span data-ttu-id="3083f-171">allow-any-email</span><span class="sxs-lookup"><span data-stu-id="3083f-171">allow-any-email</span></span> | <span data-ttu-id="3083f-172">allowAnyEmail</span><span class="sxs-lookup"><span data-stu-id="3083f-172">allowAnyEmail</span></span> | <span data-ttu-id="3083f-173">Указывает, может ли выборщик людей принимать адреса электронной почты без выбора человека.</span><span class="sxs-lookup"><span data-stu-id="3083f-173">Indicates whether the people picker can accept email addresses without selecting a person.</span></span> <span data-ttu-id="3083f-174">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="3083f-174">Default value is `false`.</span></span> <span data-ttu-id="3083f-175">Когда вы закончите вводить адрес электронной почты, вы можете нажать запятую (), запятую (), вкладку или ввести `,` `;` клавиши, чтобы добавить его.</span><span class="sxs-lookup"><span data-stu-id="3083f-175">When you finish typing an email address, you can press comma (`,`), semicolon (`;`), tab or enter keys to add it.</span></span>

<span data-ttu-id="3083f-176">Ниже приведен пример `show-max`.</span><span class="sxs-lookup"><span data-stu-id="3083f-176">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="3083f-177">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="3083f-177">Selected people</span></span>

<span data-ttu-id="3083f-178">В разделе "Выбранные люди" компонента отображаются люди, выбранные разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="3083f-178">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="3083f-180">Вы можете заполнить данные о выбранных людях, выполнив одно из следующих действий.</span><span class="sxs-lookup"><span data-stu-id="3083f-180">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="3083f-181">Задайте свойство `selectedPeople` напрямую, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="3083f-181">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="3083f-182">Используйте метод `selectUsersById()`, принимающий массив [ИД пользователей](/graph/api/resources/users) Microsoft Graph, чтобы найти сведения о связанных пользователях для выбора.</span><span class="sxs-lookup"><span data-stu-id="3083f-182">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="3083f-183">**Примечание.** Если пользователь не найден по `id`, данные для этого `id` не будут отображаться.</span><span class="sxs-lookup"><span data-stu-id="3083f-183">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="3083f-184">События</span><span class="sxs-lookup"><span data-stu-id="3083f-184">Events</span></span>

<span data-ttu-id="3083f-185">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="3083f-185">The following events are fired from the component.</span></span>

| <span data-ttu-id="3083f-186">Событие</span><span class="sxs-lookup"><span data-stu-id="3083f-186">Event</span></span> | <span data-ttu-id="3083f-187">Описание</span><span class="sxs-lookup"><span data-stu-id="3083f-187">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="3083f-188">Пользователь добавил или удалил человека из списка выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="3083f-188">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="3083f-189">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="3083f-189">CSS custom properties</span></span>

<span data-ttu-id="3083f-190">Компонент `mgt-people-picker` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="3083f-190">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="3083f-191">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="3083f-191">Templates</span></span>

 <span data-ttu-id="3083f-192">Компонент `mgt-people-picker` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части.</span><span class="sxs-lookup"><span data-stu-id="3083f-192">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="3083f-193">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="3083f-193">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="3083f-194">Тип данных</span><span class="sxs-lookup"><span data-stu-id="3083f-194">Data type</span></span> | <span data-ttu-id="3083f-195">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="3083f-195">Data context</span></span> | <span data-ttu-id="3083f-196">Описание</span><span class="sxs-lookup"><span data-stu-id="3083f-196">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="3083f-197">default</span><span class="sxs-lookup"><span data-stu-id="3083f-197">default</span></span> | <span data-ttu-id="3083f-198">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="3083f-198">null: no data</span></span> | <span data-ttu-id="3083f-199">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="3083f-199">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="3083f-200">loading</span><span class="sxs-lookup"><span data-stu-id="3083f-200">loading</span></span> | <span data-ttu-id="3083f-201">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="3083f-201">null: no data</span></span> | <span data-ttu-id="3083f-202">Шаблон, используемый для отображения состояния средства выбора при выполнении запроса к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3083f-202">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="3083f-203">error</span><span class="sxs-lookup"><span data-stu-id="3083f-203">error</span></span> | <span data-ttu-id="3083f-204">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="3083f-204">null: no data</span></span> | <span data-ttu-id="3083f-205">Шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="3083f-205">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="3083f-206">no-data</span><span class="sxs-lookup"><span data-stu-id="3083f-206">no-data</span></span> | <span data-ttu-id="3083f-207">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="3083f-207">null: no data</span></span> | <span data-ttu-id="3083f-208">Альтернативный шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="3083f-208">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="3083f-209">selected-person</span><span class="sxs-lookup"><span data-stu-id="3083f-209">selected-person</span></span> | <span data-ttu-id="3083f-210">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="3083f-210">person: The person details object</span></span> | <span data-ttu-id="3083f-211">Шаблон, отображающий выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="3083f-211">The template to render selected people.</span></span> |
| <span data-ttu-id="3083f-212">person</span><span class="sxs-lookup"><span data-stu-id="3083f-212">person</span></span> | <span data-ttu-id="3083f-213">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="3083f-213">person: The person details object</span></span> | <span data-ttu-id="3083f-214">Шаблон, отображающий людей в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="3083f-214">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="3083f-215">В следующих примерах показано, как использовать шаблон `error`.</span><span class="sxs-lookup"><span data-stu-id="3083f-215">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="3083f-216">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3083f-216">Microsoft Graph permissions</span></span>

<span data-ttu-id="3083f-217">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3083f-217">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="3083f-218">API</span><span class="sxs-lookup"><span data-stu-id="3083f-218">API</span></span>                                                                                                              | <span data-ttu-id="3083f-219">Разрешение</span><span class="sxs-lookup"><span data-stu-id="3083f-219">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="3083f-220">/me/people</span><span class="sxs-lookup"><span data-stu-id="3083f-220">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="3083f-221">People.Read</span><span class="sxs-lookup"><span data-stu-id="3083f-221">People.Read</span></span>        |
| [<span data-ttu-id="3083f-222">/users</span><span class="sxs-lookup"><span data-stu-id="3083f-222">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="3083f-223">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="3083f-223">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="3083f-224">/groups</span><span class="sxs-lookup"><span data-stu-id="3083f-224">/groups</span></span>](/group-list)  | <span data-ttu-id="3083f-225">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3083f-225">Group.Read.All</span></span> |
| [<span data-ttu-id="3083f-226">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="3083f-226">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="3083f-227">GroupMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="3083f-227">GroupMember.Read.All</span></span>        |
| [<span data-ttu-id="3083f-228">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="3083f-228">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="3083f-229">User.Read</span><span class="sxs-lookup"><span data-stu-id="3083f-229">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="3083f-230">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="3083f-230">Authentication</span></span>

<span data-ttu-id="3083f-231">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="3083f-231">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="3083f-232">Кэш</span><span class="sxs-lookup"><span data-stu-id="3083f-232">Cache</span></span>

|<span data-ttu-id="3083f-233">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="3083f-233">Object store</span></span>|<span data-ttu-id="3083f-234">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="3083f-234">Cached data</span></span>|<span data-ttu-id="3083f-235">Примечания</span><span class="sxs-lookup"><span data-stu-id="3083f-235">Remarks</span></span>|
|---------|-----------|-------|
|`groups`|<span data-ttu-id="3083f-236">Список групп</span><span class="sxs-lookup"><span data-stu-id="3083f-236">List of groups</span></span>|<span data-ttu-id="3083f-237">Используется, `type` когда установлено `PersonType.group`</span><span class="sxs-lookup"><span data-stu-id="3083f-237">Used when `type` is set to `PersonType.group`</span></span>|
|`people`|<span data-ttu-id="3083f-238">List of people</span><span class="sxs-lookup"><span data-stu-id="3083f-238">List of people</span></span>|<span data-ttu-id="3083f-239">Используется, `type` когда установлено `PersonType.person` или `PersonType.any`</span><span class="sxs-lookup"><span data-stu-id="3083f-239">Used when `type` is set to `PersonType.person` or `PersonType.any`</span></span>|
|`users`|<span data-ttu-id="3083f-240">Список пользователей</span><span class="sxs-lookup"><span data-stu-id="3083f-240">List of users</span></span>|<span data-ttu-id="3083f-241">Используется при `groupId` указании</span><span class="sxs-lookup"><span data-stu-id="3083f-241">Used when `groupId` specified</span></span>|

<span data-ttu-id="3083f-242">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="3083f-242">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="3083f-243">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="3083f-243">Extend for more control</span></span>

<span data-ttu-id="3083f-244">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="3083f-244">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="3083f-245">Метод</span><span class="sxs-lookup"><span data-stu-id="3083f-245">Method</span></span> | <span data-ttu-id="3083f-246">Описание</span><span class="sxs-lookup"><span data-stu-id="3083f-246">Description</span></span> |
| - | - |
| <span data-ttu-id="3083f-247">renderInput</span><span class="sxs-lookup"><span data-stu-id="3083f-247">renderInput</span></span> | <span data-ttu-id="3083f-248">Отображает поле ввода.</span><span class="sxs-lookup"><span data-stu-id="3083f-248">Renders the input text box.</span></span> |
| <span data-ttu-id="3083f-249">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="3083f-249">renderSelectedPeople</span></span> | <span data-ttu-id="3083f-250">Отображает маркеры выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="3083f-250">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="3083f-251">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="3083f-251">renderSelectedPerson</span></span> | <span data-ttu-id="3083f-252">Отображает маркер одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3083f-252">Renders an individual person token.</span></span> |
| <span data-ttu-id="3083f-253">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="3083f-253">renderFlyout</span></span> | <span data-ttu-id="3083f-254">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="3083f-254">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="3083f-255">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="3083f-255">renderFlyoutContent</span></span> | <span data-ttu-id="3083f-256">Отображает соответствующее состояние во всплывающем окне результатов.</span><span class="sxs-lookup"><span data-stu-id="3083f-256">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="3083f-257">renderLoading</span><span class="sxs-lookup"><span data-stu-id="3083f-257">renderLoading</span></span> | <span data-ttu-id="3083f-258">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="3083f-258">Renders the loading state.</span></span> |
| <span data-ttu-id="3083f-259">renderNoData</span><span class="sxs-lookup"><span data-stu-id="3083f-259">renderNoData</span></span> | <span data-ttu-id="3083f-260">Отображает состояние, если для поискового запроса не найдено результатов.</span><span class="sxs-lookup"><span data-stu-id="3083f-260">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="3083f-261">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="3083f-261">renderSearchResults</span></span> | <span data-ttu-id="3083f-262">Отображает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="3083f-262">Renders the list of search results.</span></span> |
| <span data-ttu-id="3083f-263">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="3083f-263">renderPersonResult</span></span> | <span data-ttu-id="3083f-264">Отображает результаты поиска для одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3083f-264">Renders an individual person search result.</span></span> |
