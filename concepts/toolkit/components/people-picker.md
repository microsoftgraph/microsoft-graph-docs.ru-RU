---
title: Компонент "Выбор людей"
description: Веб-компонент mgt-people-picker можно использовать для поиска указанного количества людей и отображать список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3531c32ae4f33898b11f7d92f91115aa1cbf43a3
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266817"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f4fcf-103">Компонент "Выбор людей" в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f4fcf-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f4fcf-104">Веб-компонент `mgt-people-picker` можно использовать для поиска людей и (или) групп.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="f4fcf-105">По умолчанию компонент ищет всех людей и пользователей в организации, но вы можете изменить его поведение, чтобы также искать группы или только группы.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="f4fcf-106">Вы также можете отфильтровать поиск по определенной группе.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="f4fcf-107">Пример</span><span class="sxs-lookup"><span data-stu-id="f4fcf-107">Example</span></span>

<span data-ttu-id="f4fcf-108">В примере ниже показан компонент `mgt-people-picker`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="f4fcf-109">Начните поиск имени, чтобы отобразить результаты, и используйте редактор кода, чтобы увидеть, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="f4fcf-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="f4fcf-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="f4fcf-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4fcf-111">Properties</span></span>

<span data-ttu-id="f4fcf-112">По умолчанию компонент `mgt-people-picker` извлекает людей из конечных точек `/me/people` и `/users`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="f4fcf-113">Используйте следующие атрибуты, чтобы изменить его поведение.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="f4fcf-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="f4fcf-114">Attribute</span></span> | <span data-ttu-id="f4fcf-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4fcf-115">Property</span></span> | <span data-ttu-id="f4fcf-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fcf-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f4fcf-117">show-max</span><span class="sxs-lookup"><span data-stu-id="f4fcf-117">show-max</span></span> | <span data-ttu-id="f4fcf-118">showMax</span><span class="sxs-lookup"><span data-stu-id="f4fcf-118">showMax</span></span>   | <span data-ttu-id="f4fcf-119">Числовое значение, указывающее максимальное количество отображаемых людей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="f4fcf-120">Значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="f4fcf-121">group-id</span><span class="sxs-lookup"><span data-stu-id="f4fcf-121">group-id</span></span>    | <span data-ttu-id="f4fcf-122">groupId</span><span class="sxs-lookup"><span data-stu-id="f4fcf-122">groupId</span></span>     | <span data-ttu-id="f4fcf-123">Значение строки, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="f4fcf-124">type</span><span class="sxs-lookup"><span data-stu-id="f4fcf-124">type</span></span>     | <span data-ttu-id="f4fcf-125">type</span><span class="sxs-lookup"><span data-stu-id="f4fcf-125">type</span></span>      | <span data-ttu-id="f4fcf-126">Тип объектов, которые необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-126">The type of entities to search for.</span></span> <span data-ttu-id="f4fcf-127">Доступные варианты — `person`, `group`, `any`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="f4fcf-128">Значение по умолчанию — `person`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-128">Default value is `person`.</span></span> <span data-ttu-id="f4fcf-129">Этот атрибут не оказывает влияния, если задано свойство `group-id`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="f4fcf-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="f4fcf-130">transitive-search</span></span>     | <span data-ttu-id="f4fcf-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="f4fcf-131">transitiveSearch</span></span>      | <span data-ttu-id="f4fcf-132">Логическое значение для выполнения транзитивного поиска, возвращающего плоский список всех вложенных элементов. По умолчанию транзитивный поиск не используется.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="f4fcf-133">group-type</span><span class="sxs-lookup"><span data-stu-id="f4fcf-133">group-type</span></span>     | <span data-ttu-id="f4fcf-134">groupType</span><span class="sxs-lookup"><span data-stu-id="f4fcf-134">groupType</span></span>      | <span data-ttu-id="f4fcf-135">Тип группы, которую необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-135">The group type to search for.</span></span> <span data-ttu-id="f4fcf-136">Доступные варианты — `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="f4fcf-137">Значение по умолчанию — `any`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-137">Default value is `any`.</span></span> <span data-ttu-id="f4fcf-138">Этот атрибут не оказывает влияния, если для свойства `type` задано значение `person`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="f4fcf-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="f4fcf-139">selected-people</span></span>  | <span data-ttu-id="f4fcf-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="f4fcf-140">selectedPeople</span></span>     | <span data-ttu-id="f4fcf-141">Массив выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-141">An array of selected people.</span></span> <span data-ttu-id="f4fcf-142">Установите это значение, чтобы выбрать людей программным образом.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="f4fcf-143">people</span><span class="sxs-lookup"><span data-stu-id="f4fcf-143">people</span></span>   | <span data-ttu-id="f4fcf-144">people</span><span class="sxs-lookup"><span data-stu-id="f4fcf-144">people</span></span>    | <span data-ttu-id="f4fcf-145">Массив людей, найденных и отображенных в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="f4fcf-146">placeholder</span><span class="sxs-lookup"><span data-stu-id="f4fcf-146">placeholder</span></span>   | <span data-ttu-id="f4fcf-147">placeholder</span><span class="sxs-lookup"><span data-stu-id="f4fcf-147">placeholder</span></span>    | <span data-ttu-id="f4fcf-148">Текст по умолчанию, который объясняет, как использовать компонент.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="f4fcf-149">Значение по умолчанию — `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="f4fcf-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="f4fcf-150">default-selected-user-ids</span></span> | <span data-ttu-id="f4fcf-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="f4fcf-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="f4fcf-152">При предоставлении строки разделенных запятой ИД пользователей Microsoft Graph, компонент отображает соответствующих пользователей как выбранных после инициализации.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="f4fcf-153">selection-mode</span><span class="sxs-lookup"><span data-stu-id="f4fcf-153">selection-mode</span></span> | <span data-ttu-id="f4fcf-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="f4fcf-154">selectionMode</span></span> | <span data-ttu-id="f4fcf-155">Используется, чтобы указать следует ли разрешить выбирать несколько элементов (пользователей или групп) или только один элемент.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="f4fcf-156">Доступные варианты — `single`, `multiple`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="f4fcf-157">Значение по умолчанию — `multiple`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-157">Default value is `multiple`.</span></span>
| <span data-ttu-id="f4fcf-158">отключено</span><span class="sxs-lookup"><span data-stu-id="f4fcf-158">disabled</span></span> | <span data-ttu-id="f4fcf-159">отключено</span><span class="sxs-lookup"><span data-stu-id="f4fcf-159">disabled</span></span> | <span data-ttu-id="f4fcf-160">Задает отключение выборщика людей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-160">Sets whether the people picker is disabled.</span></span> <span data-ttu-id="f4fcf-161">При отключении пользователь не может искать или выбирать людей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-161">When disabled, the user is not able to search or select people.</span></span>

<span data-ttu-id="f4fcf-162">Ниже приведен пример `show-max`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-162">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="f4fcf-163">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="f4fcf-163">Selected people</span></span>

<span data-ttu-id="f4fcf-164">В разделе "Выбранные люди" компонента отображаются люди, выбранные разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-164">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="f4fcf-166">Вы можете заполнить данные о выбранных людях, выполнив одно из следующих действий.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-166">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="f4fcf-167">Задайте свойство `selectedPeople` напрямую, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-167">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="f4fcf-168">Используйте метод `selectUsersById()`, принимающий массив [ИД пользователей](/graph/api/resources/users) Microsoft Graph, чтобы найти сведения о связанных пользователях для выбора.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-168">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="f4fcf-169">**Примечание.** Если пользователь не найден по `id`, данные для этого `id` не будут отображаться.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-169">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="f4fcf-170">События</span><span class="sxs-lookup"><span data-stu-id="f4fcf-170">Events</span></span>

<span data-ttu-id="f4fcf-171">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-171">The following events are fired from the component.</span></span>

| <span data-ttu-id="f4fcf-172">Событие</span><span class="sxs-lookup"><span data-stu-id="f4fcf-172">Event</span></span> | <span data-ttu-id="f4fcf-173">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fcf-173">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="f4fcf-174">Пользователь добавил или удалил человека из списка выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-174">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="f4fcf-175">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="f4fcf-175">CSS custom properties</span></span>

<span data-ttu-id="f4fcf-176">Компонент `mgt-people-picker` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-176">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="f4fcf-177">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="f4fcf-177">Templates</span></span>

 <span data-ttu-id="f4fcf-178">Компонент `mgt-people-picker` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-178">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="f4fcf-179">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-179">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f4fcf-180">Тип данных</span><span class="sxs-lookup"><span data-stu-id="f4fcf-180">Data type</span></span> | <span data-ttu-id="f4fcf-181">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="f4fcf-181">Data context</span></span> | <span data-ttu-id="f4fcf-182">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fcf-182">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f4fcf-183">default</span><span class="sxs-lookup"><span data-stu-id="f4fcf-183">default</span></span> | <span data-ttu-id="f4fcf-184">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="f4fcf-184">null: no data</span></span> | <span data-ttu-id="f4fcf-185">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-185">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="f4fcf-186">loading</span><span class="sxs-lookup"><span data-stu-id="f4fcf-186">loading</span></span> | <span data-ttu-id="f4fcf-187">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="f4fcf-187">null: no data</span></span> | <span data-ttu-id="f4fcf-188">Шаблон, используемый для отображения состояния средства выбора при выполнении запроса к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-188">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="f4fcf-189">error</span><span class="sxs-lookup"><span data-stu-id="f4fcf-189">error</span></span> | <span data-ttu-id="f4fcf-190">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="f4fcf-190">null: no data</span></span> | <span data-ttu-id="f4fcf-191">Шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-191">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="f4fcf-192">no-data</span><span class="sxs-lookup"><span data-stu-id="f4fcf-192">no-data</span></span> | <span data-ttu-id="f4fcf-193">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="f4fcf-193">null: no data</span></span> | <span data-ttu-id="f4fcf-194">Альтернативный шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-194">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="f4fcf-195">selected-person</span><span class="sxs-lookup"><span data-stu-id="f4fcf-195">selected-person</span></span> | <span data-ttu-id="f4fcf-196">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="f4fcf-196">person: The person details object</span></span> | <span data-ttu-id="f4fcf-197">Шаблон, отображающий выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-197">The template to render selected people.</span></span> |
| <span data-ttu-id="f4fcf-198">person</span><span class="sxs-lookup"><span data-stu-id="f4fcf-198">person</span></span> | <span data-ttu-id="f4fcf-199">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="f4fcf-199">person: The person details object</span></span> | <span data-ttu-id="f4fcf-200">Шаблон, отображающий людей в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-200">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="f4fcf-201">В следующих примерах показано, как использовать шаблон `error`.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-201">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f4fcf-202">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f4fcf-202">Microsoft Graph permissions</span></span>

<span data-ttu-id="f4fcf-203">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-203">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="f4fcf-204">API</span><span class="sxs-lookup"><span data-stu-id="f4fcf-204">API</span></span>                                                                                                              | <span data-ttu-id="f4fcf-205">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f4fcf-205">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="f4fcf-206">/me/people</span><span class="sxs-lookup"><span data-stu-id="f4fcf-206">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="f4fcf-207">People.Read</span><span class="sxs-lookup"><span data-stu-id="f4fcf-207">People.Read</span></span>        |
| [<span data-ttu-id="f4fcf-208">/users</span><span class="sxs-lookup"><span data-stu-id="f4fcf-208">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="f4fcf-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f4fcf-209">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="f4fcf-210">/groups</span><span class="sxs-lookup"><span data-stu-id="f4fcf-210">/groups</span></span>](/group-list)  | <span data-ttu-id="f4fcf-211">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4fcf-211">Group.Read.All</span></span> |
| [<span data-ttu-id="f4fcf-212">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="f4fcf-212">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="f4fcf-213">GroupMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4fcf-213">GroupMember.Read.All</span></span>        |
| [<span data-ttu-id="f4fcf-214">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="f4fcf-214">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="f4fcf-215">User.Read</span><span class="sxs-lookup"><span data-stu-id="f4fcf-215">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="f4fcf-216">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="f4fcf-216">Authentication</span></span>

<span data-ttu-id="f4fcf-217">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="f4fcf-217">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="f4fcf-218">Кэш</span><span class="sxs-lookup"><span data-stu-id="f4fcf-218">Cache</span></span>

|<span data-ttu-id="f4fcf-219">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="f4fcf-219">Object store</span></span>|<span data-ttu-id="f4fcf-220">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="f4fcf-220">Cached data</span></span>|<span data-ttu-id="f4fcf-221">Примечания</span><span class="sxs-lookup"><span data-stu-id="f4fcf-221">Remarks</span></span>|
|---------|-----------|-------|
|`groups`|<span data-ttu-id="f4fcf-222">Список групп</span><span class="sxs-lookup"><span data-stu-id="f4fcf-222">List of groups</span></span>|<span data-ttu-id="f4fcf-223">Используется, `type` когда установлено `PersonType.group`</span><span class="sxs-lookup"><span data-stu-id="f4fcf-223">Used when `type` is set to `PersonType.group`</span></span>|
|`people`|<span data-ttu-id="f4fcf-224">List of people</span><span class="sxs-lookup"><span data-stu-id="f4fcf-224">List of people</span></span>|<span data-ttu-id="f4fcf-225">Используется, `type` когда установлено `PersonType.person` или `PersonType.any`</span><span class="sxs-lookup"><span data-stu-id="f4fcf-225">Used when `type` is set to `PersonType.person` or `PersonType.any`</span></span>|
|`users`|<span data-ttu-id="f4fcf-226">Список пользователей</span><span class="sxs-lookup"><span data-stu-id="f4fcf-226">List of users</span></span>|<span data-ttu-id="f4fcf-227">Используется при `groupId` указании</span><span class="sxs-lookup"><span data-stu-id="f4fcf-227">Used when `groupId` specified</span></span>|

<span data-ttu-id="f4fcf-228">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="f4fcf-228">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="f4fcf-229">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="f4fcf-229">Extend for more control</span></span>

<span data-ttu-id="f4fcf-230">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-230">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="f4fcf-231">Метод</span><span class="sxs-lookup"><span data-stu-id="f4fcf-231">Method</span></span> | <span data-ttu-id="f4fcf-232">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fcf-232">Description</span></span> |
| - | - |
| <span data-ttu-id="f4fcf-233">renderInput</span><span class="sxs-lookup"><span data-stu-id="f4fcf-233">renderInput</span></span> | <span data-ttu-id="f4fcf-234">Отображает поле ввода.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-234">Renders the input text box.</span></span> |
| <span data-ttu-id="f4fcf-235">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="f4fcf-235">renderSelectedPeople</span></span> | <span data-ttu-id="f4fcf-236">Отображает маркеры выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-236">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="f4fcf-237">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="f4fcf-237">renderSelectedPerson</span></span> | <span data-ttu-id="f4fcf-238">Отображает маркер одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-238">Renders an individual person token.</span></span> |
| <span data-ttu-id="f4fcf-239">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="f4fcf-239">renderFlyout</span></span> | <span data-ttu-id="f4fcf-240">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-240">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="f4fcf-241">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="f4fcf-241">renderFlyoutContent</span></span> | <span data-ttu-id="f4fcf-242">Отображает соответствующее состояние во всплывающем окне результатов.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-242">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="f4fcf-243">renderLoading</span><span class="sxs-lookup"><span data-stu-id="f4fcf-243">renderLoading</span></span> | <span data-ttu-id="f4fcf-244">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-244">Renders the loading state.</span></span> |
| <span data-ttu-id="f4fcf-245">renderNoData</span><span class="sxs-lookup"><span data-stu-id="f4fcf-245">renderNoData</span></span> | <span data-ttu-id="f4fcf-246">Отображает состояние, если для поискового запроса не найдено результатов.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-246">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="f4fcf-247">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="f4fcf-247">renderSearchResults</span></span> | <span data-ttu-id="f4fcf-248">Отображает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-248">Renders the list of search results.</span></span> |
| <span data-ttu-id="f4fcf-249">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="f4fcf-249">renderPersonResult</span></span> | <span data-ttu-id="f4fcf-250">Отображает результаты поиска для одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fcf-250">Renders an individual person search result.</span></span> |
