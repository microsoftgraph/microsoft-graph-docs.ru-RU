---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: e3e656c6aef0ab2af9878fb3e4738ade912c4685
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681888"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="6af50-103">Компонент "Выбор людей" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6af50-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="6af50-104">Вы можете использовать `mgt-people-picker` веб-компонент для поиска людей и/или групп.</span><span class="sxs-lookup"><span data-stu-id="6af50-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="6af50-105">По умолчанию компонент будет выполнять поиск всех людей и пользователей в Организации, но вы можете изменить поведение, чтобы также выполнить поиск групп или только групп.</span><span class="sxs-lookup"><span data-stu-id="6af50-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="6af50-106">Вы также можете отфильтровать поиск в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="6af50-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="6af50-107">Пример</span><span class="sxs-lookup"><span data-stu-id="6af50-107">Example</span></span>

<span data-ttu-id="6af50-108">В приведенном ниже примере показан `mgt-people-picker` компонент.</span><span class="sxs-lookup"><span data-stu-id="6af50-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="6af50-109">Начните поиск имени, чтобы увидеть результаты, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="6af50-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="6af50-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="6af50-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="6af50-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="6af50-111">Properties</span></span>

<span data-ttu-id="6af50-112">По умолчанию `mgt-people-picker` компонент получает пользователей из `/me/people` `/users` конечных точек и.</span><span class="sxs-lookup"><span data-stu-id="6af50-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="6af50-113">Используйте следующие атрибуты, чтобы изменить это поведение.</span><span class="sxs-lookup"><span data-stu-id="6af50-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="6af50-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="6af50-114">Attribute</span></span> | <span data-ttu-id="6af50-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="6af50-115">Property</span></span> | <span data-ttu-id="6af50-116">Описание</span><span class="sxs-lookup"><span data-stu-id="6af50-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6af50-117">Show — Max</span><span class="sxs-lookup"><span data-stu-id="6af50-117">show-max</span></span> | <span data-ttu-id="6af50-118">шовмакс</span><span class="sxs-lookup"><span data-stu-id="6af50-118">showMax</span></span>   | <span data-ttu-id="6af50-119">Числовое значение, указывающее максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="6af50-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="6af50-120">значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="6af50-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="6af50-121">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="6af50-121">group-id</span></span>    | <span data-ttu-id="6af50-122">groupId</span><span class="sxs-lookup"><span data-stu-id="6af50-122">groupId</span></span>     | <span data-ttu-id="6af50-123">Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="6af50-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="6af50-124">type</span><span class="sxs-lookup"><span data-stu-id="6af50-124">type</span></span>     | <span data-ttu-id="6af50-125">type</span><span class="sxs-lookup"><span data-stu-id="6af50-125">type</span></span>      | <span data-ttu-id="6af50-126">Тип сущностей для поиска.</span><span class="sxs-lookup"><span data-stu-id="6af50-126">The type of entities to search for.</span></span> <span data-ttu-id="6af50-127">Доступные параметры: `person` , `group` , `any` .</span><span class="sxs-lookup"><span data-stu-id="6af50-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="6af50-128">Значение по умолчанию: `person`.</span><span class="sxs-lookup"><span data-stu-id="6af50-128">Default value is `person`.</span></span> <span data-ttu-id="6af50-129">Этот атрибут не оказывает никакого действия `group-id` , если свойство задано.</span><span class="sxs-lookup"><span data-stu-id="6af50-129">This attribute has no effect if `group-id` property is set.</span></span>                                                                            |
| <span data-ttu-id="6af50-130">Тип группы</span><span class="sxs-lookup"><span data-stu-id="6af50-130">group-type</span></span>     | <span data-ttu-id="6af50-131">groupType</span><span class="sxs-lookup"><span data-stu-id="6af50-131">groupType</span></span>      | <span data-ttu-id="6af50-132">Тип группы для поиска.</span><span class="sxs-lookup"><span data-stu-id="6af50-132">The group type to search for.</span></span> <span data-ttu-id="6af50-133">Доступные варианты: `unified` ,, `security` `mailenabledsecurity` , `distribution` , `any` .</span><span class="sxs-lookup"><span data-stu-id="6af50-133">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="6af50-134">Значение по умолчанию: `any`.</span><span class="sxs-lookup"><span data-stu-id="6af50-134">Default value is `any`.</span></span> <span data-ttu-id="6af50-135">Этот атрибут не оказывает никакого действия, если `type` свойство имеет значение `person` .</span><span class="sxs-lookup"><span data-stu-id="6af50-135">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="6af50-136">Выбранные пользователи</span><span class="sxs-lookup"><span data-stu-id="6af50-136">selected-people</span></span>  | <span data-ttu-id="6af50-137">селектедпеопле</span><span class="sxs-lookup"><span data-stu-id="6af50-137">selectedPeople</span></span>     | <span data-ttu-id="6af50-138">Массив выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6af50-138">An array of selected people.</span></span> <span data-ttu-id="6af50-139">Задайте это значение для программного выбора людей.</span><span class="sxs-lookup"><span data-stu-id="6af50-139">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="6af50-140">people</span><span class="sxs-lookup"><span data-stu-id="6af50-140">people</span></span>   | <span data-ttu-id="6af50-141">people</span><span class="sxs-lookup"><span data-stu-id="6af50-141">people</span></span>    | <span data-ttu-id="6af50-142">Массив людей, найденных и визуализированных в результатах поиска</span><span class="sxs-lookup"><span data-stu-id="6af50-142">An array of people found and rendered in the search result</span></span> |

<span data-ttu-id="6af50-143">Ниже приведен `show-max` пример.</span><span class="sxs-lookup"><span data-stu-id="6af50-143">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="6af50-144">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="6af50-144">Selected people</span></span>

<span data-ttu-id="6af50-145">В разделе выбранные люди компонента отображается каждый пользователь, выбранный разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="6af50-145">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![Центр управления "Выбор людей"](./images/selected-people.png)

<span data-ttu-id="6af50-147">Вы можете заполнить выбранные данные о людях, выполнив одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="6af50-147">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="6af50-148">`selectedPeople`Непосредственное задание свойства, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="6af50-148">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="6af50-149">С помощью `selectUsersById()` метода, который принимает массив [идентификаторов пользователей](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) Microsoft Graph, чтобы найти сведения о пользователе для выбора.</span><span class="sxs-lookup"><span data-stu-id="6af50-149">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="6af50-150">**Примечание:** Если для пользователя не найдено ни одного пользователя `id` , данные не будут отображены `id` .</span><span class="sxs-lookup"><span data-stu-id="6af50-150">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="6af50-151">События</span><span class="sxs-lookup"><span data-stu-id="6af50-151">Events</span></span>

<span data-ttu-id="6af50-152">Из компонента порождаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="6af50-152">The following events are fired from the component.</span></span>

| <span data-ttu-id="6af50-153">Событие</span><span class="sxs-lookup"><span data-stu-id="6af50-153">Event</span></span> | <span data-ttu-id="6af50-154">Описание</span><span class="sxs-lookup"><span data-stu-id="6af50-154">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="6af50-155">Пользователь добавил или удалил пользователя из списка выбранных/выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6af50-155">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="6af50-156">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="6af50-156">CSS custom properties</span></span>

<span data-ttu-id="6af50-157">`mgt-people-picker`Компонент определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="6af50-157">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="6af50-158">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="6af50-158">Templates</span></span>

 <span data-ttu-id="6af50-159">`mgt-people-picker`поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="6af50-159">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="6af50-160">Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="6af50-160">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="6af50-161">Тип данных</span><span class="sxs-lookup"><span data-stu-id="6af50-161">Data type</span></span> | <span data-ttu-id="6af50-162">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="6af50-162">Data context</span></span> | <span data-ttu-id="6af50-163">Description</span><span class="sxs-lookup"><span data-stu-id="6af50-163">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="6af50-164">Значение  по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6af50-164">default</span></span> | <span data-ttu-id="6af50-165">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="6af50-165">null: no data</span></span> | <span data-ttu-id="6af50-166">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="6af50-166">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="6af50-167">загрузки</span><span class="sxs-lookup"><span data-stu-id="6af50-167">loading</span></span> | <span data-ttu-id="6af50-168">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="6af50-168">null: no data</span></span> | <span data-ttu-id="6af50-169">Шаблон, используемый для отображения состояния средства выбора при запросе к Graph.</span><span class="sxs-lookup"><span data-stu-id="6af50-169">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="6af50-170">error</span><span class="sxs-lookup"><span data-stu-id="6af50-170">error</span></span> | <span data-ttu-id="6af50-171">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="6af50-171">null: no data</span></span> | <span data-ttu-id="6af50-172">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="6af50-172">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="6af50-173">нет данных</span><span class="sxs-lookup"><span data-stu-id="6af50-173">no-data</span></span> | <span data-ttu-id="6af50-174">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="6af50-174">null: no data</span></span> | <span data-ttu-id="6af50-175">Альтернативный шаблон, используемый в случае, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="6af50-175">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="6af50-176">выбранное лицо</span><span class="sxs-lookup"><span data-stu-id="6af50-176">selected-person</span></span> | <span data-ttu-id="6af50-177">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="6af50-177">person: The person details object</span></span> | <span data-ttu-id="6af50-178">Шаблон для отображения выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6af50-178">The template to render selected people.</span></span> |
| <span data-ttu-id="6af50-179">которому</span><span class="sxs-lookup"><span data-stu-id="6af50-179">person</span></span> | <span data-ttu-id="6af50-180">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="6af50-180">person: The person details object</span></span> | <span data-ttu-id="6af50-181">Шаблон для отображения людей в раскрывающемся меню.</span><span class="sxs-lookup"><span data-stu-id="6af50-181">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="6af50-182">В приведенных ниже примерах показано, как использовать `error` шаблон.</span><span class="sxs-lookup"><span data-stu-id="6af50-182">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="6af50-183">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6af50-183">Microsoft Graph permissions</span></span>

<span data-ttu-id="6af50-184">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6af50-184">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="6af50-185">API</span><span class="sxs-lookup"><span data-stu-id="6af50-185">API</span></span>                                                                                                              | <span data-ttu-id="6af50-186">Permission</span><span class="sxs-lookup"><span data-stu-id="6af50-186">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="6af50-187">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="6af50-187">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="6af50-188">People.Read</span><span class="sxs-lookup"><span data-stu-id="6af50-188">People.Read</span></span>        |
| [<span data-ttu-id="6af50-189">/Users</span><span class="sxs-lookup"><span data-stu-id="6af50-189">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0)  | <span data-ttu-id="6af50-190">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="6af50-190">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="6af50-191">/граупс</span><span class="sxs-lookup"><span data-stu-id="6af50-191">/groups</span></span>](/group-list?view=graph-rest-beta)  | <span data-ttu-id="6af50-192">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6af50-192">Group.Read.All</span></span> |
| [<span data-ttu-id="6af50-193">/граупс/ \$ {groupId}/мемберс</span><span class="sxs-lookup"><span data-stu-id="6af50-193">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="6af50-194">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="6af50-194">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="6af50-195">/Users/$ {УсерпринЦипленаме}</span><span class="sxs-lookup"><span data-stu-id="6af50-195">/users/${userPrincipleName} </span></span>](/graph/api/user-get?view=graph-rest-1.0)  | <span data-ttu-id="6af50-196">User.Read</span><span class="sxs-lookup"><span data-stu-id="6af50-196">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="6af50-197">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="6af50-197">Authentication</span></span>

<span data-ttu-id="6af50-198">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="6af50-198">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="6af50-199">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="6af50-199">Extend for more control</span></span>

<span data-ttu-id="6af50-200">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected render*` способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="6af50-200">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="6af50-201">Метод</span><span class="sxs-lookup"><span data-stu-id="6af50-201">Method</span></span> | <span data-ttu-id="6af50-202">Описание</span><span class="sxs-lookup"><span data-stu-id="6af50-202">Description</span></span> |
| - | - |
| <span data-ttu-id="6af50-203">рендеринпут</span><span class="sxs-lookup"><span data-stu-id="6af50-203">renderInput</span></span> | <span data-ttu-id="6af50-204">Отрисовывает текстовое поле ввода.</span><span class="sxs-lookup"><span data-stu-id="6af50-204">Renders the input text box.</span></span> |
| <span data-ttu-id="6af50-205">рендерселектедпеопле</span><span class="sxs-lookup"><span data-stu-id="6af50-205">renderSelectedPeople</span></span> | <span data-ttu-id="6af50-206">Отрисовывает выбранные маркеры людей.</span><span class="sxs-lookup"><span data-stu-id="6af50-206">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="6af50-207">рендерселектедперсон</span><span class="sxs-lookup"><span data-stu-id="6af50-207">renderSelectedPerson</span></span> | <span data-ttu-id="6af50-208">Отрисовывает маркер отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="6af50-208">Renders an individual person token.</span></span> |
| <span data-ttu-id="6af50-209">рендерфлйоут</span><span class="sxs-lookup"><span data-stu-id="6af50-209">renderFlyout</span></span> | <span data-ttu-id="6af50-210">Отрисовывает всплывающий хром.</span><span class="sxs-lookup"><span data-stu-id="6af50-210">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="6af50-211">рендерфлйоутконтент</span><span class="sxs-lookup"><span data-stu-id="6af50-211">renderFlyoutContent</span></span> | <span data-ttu-id="6af50-212">Отображает соответствующее состояние в всплывающем окне результаты.</span><span class="sxs-lookup"><span data-stu-id="6af50-212">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="6af50-213">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="6af50-213">renderLoading</span></span> | <span data-ttu-id="6af50-214">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="6af50-214">Renders the loading state.</span></span> |
| <span data-ttu-id="6af50-215">рендернодата</span><span class="sxs-lookup"><span data-stu-id="6af50-215">renderNoData</span></span> | <span data-ttu-id="6af50-216">Отображает состояние, если результаты поискового запроса не найдены.</span><span class="sxs-lookup"><span data-stu-id="6af50-216">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="6af50-217">рендерсеарчресултс</span><span class="sxs-lookup"><span data-stu-id="6af50-217">renderSearchResults</span></span> | <span data-ttu-id="6af50-218">Отрисовывает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="6af50-218">Renders the list of search results.</span></span> |
| <span data-ttu-id="6af50-219">рендерперсонресулт</span><span class="sxs-lookup"><span data-stu-id="6af50-219">renderPersonResult</span></span> | <span data-ttu-id="6af50-220">Отображает результат поиска отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="6af50-220">Renders an individual person search result.</span></span> |
