---
title: People-Picker компонента
description: Веб-компонент mgt-people-picker можно использовать для поиска указанного количества людей и отображения списка результатов через Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 9c23abbb3d525a3110cca31b21f2ee24d3c9f26d
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753776"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8d6f5-103">People-Picker компонента в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="8d6f5-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8d6f5-104">Веб-компонент `mgt-people-picker` можно использовать для поиска людей и/или групп.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="8d6f5-105">По умолчанию компонент будет искать всех людей и пользователей в организации, но вы можете изменить поведение, чтобы также искать группы или только группы.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="8d6f5-106">Вы также можете отфильтровать поиск по определенной группе.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="8d6f5-107">Пример</span><span class="sxs-lookup"><span data-stu-id="8d6f5-107">Example</span></span>

<span data-ttu-id="8d6f5-108">В следующем примере показан `mgt-people-picker` компонент.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="8d6f5-109">Начните поиск имени для отображения результатов и используйте [](#properties) редактор кода, чтобы увидеть, как свойства изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="8d6f5-110">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="8d6f5-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="8d6f5-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d6f5-111">Properties</span></span>

<span data-ttu-id="8d6f5-112">По умолчанию компонент `mgt-people-picker` получает людей из конечных `/me/people` `/users` точек и конечных точек.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="8d6f5-113">Чтобы изменить это поведение, используйте следующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="8d6f5-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="8d6f5-114">Attribute</span></span> | <span data-ttu-id="8d6f5-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d6f5-115">Property</span></span> | <span data-ttu-id="8d6f5-116">Описание</span><span class="sxs-lookup"><span data-stu-id="8d6f5-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8d6f5-117">show-max</span><span class="sxs-lookup"><span data-stu-id="8d6f5-117">show-max</span></span> | <span data-ttu-id="8d6f5-118">showMax</span><span class="sxs-lookup"><span data-stu-id="8d6f5-118">showMax</span></span>   | <span data-ttu-id="8d6f5-119">Значение числа, чтобы указать максимальное количество людей для показа.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="8d6f5-120">Значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="8d6f5-121">group-id</span><span class="sxs-lookup"><span data-stu-id="8d6f5-121">group-id</span></span>    | <span data-ttu-id="8d6f5-122">groupId</span><span class="sxs-lookup"><span data-stu-id="8d6f5-122">groupId</span></span>     | <span data-ttu-id="8d6f5-123">Строка, которая принадлежит определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="8d6f5-124">type</span><span class="sxs-lookup"><span data-stu-id="8d6f5-124">type</span></span>     | <span data-ttu-id="8d6f5-125">type</span><span class="sxs-lookup"><span data-stu-id="8d6f5-125">type</span></span>      | <span data-ttu-id="8d6f5-126">Тип сущностями, которые необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-126">The type of entities to search for.</span></span> <span data-ttu-id="8d6f5-127">Доступные варианты: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="8d6f5-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="8d6f5-128">Значение по умолчанию: `person`.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-128">Default value is `person`.</span></span> <span data-ttu-id="8d6f5-129">Этот атрибут не действует, если `group-id` заданной является свойство.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="8d6f5-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="8d6f5-130">transitive-search</span></span>     | <span data-ttu-id="8d6f5-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="8d6f5-131">transitiveSearch</span></span>      | <span data-ttu-id="8d6f5-132">Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="8d6f5-133">group-type</span><span class="sxs-lookup"><span data-stu-id="8d6f5-133">group-type</span></span>     | <span data-ttu-id="8d6f5-134">groupType</span><span class="sxs-lookup"><span data-stu-id="8d6f5-134">groupType</span></span>      | <span data-ttu-id="8d6f5-135">Тип группы для поиска.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-135">The group type to search for.</span></span> <span data-ttu-id="8d6f5-136">Доступные параметры: `unified` , `security` , , `mailenabledsecurity` `distribution` `any` .</span><span class="sxs-lookup"><span data-stu-id="8d6f5-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="8d6f5-137">Значение по умолчанию: `any`.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-137">Default value is `any`.</span></span> <span data-ttu-id="8d6f5-138">Этот атрибут не действует, если `type` для свойства установлено свойство `person` .</span><span class="sxs-lookup"><span data-stu-id="8d6f5-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="8d6f5-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="8d6f5-139">selected-people</span></span>  | <span data-ttu-id="8d6f5-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="8d6f5-140">selectedPeople</span></span>     | <span data-ttu-id="8d6f5-141">Массив выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-141">An array of selected people.</span></span> <span data-ttu-id="8d6f5-142">Установите это значение, чтобы выбрать людей программным путем.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="8d6f5-143">people</span><span class="sxs-lookup"><span data-stu-id="8d6f5-143">people</span></span>   | <span data-ttu-id="8d6f5-144">people</span><span class="sxs-lookup"><span data-stu-id="8d6f5-144">people</span></span>    | <span data-ttu-id="8d6f5-145">Массив людей, найденных и отрисовки в результатах поиска</span><span class="sxs-lookup"><span data-stu-id="8d6f5-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="8d6f5-146">placeholder</span><span class="sxs-lookup"><span data-stu-id="8d6f5-146">placeholder</span></span>   | <span data-ttu-id="8d6f5-147">placeholder</span><span class="sxs-lookup"><span data-stu-id="8d6f5-147">placeholder</span></span>    | <span data-ttu-id="8d6f5-148">Текст по умолчанию, который объясняет, как использовать компонент.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="8d6f5-149">Значение по умолчанию: `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="8d6f5-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="8d6f5-150">default-selected-user-ids</span></span> | <span data-ttu-id="8d6f5-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="8d6f5-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="8d6f5-152">Если предоставляется строка разделенных запятой пользовательских ИД Microsoft Graph, компонент отрисовка соответствующих пользователей, выбранных после инициализации.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="8d6f5-153">selection-mode</span><span class="sxs-lookup"><span data-stu-id="8d6f5-153">selection-mode</span></span> | <span data-ttu-id="8d6f5-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="8d6f5-154">selectionMode</span></span> | <span data-ttu-id="8d6f5-155">Используется для того, чтобы указать, следует ли выбирать несколько элементов (пользователей или групп) или только один элемент.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="8d6f5-156">Доступные варианты: `single` , `multiple` .</span><span class="sxs-lookup"><span data-stu-id="8d6f5-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="8d6f5-157">Значение по умолчанию: `multiple`.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-157">Default value is `multiple`.</span></span>

<span data-ttu-id="8d6f5-158">Ниже приводится `show-max` пример.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-158">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="8d6f5-159">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="8d6f5-159">Selected people</span></span>

<span data-ttu-id="8d6f5-160">В разделе "Выбранные люди" компонента отрисовка каждого пользователя, выбранного разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-160">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="8d6f5-162">Вы можете заполнить выбранные данные пользователей, выступая одним из следующих пунктов:</span><span class="sxs-lookup"><span data-stu-id="8d6f5-162">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="8d6f5-163">Настройка свойства `selectedPeople` напрямую, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-163">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="8d6f5-164">Использование метода, который принимает массив пользовательских ид Microsoft Graph для поиска связанных сведений `selectUsersById()` о пользователе для выбора. [](/graph/api/resources/users)</span><span class="sxs-lookup"><span data-stu-id="8d6f5-164">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="8d6f5-165">**Примечание.** Если для пользователя не найдено ни один пользователь, данные для этого не будут `id` отрисовки. `id`</span><span class="sxs-lookup"><span data-stu-id="8d6f5-165">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="8d6f5-166">События</span><span class="sxs-lookup"><span data-stu-id="8d6f5-166">Events</span></span>

<span data-ttu-id="8d6f5-167">Следующие события и происходят из компонента.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-167">The following events are fired from the component.</span></span>

| <span data-ttu-id="8d6f5-168">Событие</span><span class="sxs-lookup"><span data-stu-id="8d6f5-168">Event</span></span> | <span data-ttu-id="8d6f5-169">Описание</span><span class="sxs-lookup"><span data-stu-id="8d6f5-169">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="8d6f5-170">Пользователь добавил или удалил пользователя из списка выбранных или выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-170">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="8d6f5-171">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="8d6f5-171">CSS custom properties</span></span>

<span data-ttu-id="8d6f5-172">Компонент `mgt-people-picker` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-172">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="8d6f5-173">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="8d6f5-173">Templates</span></span>

 <span data-ttu-id="8d6f5-174">`mgt-people-picker` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-174">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="8d6f5-175">Чтобы указать шаблон, включив элемент в `<template>` компонент, закажите одно из `data-type` следующих значений.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-175">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="8d6f5-176">Тип данных</span><span class="sxs-lookup"><span data-stu-id="8d6f5-176">Data type</span></span> | <span data-ttu-id="8d6f5-177">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="8d6f5-177">Data context</span></span> | <span data-ttu-id="8d6f5-178">Описание</span><span class="sxs-lookup"><span data-stu-id="8d6f5-178">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8d6f5-179">default</span><span class="sxs-lookup"><span data-stu-id="8d6f5-179">default</span></span> | <span data-ttu-id="8d6f5-180">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="8d6f5-180">null: no data</span></span> | <span data-ttu-id="8d6f5-181">Шаблон, используемый для переопределения отрисовки всего компонента.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-181">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="8d6f5-182">loading</span><span class="sxs-lookup"><span data-stu-id="8d6f5-182">loading</span></span> | <span data-ttu-id="8d6f5-183">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="8d6f5-183">null: no data</span></span> | <span data-ttu-id="8d6f5-184">Шаблон, используемый для отображения состояния picker во время запроса графа.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-184">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="8d6f5-185">error</span><span class="sxs-lookup"><span data-stu-id="8d6f5-185">error</span></span> | <span data-ttu-id="8d6f5-186">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="8d6f5-186">null: no data</span></span> | <span data-ttu-id="8d6f5-187">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-187">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="8d6f5-188">no-data</span><span class="sxs-lookup"><span data-stu-id="8d6f5-188">no-data</span></span> | <span data-ttu-id="8d6f5-189">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="8d6f5-189">null: no data</span></span> | <span data-ttu-id="8d6f5-190">Альтернативный шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-190">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="8d6f5-191">selected-person</span><span class="sxs-lookup"><span data-stu-id="8d6f5-191">selected-person</span></span> | <span data-ttu-id="8d6f5-192">person: объект сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="8d6f5-192">person: The person details object</span></span> | <span data-ttu-id="8d6f5-193">Шаблон для отображения выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-193">The template to render selected people.</span></span> |
| <span data-ttu-id="8d6f5-194">person</span><span class="sxs-lookup"><span data-stu-id="8d6f5-194">person</span></span> | <span data-ttu-id="8d6f5-195">person: объект сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="8d6f5-195">person: The person details object</span></span> | <span data-ttu-id="8d6f5-196">Шаблон для отображения людей в выпадаемом меню.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-196">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="8d6f5-197">В следующих примерах показано, как использовать `error` шаблон.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-197">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8d6f5-198">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d6f5-198">Microsoft Graph permissions</span></span>

<span data-ttu-id="8d6f5-199">Этот компонент использует следующие API Microsoft Graph и разрешения.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-199">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="8d6f5-200">API</span><span class="sxs-lookup"><span data-stu-id="8d6f5-200">API</span></span>                                                                                                              | <span data-ttu-id="8d6f5-201">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8d6f5-201">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="8d6f5-202">/me/people</span><span class="sxs-lookup"><span data-stu-id="8d6f5-202">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="8d6f5-203">People.Read</span><span class="sxs-lookup"><span data-stu-id="8d6f5-203">People.Read</span></span>        |
| [<span data-ttu-id="8d6f5-204">/users</span><span class="sxs-lookup"><span data-stu-id="8d6f5-204">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="8d6f5-205">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="8d6f5-205">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="8d6f5-206">/groups</span><span class="sxs-lookup"><span data-stu-id="8d6f5-206">/groups</span></span>](/group-list)  | <span data-ttu-id="8d6f5-207">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d6f5-207">Group.Read.All</span></span> |
| [<span data-ttu-id="8d6f5-208">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="8d6f5-208">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="8d6f5-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="8d6f5-209">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="8d6f5-210">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="8d6f5-210">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="8d6f5-211">User.Read</span><span class="sxs-lookup"><span data-stu-id="8d6f5-211">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="8d6f5-212">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="8d6f5-212">Authentication</span></span>

<span data-ttu-id="8d6f5-213">Этот контроль использует глобального поставщика проверки подлинности, описанного в [документации по проверке подлинности.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="8d6f5-213">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="8d6f5-214">Расширение для большего контроля</span><span class="sxs-lookup"><span data-stu-id="8d6f5-214">Extend for more control</span></span>

<span data-ttu-id="8d6f5-215">Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-215">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="8d6f5-216">Метод</span><span class="sxs-lookup"><span data-stu-id="8d6f5-216">Method</span></span> | <span data-ttu-id="8d6f5-217">Описание</span><span class="sxs-lookup"><span data-stu-id="8d6f5-217">Description</span></span> |
| - | - |
| <span data-ttu-id="8d6f5-218">renderInput</span><span class="sxs-lookup"><span data-stu-id="8d6f5-218">renderInput</span></span> | <span data-ttu-id="8d6f5-219">Отрисовка текстового окна ввода.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-219">Renders the input text box.</span></span> |
| <span data-ttu-id="8d6f5-220">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="8d6f5-220">renderSelectedPeople</span></span> | <span data-ttu-id="8d6f5-221">Отрисовка выбранных маркеров людей.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-221">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="8d6f5-222">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="8d6f5-222">renderSelectedPerson</span></span> | <span data-ttu-id="8d6f5-223">Отрисовка маркера отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-223">Renders an individual person token.</span></span> |
| <span data-ttu-id="8d6f5-224">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="8d6f5-224">renderFlyout</span></span> | <span data-ttu-id="8d6f5-225">Отрисовка хрома во весь экран.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-225">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="8d6f5-226">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="8d6f5-226">renderFlyoutContent</span></span> | <span data-ttu-id="8d6f5-227">Отрисовка соответствующего состояния во flyout результатов.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-227">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="8d6f5-228">renderLoading</span><span class="sxs-lookup"><span data-stu-id="8d6f5-228">renderLoading</span></span> | <span data-ttu-id="8d6f5-229">Отрисовка состояния загрузки.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-229">Renders the loading state.</span></span> |
| <span data-ttu-id="8d6f5-230">renderNoData</span><span class="sxs-lookup"><span data-stu-id="8d6f5-230">renderNoData</span></span> | <span data-ttu-id="8d6f5-231">Отрисовка состояния, когда результаты для поискового запроса не найдены.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-231">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="8d6f5-232">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="8d6f5-232">renderSearchResults</span></span> | <span data-ttu-id="8d6f5-233">Отрисовка списка результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-233">Renders the list of search results.</span></span> |
| <span data-ttu-id="8d6f5-234">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="8d6f5-234">renderPersonResult</span></span> | <span data-ttu-id="8d6f5-235">Отрисовка результата поиска отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="8d6f5-235">Renders an individual person search result.</span></span> |
