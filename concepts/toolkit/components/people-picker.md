---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 22ad36715dd0405d44214901a0adf90bb717b167
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955890"
---
# <a name="people-picker-component"></a><span data-ttu-id="6722e-103">Компонент "Выбор людей"</span><span class="sxs-lookup"><span data-stu-id="6722e-103">People-Picker component</span></span>

<span data-ttu-id="6722e-104">Вы можете использовать поиск `mgt-people-picker` в веб-компоненте для указанного числа людей и отобразить список результатов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6722e-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="6722e-105">По умолчанию компонент будет выполнять поиск всех пользователей; Кроме того, можно определить свойство Group, чтобы отфильтровать результаты.</span><span class="sxs-lookup"><span data-stu-id="6722e-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="6722e-106">Если количество отображаемых людей превышает `show-max` значение, в списке поиска будут отображаться не все возвращенные пользователи.</span><span class="sxs-lookup"><span data-stu-id="6722e-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="6722e-107">Пример</span><span class="sxs-lookup"><span data-stu-id="6722e-107">Example</span></span>

[<span data-ttu-id="6722e-108">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="6722e-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![Центр управления "Выбор людей"](./images/mgt-people-picker-image.png)

## <a name="properties"></a><span data-ttu-id="6722e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="6722e-110">Properties</span></span>

<span data-ttu-id="6722e-111">По умолчанию `mgt-people-picker` компонент получает события от `/me/people` конечной точки.</span><span class="sxs-lookup"><span data-stu-id="6722e-111">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="6722e-112">Используйте следующие атрибуты, чтобы изменить это поведение.</span><span class="sxs-lookup"><span data-stu-id="6722e-112">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="6722e-113">Атрибут</span><span class="sxs-lookup"><span data-stu-id="6722e-113">Attribute</span></span> | <span data-ttu-id="6722e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="6722e-114">Property</span></span> | <span data-ttu-id="6722e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6722e-115">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6722e-116">Show — Max</span><span class="sxs-lookup"><span data-stu-id="6722e-116">show-max</span></span> | <span data-ttu-id="6722e-117">шовмакс</span><span class="sxs-lookup"><span data-stu-id="6722e-117">showMax</span></span>   | <span data-ttu-id="6722e-118">Числовое значение, указывающее максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="6722e-118">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="6722e-119">значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="6722e-119">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="6722e-120">people</span><span class="sxs-lookup"><span data-stu-id="6722e-120">people</span></span>   | <span data-ttu-id="6722e-121">people</span><span class="sxs-lookup"><span data-stu-id="6722e-121">people</span></span>    | <span data-ttu-id="6722e-122">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="6722e-122">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="6722e-123">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="6722e-123">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="6722e-124">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6722e-124">Set this value to load your own people.</span></span> |
| <span data-ttu-id="6722e-125">group</span><span class="sxs-lookup"><span data-stu-id="6722e-125">group</span></span>    | <span data-ttu-id="6722e-126">group</span><span class="sxs-lookup"><span data-stu-id="6722e-126">group</span></span>     | <span data-ttu-id="6722e-127">Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="6722e-127">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="6722e-128">Выбранные пользователи</span><span class="sxs-lookup"><span data-stu-id="6722e-128">selected-people</span></span>  | <span data-ttu-id="6722e-129">селектедпеопле</span><span class="sxs-lookup"><span data-stu-id="6722e-129">selectedPeople</span></span>     | <span data-ttu-id="6722e-130">Массив типа `person`, представляющий людей, выбранных в компоненте.</span><span class="sxs-lookup"><span data-stu-id="6722e-130">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="6722e-131">Задайте для этого параметра значение выбранные пользователи по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6722e-131">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="6722e-132">Ниже приведен `show-max` пример.</span><span class="sxs-lookup"><span data-stu-id="6722e-132">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="6722e-133">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="6722e-133">Selected people</span></span>

<span data-ttu-id="6722e-134">В разделе выбранные люди компонента отображается каждый пользователь, выбранный разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="6722e-134">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![Центр управления "Выбор людей"](./images/selected-people.png)

<span data-ttu-id="6722e-136">Вы можете заполнить выбранные данные о людях, выполнив одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="6722e-136">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="6722e-137">Непосредственное `selectedPeople` задание свойства, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="6722e-137">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="6722e-138">С помощью `selectUsersById()` метода, который принимает массив [идентификаторов пользователей](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) Microsoft Graph, чтобы найти сведения о пользователе для выбора.</span><span class="sxs-lookup"><span data-stu-id="6722e-138">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="6722e-139">**Примечание:** Если для пользователя не найдено ни одного `id`пользователя, данные не будут отображены `id`.</span><span class="sxs-lookup"><span data-stu-id="6722e-139">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="6722e-140">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="6722e-140">CSS custom properties</span></span>

<span data-ttu-id="6722e-141">`mgt-people-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="6722e-141">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="6722e-142">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="6722e-142">Templates</span></span>

 <span data-ttu-id="6722e-143">`mgt-people-picker`поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="6722e-143">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="6722e-144">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="6722e-144">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="6722e-145">Тип данных</span><span class="sxs-lookup"><span data-stu-id="6722e-145">Data type</span></span> | <span data-ttu-id="6722e-146">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="6722e-146">Data context</span></span> | <span data-ttu-id="6722e-147">Описание</span><span class="sxs-lookup"><span data-stu-id="6722e-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="6722e-148">загрузки</span><span class="sxs-lookup"><span data-stu-id="6722e-148">loading</span></span> | <span data-ttu-id="6722e-149">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="6722e-149">null: no data</span></span> | <span data-ttu-id="6722e-150">Шаблон, используемый для отображения состояния средства выбора при запросе к Graph.</span><span class="sxs-lookup"><span data-stu-id="6722e-150">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="6722e-151">error</span><span class="sxs-lookup"><span data-stu-id="6722e-151">error</span></span> | <span data-ttu-id="6722e-152">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="6722e-152">null: no data</span></span>| <span data-ttu-id="6722e-153">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="6722e-153">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="6722e-154">выбранное лицо</span><span class="sxs-lookup"><span data-stu-id="6722e-154">selected-person</span></span> |<span data-ttu-id="6722e-155">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="6722e-155">person: The person details object</span></span>| <span data-ttu-id="6722e-156">Шаблон для отображения выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6722e-156">The template to render selected people.</span></span> |
| <span data-ttu-id="6722e-157">person</span><span class="sxs-lookup"><span data-stu-id="6722e-157">person</span></span> | <span data-ttu-id="6722e-158">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="6722e-158">person: The person details object</span></span>| <span data-ttu-id="6722e-159">Шаблон для отображения людей в раскрывающемся меню.</span><span class="sxs-lookup"><span data-stu-id="6722e-159">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="6722e-160">В приведенных ниже примерах показано, `error` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="6722e-160">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="6722e-161">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6722e-161">Microsoft Graph permissions</span></span>

<span data-ttu-id="6722e-162">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6722e-162">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="6722e-163">API</span><span class="sxs-lookup"><span data-stu-id="6722e-163">API</span></span>                                                                                                              | <span data-ttu-id="6722e-164">Разрешение</span><span class="sxs-lookup"><span data-stu-id="6722e-164">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="6722e-165">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="6722e-165">/me/people</span></span>](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="6722e-166">People.Read</span><span class="sxs-lookup"><span data-stu-id="6722e-166">People.Read</span></span> |
| [<span data-ttu-id="6722e-167">/граупс/\${groupId}/мемберс</span><span class="sxs-lookup"><span data-stu-id="6722e-167">/groups/\${groupId}/members</span></span>](https://docs.microsoft.com/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="6722e-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="6722e-168">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="6722e-169">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="6722e-169">Authentication</span></span>

<span data-ttu-id="6722e-170">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="6722e-170">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
