---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: eca2ad4c0b56ff3475480a36eab2e943e3b6d9e4
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288618"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="414c5-103">Компонент "Выбор людей" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="414c5-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="414c5-104">Вы можете использовать `mgt-people-picker` веб-компонент для поиска людей и/или групп.</span><span class="sxs-lookup"><span data-stu-id="414c5-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="414c5-105">По умолчанию компонент будет выполнять поиск всех людей и пользователей в Организации, но вы можете изменить поведение, чтобы также выполнить поиск групп или только групп.</span><span class="sxs-lookup"><span data-stu-id="414c5-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="414c5-106">Вы также можете отфильтровать поиск в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="414c5-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="414c5-107">Пример</span><span class="sxs-lookup"><span data-stu-id="414c5-107">Example</span></span>

<span data-ttu-id="414c5-108">В приведенном ниже примере показан `mgt-people-picker` компонент.</span><span class="sxs-lookup"><span data-stu-id="414c5-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="414c5-109">Начните поиск имени, чтобы увидеть результаты, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="414c5-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="414c5-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="414c5-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="414c5-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="414c5-111">Properties</span></span>

<span data-ttu-id="414c5-112">По умолчанию `mgt-people-picker` компонент получает пользователей из `/me/people` `/users` конечных точек и.</span><span class="sxs-lookup"><span data-stu-id="414c5-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="414c5-113">Используйте следующие атрибуты, чтобы изменить это поведение.</span><span class="sxs-lookup"><span data-stu-id="414c5-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="414c5-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="414c5-114">Attribute</span></span> | <span data-ttu-id="414c5-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="414c5-115">Property</span></span> | <span data-ttu-id="414c5-116">Описание</span><span class="sxs-lookup"><span data-stu-id="414c5-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="414c5-117">Show — Max</span><span class="sxs-lookup"><span data-stu-id="414c5-117">show-max</span></span> | <span data-ttu-id="414c5-118">шовмакс</span><span class="sxs-lookup"><span data-stu-id="414c5-118">showMax</span></span>   | <span data-ttu-id="414c5-119">Числовое значение, указывающее максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="414c5-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="414c5-120">значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="414c5-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="414c5-121">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="414c5-121">group-id</span></span>    | <span data-ttu-id="414c5-122">groupId</span><span class="sxs-lookup"><span data-stu-id="414c5-122">groupId</span></span>     | <span data-ttu-id="414c5-123">Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="414c5-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="414c5-124">type</span><span class="sxs-lookup"><span data-stu-id="414c5-124">type</span></span>     | <span data-ttu-id="414c5-125">type</span><span class="sxs-lookup"><span data-stu-id="414c5-125">type</span></span>      | <span data-ttu-id="414c5-126">Тип сущностей для поиска.</span><span class="sxs-lookup"><span data-stu-id="414c5-126">The type of entities to search for.</span></span> <span data-ttu-id="414c5-127">Доступные параметры: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="414c5-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="414c5-128">Значение по умолчанию: `person`.</span><span class="sxs-lookup"><span data-stu-id="414c5-128">Default value is `person`.</span></span> <span data-ttu-id="414c5-129">Этот атрибут не оказывает никакого действия `group-id` , если свойство задано.</span><span class="sxs-lookup"><span data-stu-id="414c5-129">This attribute has no effect if `group-id` property is set.</span></span>                                                                            |
| <span data-ttu-id="414c5-130">Тип группы</span><span class="sxs-lookup"><span data-stu-id="414c5-130">group-type</span></span>     | <span data-ttu-id="414c5-131">groupType</span><span class="sxs-lookup"><span data-stu-id="414c5-131">groupType</span></span>      | <span data-ttu-id="414c5-132">Тип группы для поиска.</span><span class="sxs-lookup"><span data-stu-id="414c5-132">The group type to search for.</span></span> <span data-ttu-id="414c5-133">Доступные варианты: `unified` ,, `security` `mailenabledsecurity` , `distribution` , `any` .</span><span class="sxs-lookup"><span data-stu-id="414c5-133">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="414c5-134">Значение по умолчанию: `any`.</span><span class="sxs-lookup"><span data-stu-id="414c5-134">Default value is `any`.</span></span> <span data-ttu-id="414c5-135">Этот атрибут не оказывает никакого действия, если `type` свойство имеет значение `person` .</span><span class="sxs-lookup"><span data-stu-id="414c5-135">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="414c5-136">Выбранные пользователи</span><span class="sxs-lookup"><span data-stu-id="414c5-136">selected-people</span></span>  | <span data-ttu-id="414c5-137">селектедпеопле</span><span class="sxs-lookup"><span data-stu-id="414c5-137">selectedPeople</span></span>     | <span data-ttu-id="414c5-138">Массив выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="414c5-138">An array of selected people.</span></span> <span data-ttu-id="414c5-139">Задайте это значение для программного выбора людей.</span><span class="sxs-lookup"><span data-stu-id="414c5-139">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="414c5-140">people</span><span class="sxs-lookup"><span data-stu-id="414c5-140">people</span></span>   | <span data-ttu-id="414c5-141">people</span><span class="sxs-lookup"><span data-stu-id="414c5-141">people</span></span>    | <span data-ttu-id="414c5-142">Массив людей, найденных и визуализированных в результатах поиска</span><span class="sxs-lookup"><span data-stu-id="414c5-142">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="414c5-143">по умолчанию — выбранные: Users ID</span><span class="sxs-lookup"><span data-stu-id="414c5-143">default-selected-user-ids</span></span> | <span data-ttu-id="414c5-144">дефаултселектедусеридс</span><span class="sxs-lookup"><span data-stu-id="414c5-144">defaultSelectedUserIds</span></span> | <span data-ttu-id="414c5-145">При указании строки с разделителями, разделенными запятыми, компонент отрисовывает соответствующих пользователей, как выбрано при инициализации.</span><span class="sxs-lookup"><span data-stu-id="414c5-145">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>

<span data-ttu-id="414c5-146">Ниже приведен `show-max` пример.</span><span class="sxs-lookup"><span data-stu-id="414c5-146">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="414c5-147">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="414c5-147">Selected people</span></span>

<span data-ttu-id="414c5-148">В разделе выбранные люди компонента отображается каждый пользователь, выбранный разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="414c5-148">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![Центр управления "Выбор людей"](./images/selected-people.png)

<span data-ttu-id="414c5-150">Вы можете заполнить выбранные данные о людях, выполнив одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="414c5-150">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="414c5-151">`selectedPeople`Непосредственное задание свойства, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="414c5-151">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="414c5-152">С помощью `selectUsersById()` метода, который принимает массив [идентификаторов пользователей](/graph/api/resources/users?view=graph-rest-1.0) Microsoft Graph, чтобы найти сведения о пользователе для выбора.</span><span class="sxs-lookup"><span data-stu-id="414c5-152">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="414c5-153">**Примечание:** Если для пользователя не найдено ни одного пользователя `id` , данные не будут отображены `id` .</span><span class="sxs-lookup"><span data-stu-id="414c5-153">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="414c5-154">События</span><span class="sxs-lookup"><span data-stu-id="414c5-154">Events</span></span>

<span data-ttu-id="414c5-155">Из компонента порождаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="414c5-155">The following events are fired from the component.</span></span>

| <span data-ttu-id="414c5-156">Событие</span><span class="sxs-lookup"><span data-stu-id="414c5-156">Event</span></span> | <span data-ttu-id="414c5-157">Описание</span><span class="sxs-lookup"><span data-stu-id="414c5-157">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="414c5-158">Пользователь добавил или удалил пользователя из списка выбранных/выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="414c5-158">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="414c5-159">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="414c5-159">CSS custom properties</span></span>

<span data-ttu-id="414c5-160">`mgt-people-picker`Компонент определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="414c5-160">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="414c5-161">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="414c5-161">Templates</span></span>

 <span data-ttu-id="414c5-162">`mgt-people-picker` поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="414c5-162">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="414c5-163">Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="414c5-163">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="414c5-164">Тип данных</span><span class="sxs-lookup"><span data-stu-id="414c5-164">Data type</span></span> | <span data-ttu-id="414c5-165">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="414c5-165">Data context</span></span> | <span data-ttu-id="414c5-166">Описание</span><span class="sxs-lookup"><span data-stu-id="414c5-166">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="414c5-167">Значение  по умолчанию</span><span class="sxs-lookup"><span data-stu-id="414c5-167">default</span></span> | <span data-ttu-id="414c5-168">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="414c5-168">null: no data</span></span> | <span data-ttu-id="414c5-169">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="414c5-169">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="414c5-170">загрузки</span><span class="sxs-lookup"><span data-stu-id="414c5-170">loading</span></span> | <span data-ttu-id="414c5-171">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="414c5-171">null: no data</span></span> | <span data-ttu-id="414c5-172">Шаблон, используемый для отображения состояния средства выбора при запросе к Graph.</span><span class="sxs-lookup"><span data-stu-id="414c5-172">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="414c5-173">error</span><span class="sxs-lookup"><span data-stu-id="414c5-173">error</span></span> | <span data-ttu-id="414c5-174">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="414c5-174">null: no data</span></span> | <span data-ttu-id="414c5-175">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="414c5-175">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="414c5-176">нет данных</span><span class="sxs-lookup"><span data-stu-id="414c5-176">no-data</span></span> | <span data-ttu-id="414c5-177">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="414c5-177">null: no data</span></span> | <span data-ttu-id="414c5-178">Альтернативный шаблон, используемый в случае, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="414c5-178">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="414c5-179">выбранное лицо</span><span class="sxs-lookup"><span data-stu-id="414c5-179">selected-person</span></span> | <span data-ttu-id="414c5-180">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="414c5-180">person: The person details object</span></span> | <span data-ttu-id="414c5-181">Шаблон для отображения выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="414c5-181">The template to render selected people.</span></span> |
| <span data-ttu-id="414c5-182">которому</span><span class="sxs-lookup"><span data-stu-id="414c5-182">person</span></span> | <span data-ttu-id="414c5-183">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="414c5-183">person: The person details object</span></span> | <span data-ttu-id="414c5-184">Шаблон для отображения людей в раскрывающемся меню.</span><span class="sxs-lookup"><span data-stu-id="414c5-184">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="414c5-185">В приведенных ниже примерах показано, как использовать `error` шаблон.</span><span class="sxs-lookup"><span data-stu-id="414c5-185">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="414c5-186">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="414c5-186">Microsoft Graph permissions</span></span>

<span data-ttu-id="414c5-187">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="414c5-187">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="414c5-188">API</span><span class="sxs-lookup"><span data-stu-id="414c5-188">API</span></span>                                                                                                              | <span data-ttu-id="414c5-189">Разрешение</span><span class="sxs-lookup"><span data-stu-id="414c5-189">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="414c5-190">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="414c5-190">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="414c5-191">People.Read</span><span class="sxs-lookup"><span data-stu-id="414c5-191">People.Read</span></span>        |
| [<span data-ttu-id="414c5-192">/Users</span><span class="sxs-lookup"><span data-stu-id="414c5-192">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0)  | <span data-ttu-id="414c5-193">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="414c5-193">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="414c5-194">/граупс</span><span class="sxs-lookup"><span data-stu-id="414c5-194">/groups</span></span>](/group-list?view=graph-rest-beta)  | <span data-ttu-id="414c5-195">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="414c5-195">Group.Read.All</span></span> |
| [<span data-ttu-id="414c5-196">/граупс/ \$ {groupId}/мемберс</span><span class="sxs-lookup"><span data-stu-id="414c5-196">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="414c5-197">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="414c5-197">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="414c5-198">/Users/$ {УсерпринЦипленаме} </span><span class="sxs-lookup"><span data-stu-id="414c5-198">/users/${userPrincipleName} </span></span>](/graph/api/user-get?view=graph-rest-1.0)  | <span data-ttu-id="414c5-199">User.Read</span><span class="sxs-lookup"><span data-stu-id="414c5-199">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="414c5-200">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="414c5-200">Authentication</span></span>

<span data-ttu-id="414c5-201">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="414c5-201">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="414c5-202">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="414c5-202">Extend for more control</span></span>

<span data-ttu-id="414c5-203">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected render*` способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="414c5-203">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="414c5-204">Метод</span><span class="sxs-lookup"><span data-stu-id="414c5-204">Method</span></span> | <span data-ttu-id="414c5-205">Описание</span><span class="sxs-lookup"><span data-stu-id="414c5-205">Description</span></span> |
| - | - |
| <span data-ttu-id="414c5-206">рендеринпут</span><span class="sxs-lookup"><span data-stu-id="414c5-206">renderInput</span></span> | <span data-ttu-id="414c5-207">Отрисовывает текстовое поле ввода.</span><span class="sxs-lookup"><span data-stu-id="414c5-207">Renders the input text box.</span></span> |
| <span data-ttu-id="414c5-208">рендерселектедпеопле</span><span class="sxs-lookup"><span data-stu-id="414c5-208">renderSelectedPeople</span></span> | <span data-ttu-id="414c5-209">Отрисовывает выбранные маркеры людей.</span><span class="sxs-lookup"><span data-stu-id="414c5-209">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="414c5-210">рендерселектедперсон</span><span class="sxs-lookup"><span data-stu-id="414c5-210">renderSelectedPerson</span></span> | <span data-ttu-id="414c5-211">Отрисовывает маркер отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="414c5-211">Renders an individual person token.</span></span> |
| <span data-ttu-id="414c5-212">рендерфлйоут</span><span class="sxs-lookup"><span data-stu-id="414c5-212">renderFlyout</span></span> | <span data-ttu-id="414c5-213">Отрисовывает всплывающий хром.</span><span class="sxs-lookup"><span data-stu-id="414c5-213">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="414c5-214">рендерфлйоутконтент</span><span class="sxs-lookup"><span data-stu-id="414c5-214">renderFlyoutContent</span></span> | <span data-ttu-id="414c5-215">Отображает соответствующее состояние в всплывающем окне результаты.</span><span class="sxs-lookup"><span data-stu-id="414c5-215">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="414c5-216">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="414c5-216">renderLoading</span></span> | <span data-ttu-id="414c5-217">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="414c5-217">Renders the loading state.</span></span> |
| <span data-ttu-id="414c5-218">рендернодата</span><span class="sxs-lookup"><span data-stu-id="414c5-218">renderNoData</span></span> | <span data-ttu-id="414c5-219">Отображает состояние, если результаты поискового запроса не найдены.</span><span class="sxs-lookup"><span data-stu-id="414c5-219">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="414c5-220">рендерсеарчресултс</span><span class="sxs-lookup"><span data-stu-id="414c5-220">renderSearchResults</span></span> | <span data-ttu-id="414c5-221">Отрисовывает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="414c5-221">Renders the list of search results.</span></span> |
| <span data-ttu-id="414c5-222">рендерперсонресулт</span><span class="sxs-lookup"><span data-stu-id="414c5-222">renderPersonResult</span></span> | <span data-ttu-id="414c5-223">Отображает результат поиска отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="414c5-223">Renders an individual person search result.</span></span> |