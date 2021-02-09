---
title: Компонент "Выбор людей"
description: Веб-компонент mgt-people-picker можно использовать для поиска указанного количества людей и отображать список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 691955aa64ff0afc42b5f8912658a6f36e1d77ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161378"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="b4cca-103">Компонент "Выбор людей" в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="b4cca-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="b4cca-104">Веб-компонент `mgt-people-picker` можно использовать для поиска людей и (или) групп.</span><span class="sxs-lookup"><span data-stu-id="b4cca-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="b4cca-105">По умолчанию компонент ищет всех людей и пользователей в организации, но вы можете изменить его поведение, чтобы также искать группы или только группы.</span><span class="sxs-lookup"><span data-stu-id="b4cca-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="b4cca-106">Вы также можете отфильтровать поиск по определенной группе.</span><span class="sxs-lookup"><span data-stu-id="b4cca-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="b4cca-107">Пример</span><span class="sxs-lookup"><span data-stu-id="b4cca-107">Example</span></span>

<span data-ttu-id="b4cca-108">В примере ниже показан компонент `mgt-people-picker`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="b4cca-109">Начните поиск имени, чтобы отобразить результаты, и используйте редактор кода, чтобы увидеть, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="b4cca-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="b4cca-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="b4cca-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="b4cca-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4cca-111">Properties</span></span>

<span data-ttu-id="b4cca-112">По умолчанию компонент `mgt-people-picker` извлекает людей из конечных точек `/me/people` и `/users`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="b4cca-113">Используйте следующие атрибуты, чтобы изменить его поведение.</span><span class="sxs-lookup"><span data-stu-id="b4cca-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="b4cca-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="b4cca-114">Attribute</span></span> | <span data-ttu-id="b4cca-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4cca-115">Property</span></span> | <span data-ttu-id="b4cca-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cca-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b4cca-117">show-max</span><span class="sxs-lookup"><span data-stu-id="b4cca-117">show-max</span></span> | <span data-ttu-id="b4cca-118">showMax</span><span class="sxs-lookup"><span data-stu-id="b4cca-118">showMax</span></span>   | <span data-ttu-id="b4cca-119">Числовое значение, указывающее максимальное количество отображаемых людей.</span><span class="sxs-lookup"><span data-stu-id="b4cca-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="b4cca-120">Значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="b4cca-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="b4cca-121">group-id</span><span class="sxs-lookup"><span data-stu-id="b4cca-121">group-id</span></span>    | <span data-ttu-id="b4cca-122">groupId</span><span class="sxs-lookup"><span data-stu-id="b4cca-122">groupId</span></span>     | <span data-ttu-id="b4cca-123">Значение строки, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="b4cca-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="b4cca-124">type</span><span class="sxs-lookup"><span data-stu-id="b4cca-124">type</span></span>     | <span data-ttu-id="b4cca-125">type</span><span class="sxs-lookup"><span data-stu-id="b4cca-125">type</span></span>      | <span data-ttu-id="b4cca-126">Тип объектов, которые необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="b4cca-126">The type of entities to search for.</span></span> <span data-ttu-id="b4cca-127">Доступные варианты — `person`, `group`, `any`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="b4cca-128">Значение по умолчанию — `person`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-128">Default value is `person`.</span></span> <span data-ttu-id="b4cca-129">Этот атрибут не оказывает влияния, если задано свойство `group-id`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="b4cca-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="b4cca-130">transitive-search</span></span>     | <span data-ttu-id="b4cca-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="b4cca-131">transitiveSearch</span></span>      | <span data-ttu-id="b4cca-132">Логическое значение для выполнения транзитивного поиска, возвращающего плоский список всех вложенных элементов. По умолчанию транзитивный поиск не используется.</span><span class="sxs-lookup"><span data-stu-id="b4cca-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="b4cca-133">group-type</span><span class="sxs-lookup"><span data-stu-id="b4cca-133">group-type</span></span>     | <span data-ttu-id="b4cca-134">groupType</span><span class="sxs-lookup"><span data-stu-id="b4cca-134">groupType</span></span>      | <span data-ttu-id="b4cca-135">Тип группы, которую необходимо найти.</span><span class="sxs-lookup"><span data-stu-id="b4cca-135">The group type to search for.</span></span> <span data-ttu-id="b4cca-136">Доступные варианты — `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="b4cca-137">Значение по умолчанию — `any`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-137">Default value is `any`.</span></span> <span data-ttu-id="b4cca-138">Этот атрибут не оказывает влияния, если для свойства `type` задано значение `person`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="b4cca-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="b4cca-139">selected-people</span></span>  | <span data-ttu-id="b4cca-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="b4cca-140">selectedPeople</span></span>     | <span data-ttu-id="b4cca-141">Массив выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="b4cca-141">An array of selected people.</span></span> <span data-ttu-id="b4cca-142">Установите это значение, чтобы выбрать людей программным образом.</span><span class="sxs-lookup"><span data-stu-id="b4cca-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="b4cca-143">people</span><span class="sxs-lookup"><span data-stu-id="b4cca-143">people</span></span>   | <span data-ttu-id="b4cca-144">people</span><span class="sxs-lookup"><span data-stu-id="b4cca-144">people</span></span>    | <span data-ttu-id="b4cca-145">Массив людей, найденных и отображенных в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="b4cca-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="b4cca-146">placeholder</span><span class="sxs-lookup"><span data-stu-id="b4cca-146">placeholder</span></span>   | <span data-ttu-id="b4cca-147">placeholder</span><span class="sxs-lookup"><span data-stu-id="b4cca-147">placeholder</span></span>    | <span data-ttu-id="b4cca-148">Текст по умолчанию, который объясняет, как использовать компонент.</span><span class="sxs-lookup"><span data-stu-id="b4cca-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="b4cca-149">Значение по умолчанию — `Start typing a name`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="b4cca-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="b4cca-150">default-selected-user-ids</span></span> | <span data-ttu-id="b4cca-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="b4cca-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="b4cca-152">При предоставлении строки разделенных запятой ИД пользователей Microsoft Graph, компонент отображает соответствующих пользователей как выбранных после инициализации.</span><span class="sxs-lookup"><span data-stu-id="b4cca-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="b4cca-153">selection-mode</span><span class="sxs-lookup"><span data-stu-id="b4cca-153">selection-mode</span></span> | <span data-ttu-id="b4cca-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="b4cca-154">selectionMode</span></span> | <span data-ttu-id="b4cca-155">Используется, чтобы указать следует ли разрешить выбирать несколько элементов (пользователей или групп) или только один элемент.</span><span class="sxs-lookup"><span data-stu-id="b4cca-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="b4cca-156">Доступные варианты — `single`, `multiple`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="b4cca-157">Значение по умолчанию — `multiple`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-157">Default value is `multiple`.</span></span>

<span data-ttu-id="b4cca-158">Ниже приведен пример `show-max`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-158">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="b4cca-159">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="b4cca-159">Selected people</span></span>

<span data-ttu-id="b4cca-160">В разделе "Выбранные люди" компонента отображаются люди, выбранные разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="b4cca-160">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="b4cca-162">Вы можете заполнить данные о выбранных людях, выполнив одно из следующих действий.</span><span class="sxs-lookup"><span data-stu-id="b4cca-162">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="b4cca-163">Задайте свойство `selectedPeople` напрямую, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="b4cca-163">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="b4cca-164">Используйте метод `selectUsersById()`, принимающий массив [ИД пользователей](/graph/api/resources/users) Microsoft Graph, чтобы найти сведения о связанных пользователях для выбора.</span><span class="sxs-lookup"><span data-stu-id="b4cca-164">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="b4cca-165">**Примечание.** Если пользователь не найден по `id`, данные для этого `id` не будут отображаться.</span><span class="sxs-lookup"><span data-stu-id="b4cca-165">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="b4cca-166">События</span><span class="sxs-lookup"><span data-stu-id="b4cca-166">Events</span></span>

<span data-ttu-id="b4cca-167">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="b4cca-167">The following events are fired from the component.</span></span>

| <span data-ttu-id="b4cca-168">Событие</span><span class="sxs-lookup"><span data-stu-id="b4cca-168">Event</span></span> | <span data-ttu-id="b4cca-169">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cca-169">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="b4cca-170">Пользователь добавил или удалил человека из списка выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="b4cca-170">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="b4cca-171">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="b4cca-171">CSS custom properties</span></span>

<span data-ttu-id="b4cca-172">Компонент `mgt-people-picker` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="b4cca-172">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="b4cca-173">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="b4cca-173">Templates</span></span>

 <span data-ttu-id="b4cca-174">Компонент `mgt-people-picker` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части.</span><span class="sxs-lookup"><span data-stu-id="b4cca-174">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="b4cca-175">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="b4cca-175">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="b4cca-176">Тип данных</span><span class="sxs-lookup"><span data-stu-id="b4cca-176">Data type</span></span> | <span data-ttu-id="b4cca-177">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="b4cca-177">Data context</span></span> | <span data-ttu-id="b4cca-178">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cca-178">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="b4cca-179">default</span><span class="sxs-lookup"><span data-stu-id="b4cca-179">default</span></span> | <span data-ttu-id="b4cca-180">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="b4cca-180">null: no data</span></span> | <span data-ttu-id="b4cca-181">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="b4cca-181">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="b4cca-182">loading</span><span class="sxs-lookup"><span data-stu-id="b4cca-182">loading</span></span> | <span data-ttu-id="b4cca-183">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="b4cca-183">null: no data</span></span> | <span data-ttu-id="b4cca-184">Шаблон, используемый для отображения состояния средства выбора при выполнении запроса к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b4cca-184">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="b4cca-185">error</span><span class="sxs-lookup"><span data-stu-id="b4cca-185">error</span></span> | <span data-ttu-id="b4cca-186">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="b4cca-186">null: no data</span></span> | <span data-ttu-id="b4cca-187">Шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="b4cca-187">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="b4cca-188">no-data</span><span class="sxs-lookup"><span data-stu-id="b4cca-188">no-data</span></span> | <span data-ttu-id="b4cca-189">null: нет данных</span><span class="sxs-lookup"><span data-stu-id="b4cca-189">null: no data</span></span> | <span data-ttu-id="b4cca-190">Альтернативный шаблон, используемый в том случае, если поиск не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="b4cca-190">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="b4cca-191">selected-person</span><span class="sxs-lookup"><span data-stu-id="b4cca-191">selected-person</span></span> | <span data-ttu-id="b4cca-192">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="b4cca-192">person: The person details object</span></span> | <span data-ttu-id="b4cca-193">Шаблон, отображающий выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="b4cca-193">The template to render selected people.</span></span> |
| <span data-ttu-id="b4cca-194">person</span><span class="sxs-lookup"><span data-stu-id="b4cca-194">person</span></span> | <span data-ttu-id="b4cca-195">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="b4cca-195">person: The person details object</span></span> | <span data-ttu-id="b4cca-196">Шаблон, отображающий людей в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="b4cca-196">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="b4cca-197">В следующих примерах показано, как использовать шаблон `error`.</span><span class="sxs-lookup"><span data-stu-id="b4cca-197">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="b4cca-198">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b4cca-198">Microsoft Graph permissions</span></span>

<span data-ttu-id="b4cca-199">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b4cca-199">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="b4cca-200">API</span><span class="sxs-lookup"><span data-stu-id="b4cca-200">API</span></span>                                                                                                              | <span data-ttu-id="b4cca-201">Разрешение</span><span class="sxs-lookup"><span data-stu-id="b4cca-201">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="b4cca-202">/me/people</span><span class="sxs-lookup"><span data-stu-id="b4cca-202">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="b4cca-203">People.Read</span><span class="sxs-lookup"><span data-stu-id="b4cca-203">People.Read</span></span>        |
| [<span data-ttu-id="b4cca-204">/users</span><span class="sxs-lookup"><span data-stu-id="b4cca-204">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="b4cca-205">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b4cca-205">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="b4cca-206">/groups</span><span class="sxs-lookup"><span data-stu-id="b4cca-206">/groups</span></span>](/group-list)  | <span data-ttu-id="b4cca-207">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4cca-207">Group.Read.All</span></span> |
| [<span data-ttu-id="b4cca-208">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="b4cca-208">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="b4cca-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b4cca-209">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="b4cca-210">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="b4cca-210">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="b4cca-211">User.Read</span><span class="sxs-lookup"><span data-stu-id="b4cca-211">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="b4cca-212">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="b4cca-212">Authentication</span></span>

<span data-ttu-id="b4cca-213">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="b4cca-213">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="b4cca-214">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="b4cca-214">Extend for more control</span></span>

<span data-ttu-id="b4cca-215">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="b4cca-215">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="b4cca-216">Метод</span><span class="sxs-lookup"><span data-stu-id="b4cca-216">Method</span></span> | <span data-ttu-id="b4cca-217">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cca-217">Description</span></span> |
| - | - |
| <span data-ttu-id="b4cca-218">renderInput</span><span class="sxs-lookup"><span data-stu-id="b4cca-218">renderInput</span></span> | <span data-ttu-id="b4cca-219">Отображает поле ввода.</span><span class="sxs-lookup"><span data-stu-id="b4cca-219">Renders the input text box.</span></span> |
| <span data-ttu-id="b4cca-220">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="b4cca-220">renderSelectedPeople</span></span> | <span data-ttu-id="b4cca-221">Отображает маркеры выбранных людей.</span><span class="sxs-lookup"><span data-stu-id="b4cca-221">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="b4cca-222">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="b4cca-222">renderSelectedPerson</span></span> | <span data-ttu-id="b4cca-223">Отображает маркер одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4cca-223">Renders an individual person token.</span></span> |
| <span data-ttu-id="b4cca-224">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="b4cca-224">renderFlyout</span></span> | <span data-ttu-id="b4cca-225">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="b4cca-225">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="b4cca-226">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="b4cca-226">renderFlyoutContent</span></span> | <span data-ttu-id="b4cca-227">Отображает соответствующее состояние во всплывающем окне результатов.</span><span class="sxs-lookup"><span data-stu-id="b4cca-227">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="b4cca-228">renderLoading</span><span class="sxs-lookup"><span data-stu-id="b4cca-228">renderLoading</span></span> | <span data-ttu-id="b4cca-229">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="b4cca-229">Renders the loading state.</span></span> |
| <span data-ttu-id="b4cca-230">renderNoData</span><span class="sxs-lookup"><span data-stu-id="b4cca-230">renderNoData</span></span> | <span data-ttu-id="b4cca-231">Отображает состояние, если для поискового запроса не найдено результатов.</span><span class="sxs-lookup"><span data-stu-id="b4cca-231">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="b4cca-232">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="b4cca-232">renderSearchResults</span></span> | <span data-ttu-id="b4cca-233">Отображает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="b4cca-233">Renders the list of search results.</span></span> |
| <span data-ttu-id="b4cca-234">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="b4cca-234">renderPersonResult</span></span> | <span data-ttu-id="b4cca-235">Отображает результаты поиска для одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4cca-235">Renders an individual person search result.</span></span> |
