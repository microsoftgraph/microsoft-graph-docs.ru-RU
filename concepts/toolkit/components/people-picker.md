---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 91b11006df02d563902b99c79c4b1ec09bb7e50a
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639942"
---
# <a name="people-picker-component"></a><span data-ttu-id="f7218-103">Компонент "Выбор людей"</span><span class="sxs-lookup"><span data-stu-id="f7218-103">People-Picker component</span></span>

<span data-ttu-id="f7218-104">Вы можете использовать поиск `mgt-people-picker` в веб-компоненте для указанного числа людей и отобразить список результатов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7218-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="f7218-105">По умолчанию компонент будет выполнять поиск всех пользователей; Кроме того, можно определить свойство Group, чтобы отфильтровать результаты.</span><span class="sxs-lookup"><span data-stu-id="f7218-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="f7218-106">Если количество отображаемых людей превышает `show-max` значение, в списке поиска будут отображаться не все возвращенные пользователи.</span><span class="sxs-lookup"><span data-stu-id="f7218-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="f7218-107">Пример</span><span class="sxs-lookup"><span data-stu-id="f7218-107">Example</span></span>

<span data-ttu-id="f7218-108">В приведенном ниже примере `mgt-people-picker` показан компонент.</span><span class="sxs-lookup"><span data-stu-id="f7218-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="f7218-109">Начните поиск имени, чтобы увидеть результаты, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="f7218-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="f7218-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="f7218-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="f7218-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7218-111">Properties</span></span>

<span data-ttu-id="f7218-112">По умолчанию `mgt-people-picker` компонент получает события от `/me/people` конечной точки.</span><span class="sxs-lookup"><span data-stu-id="f7218-112">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="f7218-113">Используйте следующие атрибуты, чтобы изменить это поведение.</span><span class="sxs-lookup"><span data-stu-id="f7218-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="f7218-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="f7218-114">Attribute</span></span> | <span data-ttu-id="f7218-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7218-115">Property</span></span> | <span data-ttu-id="f7218-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f7218-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f7218-117">Show — Max</span><span class="sxs-lookup"><span data-stu-id="f7218-117">show-max</span></span> | <span data-ttu-id="f7218-118">шовмакс</span><span class="sxs-lookup"><span data-stu-id="f7218-118">showMax</span></span>   | <span data-ttu-id="f7218-119">Числовое значение, указывающее максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="f7218-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="f7218-120">значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="f7218-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="f7218-121">people</span><span class="sxs-lookup"><span data-stu-id="f7218-121">people</span></span>   | <span data-ttu-id="f7218-122">people</span><span class="sxs-lookup"><span data-stu-id="f7218-122">people</span></span>    | <span data-ttu-id="f7218-123">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="f7218-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="f7218-124">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="f7218-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="f7218-125">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7218-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="f7218-126">group</span><span class="sxs-lookup"><span data-stu-id="f7218-126">group</span></span>    | <span data-ttu-id="f7218-127">group</span><span class="sxs-lookup"><span data-stu-id="f7218-127">group</span></span>     | <span data-ttu-id="f7218-128">Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="f7218-128">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="f7218-129">Выбранные пользователи</span><span class="sxs-lookup"><span data-stu-id="f7218-129">selected-people</span></span>  | <span data-ttu-id="f7218-130">селектедпеопле</span><span class="sxs-lookup"><span data-stu-id="f7218-130">selectedPeople</span></span>     | <span data-ttu-id="f7218-131">Массив типа `person`, представляющий людей, выбранных в компоненте.</span><span class="sxs-lookup"><span data-stu-id="f7218-131">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="f7218-132">Задайте для этого параметра значение выбранные пользователи по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7218-132">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="f7218-133">Ниже приведен `show-max` пример.</span><span class="sxs-lookup"><span data-stu-id="f7218-133">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="f7218-134">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="f7218-134">Selected people</span></span>

<span data-ttu-id="f7218-135">В разделе выбранные люди компонента отображается каждый пользователь, выбранный разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="f7218-135">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![Центр управления "Выбор людей"](./images/selected-people.png)

<span data-ttu-id="f7218-137">Вы можете заполнить выбранные данные о людях, выполнив одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="f7218-137">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="f7218-138">Непосредственное `selectedPeople` задание свойства, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="f7218-138">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="f7218-139">С помощью `selectUsersById()` метода, который принимает массив [идентификаторов пользователей](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) Microsoft Graph, чтобы найти сведения о пользователе для выбора.</span><span class="sxs-lookup"><span data-stu-id="f7218-139">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="f7218-140">**Примечание:** Если для пользователя не найдено ни одного `id`пользователя, данные не будут отображены `id`.</span><span class="sxs-lookup"><span data-stu-id="f7218-140">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="f7218-141">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="f7218-141">CSS custom properties</span></span>

<span data-ttu-id="f7218-142">`mgt-people-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="f7218-142">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="f7218-143">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="f7218-143">Templates</span></span>

 <span data-ttu-id="f7218-144">`mgt-people-picker`поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="f7218-144">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="f7218-145">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="f7218-145">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f7218-146">Тип данных</span><span class="sxs-lookup"><span data-stu-id="f7218-146">Data type</span></span> | <span data-ttu-id="f7218-147">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="f7218-147">Data context</span></span> | <span data-ttu-id="f7218-148">Описание</span><span class="sxs-lookup"><span data-stu-id="f7218-148">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f7218-149">загрузки</span><span class="sxs-lookup"><span data-stu-id="f7218-149">loading</span></span> | <span data-ttu-id="f7218-150">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="f7218-150">null: no data</span></span> | <span data-ttu-id="f7218-151">Шаблон, используемый для отображения состояния средства выбора при запросе к Graph.</span><span class="sxs-lookup"><span data-stu-id="f7218-151">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="f7218-152">error</span><span class="sxs-lookup"><span data-stu-id="f7218-152">error</span></span> | <span data-ttu-id="f7218-153">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="f7218-153">null: no data</span></span>| <span data-ttu-id="f7218-154">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7218-154">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="f7218-155">выбранное лицо</span><span class="sxs-lookup"><span data-stu-id="f7218-155">selected-person</span></span> |<span data-ttu-id="f7218-156">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="f7218-156">person: The person details object</span></span>| <span data-ttu-id="f7218-157">Шаблон для отображения выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7218-157">The template to render selected people.</span></span> |
| <span data-ttu-id="f7218-158">которому</span><span class="sxs-lookup"><span data-stu-id="f7218-158">person</span></span> | <span data-ttu-id="f7218-159">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="f7218-159">person: The person details object</span></span>| <span data-ttu-id="f7218-160">Шаблон для отображения людей в раскрывающемся меню.</span><span class="sxs-lookup"><span data-stu-id="f7218-160">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="f7218-161">В приведенных ниже примерах показано, `error` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="f7218-161">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f7218-162">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f7218-162">Microsoft Graph permissions</span></span>

<span data-ttu-id="f7218-163">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7218-163">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="f7218-164">API</span><span class="sxs-lookup"><span data-stu-id="f7218-164">API</span></span>                                                                                                              | <span data-ttu-id="f7218-165">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f7218-165">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="f7218-166">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="f7218-166">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="f7218-167">People.Read</span><span class="sxs-lookup"><span data-stu-id="f7218-167">People.Read</span></span>        |
| [<span data-ttu-id="f7218-168">/граупс/\${groupId}/мемберс</span><span class="sxs-lookup"><span data-stu-id="f7218-168">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="f7218-169">People.Read</span><span class="sxs-lookup"><span data-stu-id="f7218-169">People.Read</span></span>        |
| [<span data-ttu-id="f7218-170">/Users/$ {УсерпринЦипленаме}</span><span class="sxs-lookup"><span data-stu-id="f7218-170">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="f7218-171">User. Readbasic. ALL</span><span class="sxs-lookup"><span data-stu-id="f7218-171">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="f7218-172">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="f7218-172">Authentication</span></span>

<span data-ttu-id="f7218-173">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="f7218-173">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
