---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 175370b3c00ebaef0db85912c032898e2dacb5e7
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144305"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0ce11-103">Компонент "Выбор людей" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0ce11-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0ce11-104">Вы можете использовать поиск `mgt-people-picker` в веб-компоненте для указанного числа людей и отобразить список результатов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0ce11-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="0ce11-105">По умолчанию компонент будет выполнять поиск всех пользователей; Кроме того, можно определить свойство Group, чтобы отфильтровать результаты.</span><span class="sxs-lookup"><span data-stu-id="0ce11-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="0ce11-106">Если количество отображаемых людей превышает `show-max` значение, в списке поиска будут отображаться не все возвращенные пользователи.</span><span class="sxs-lookup"><span data-stu-id="0ce11-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="0ce11-107">Пример</span><span class="sxs-lookup"><span data-stu-id="0ce11-107">Example</span></span>

<span data-ttu-id="0ce11-108">В приведенном ниже примере `mgt-people-picker` показан компонент.</span><span class="sxs-lookup"><span data-stu-id="0ce11-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="0ce11-109">Начните поиск имени, чтобы увидеть результаты, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="0ce11-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="0ce11-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="0ce11-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="0ce11-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ce11-111">Properties</span></span>

<span data-ttu-id="0ce11-112">По умолчанию `mgt-people-picker` компонент получает события от `/me/people` конечной точки.</span><span class="sxs-lookup"><span data-stu-id="0ce11-112">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="0ce11-113">Используйте следующие атрибуты, чтобы изменить это поведение.</span><span class="sxs-lookup"><span data-stu-id="0ce11-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="0ce11-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="0ce11-114">Attribute</span></span> | <span data-ttu-id="0ce11-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ce11-115">Property</span></span> | <span data-ttu-id="0ce11-116">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce11-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0ce11-117">Show — Max</span><span class="sxs-lookup"><span data-stu-id="0ce11-117">show-max</span></span> | <span data-ttu-id="0ce11-118">шовмакс</span><span class="sxs-lookup"><span data-stu-id="0ce11-118">showMax</span></span>   | <span data-ttu-id="0ce11-119">Числовое значение, указывающее максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="0ce11-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="0ce11-120">значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="0ce11-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="0ce11-121">people</span><span class="sxs-lookup"><span data-stu-id="0ce11-121">people</span></span>   | <span data-ttu-id="0ce11-122">people</span><span class="sxs-lookup"><span data-stu-id="0ce11-122">people</span></span>    | <span data-ttu-id="0ce11-123">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="0ce11-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="0ce11-124">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="0ce11-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="0ce11-125">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="0ce11-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="0ce11-126">group</span><span class="sxs-lookup"><span data-stu-id="0ce11-126">group</span></span>    | <span data-ttu-id="0ce11-127">group</span><span class="sxs-lookup"><span data-stu-id="0ce11-127">group</span></span>     | <span data-ttu-id="0ce11-128">Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="0ce11-128">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="0ce11-129">Выбранные пользователи</span><span class="sxs-lookup"><span data-stu-id="0ce11-129">selected-people</span></span>  | <span data-ttu-id="0ce11-130">селектедпеопле</span><span class="sxs-lookup"><span data-stu-id="0ce11-130">selectedPeople</span></span>     | <span data-ttu-id="0ce11-131">Массив типа `person`, представляющий людей, выбранных в компоненте.</span><span class="sxs-lookup"><span data-stu-id="0ce11-131">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="0ce11-132">Задайте для этого параметра значение выбранные пользователи по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0ce11-132">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="0ce11-133">Ниже приведен `show-max` пример.</span><span class="sxs-lookup"><span data-stu-id="0ce11-133">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="0ce11-134">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="0ce11-134">Selected people</span></span>

<span data-ttu-id="0ce11-135">В разделе выбранные люди компонента отображается каждый пользователь, выбранный разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="0ce11-135">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![Центр управления "Выбор людей"](./images/selected-people.png)

<span data-ttu-id="0ce11-137">Вы можете заполнить выбранные данные о людях, выполнив одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="0ce11-137">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="0ce11-138">Непосредственное `selectedPeople` задание свойства, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="0ce11-138">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="0ce11-139">С помощью `selectUsersById()` метода, который принимает массив [идентификаторов пользователей](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) Microsoft Graph, чтобы найти сведения о пользователе для выбора.</span><span class="sxs-lookup"><span data-stu-id="0ce11-139">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="0ce11-140">**Примечание:** Если для пользователя не найдено ни одного `id`пользователя, данные не будут отображены `id`.</span><span class="sxs-lookup"><span data-stu-id="0ce11-140">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a><span data-ttu-id="0ce11-141">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="0ce11-141">CSS custom properties</span></span>

<span data-ttu-id="0ce11-142">`mgt-people-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="0ce11-142">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="0ce11-143">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="0ce11-143">Templates</span></span>

 <span data-ttu-id="0ce11-144">`mgt-people-picker`поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="0ce11-144">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="0ce11-145">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="0ce11-145">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="0ce11-146">Тип данных</span><span class="sxs-lookup"><span data-stu-id="0ce11-146">Data type</span></span> | <span data-ttu-id="0ce11-147">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="0ce11-147">Data context</span></span> | <span data-ttu-id="0ce11-148">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce11-148">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="0ce11-149">умолчани</span><span class="sxs-lookup"><span data-stu-id="0ce11-149">default</span></span> | <span data-ttu-id="0ce11-150">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="0ce11-150">null: no data</span></span> | <span data-ttu-id="0ce11-151">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="0ce11-151">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="0ce11-152">загрузки</span><span class="sxs-lookup"><span data-stu-id="0ce11-152">loading</span></span> | <span data-ttu-id="0ce11-153">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="0ce11-153">null: no data</span></span> | <span data-ttu-id="0ce11-154">Шаблон, используемый для отображения состояния средства выбора при запросе к Graph.</span><span class="sxs-lookup"><span data-stu-id="0ce11-154">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="0ce11-155">error</span><span class="sxs-lookup"><span data-stu-id="0ce11-155">error</span></span> | <span data-ttu-id="0ce11-156">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="0ce11-156">null: no data</span></span> | <span data-ttu-id="0ce11-157">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="0ce11-157">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="0ce11-158">нет данных</span><span class="sxs-lookup"><span data-stu-id="0ce11-158">no-data</span></span> | <span data-ttu-id="0ce11-159">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="0ce11-159">null: no data</span></span> | <span data-ttu-id="0ce11-160">Альтернативный шаблон, используемый в случае, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="0ce11-160">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="0ce11-161">выбранное лицо</span><span class="sxs-lookup"><span data-stu-id="0ce11-161">selected-person</span></span> | <span data-ttu-id="0ce11-162">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="0ce11-162">person: The person details object</span></span> | <span data-ttu-id="0ce11-163">Шаблон для отображения выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="0ce11-163">The template to render selected people.</span></span> |
| <span data-ttu-id="0ce11-164">person</span><span class="sxs-lookup"><span data-stu-id="0ce11-164">person</span></span> | <span data-ttu-id="0ce11-165">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="0ce11-165">person: The person details object</span></span> | <span data-ttu-id="0ce11-166">Шаблон для отображения людей в раскрывающемся меню.</span><span class="sxs-lookup"><span data-stu-id="0ce11-166">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="0ce11-167">В приведенных ниже примерах показано, `error` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="0ce11-167">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="0ce11-168">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0ce11-168">Microsoft Graph permissions</span></span>

<span data-ttu-id="0ce11-169">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0ce11-169">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="0ce11-170">API</span><span class="sxs-lookup"><span data-stu-id="0ce11-170">API</span></span>                                                                                                              | <span data-ttu-id="0ce11-171">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0ce11-171">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="0ce11-172">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="0ce11-172">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="0ce11-173">People.Read</span><span class="sxs-lookup"><span data-stu-id="0ce11-173">People.Read</span></span>        |
| [<span data-ttu-id="0ce11-174">/граупс/\${groupId}/мемберс</span><span class="sxs-lookup"><span data-stu-id="0ce11-174">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="0ce11-175">People.Read</span><span class="sxs-lookup"><span data-stu-id="0ce11-175">People.Read</span></span>        |
| [<span data-ttu-id="0ce11-176">/Users/$ {УсерпринЦипленаме}</span><span class="sxs-lookup"><span data-stu-id="0ce11-176">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="0ce11-177">User. Readbasic. ALL</span><span class="sxs-lookup"><span data-stu-id="0ce11-177">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="0ce11-178">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="0ce11-178">Authentication</span></span>

<span data-ttu-id="0ce11-179">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="0ce11-179">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="0ce11-180">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="0ce11-180">Extend for more control</span></span>

<span data-ttu-id="0ce11-181">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="0ce11-181">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="0ce11-182">Метод</span><span class="sxs-lookup"><span data-stu-id="0ce11-182">Method</span></span> | <span data-ttu-id="0ce11-183">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce11-183">Description</span></span> |
| - | - |
| <span data-ttu-id="0ce11-184">рендеринпут</span><span class="sxs-lookup"><span data-stu-id="0ce11-184">renderInput</span></span> | <span data-ttu-id="0ce11-185">Отрисовывает текстовое поле ввода.</span><span class="sxs-lookup"><span data-stu-id="0ce11-185">Renders the input text box.</span></span> |
| <span data-ttu-id="0ce11-186">рендерселектедпеопле</span><span class="sxs-lookup"><span data-stu-id="0ce11-186">renderSelectedPeople</span></span> | <span data-ttu-id="0ce11-187">Отрисовывает выбранные маркеры людей.</span><span class="sxs-lookup"><span data-stu-id="0ce11-187">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="0ce11-188">рендерселектедперсон</span><span class="sxs-lookup"><span data-stu-id="0ce11-188">renderSelectedPerson</span></span> | <span data-ttu-id="0ce11-189">Отрисовывает маркер отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="0ce11-189">Renders an individual person token.</span></span> |
| <span data-ttu-id="0ce11-190">рендерфлйоут</span><span class="sxs-lookup"><span data-stu-id="0ce11-190">renderFlyout</span></span> | <span data-ttu-id="0ce11-191">Отрисовывает всплывающий хром.</span><span class="sxs-lookup"><span data-stu-id="0ce11-191">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="0ce11-192">рендерфлйоутконтент</span><span class="sxs-lookup"><span data-stu-id="0ce11-192">renderFlyoutContent</span></span> | <span data-ttu-id="0ce11-193">Отображает соответствующее состояние в всплывающем окне результаты.</span><span class="sxs-lookup"><span data-stu-id="0ce11-193">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="0ce11-194">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="0ce11-194">renderLoading</span></span> | <span data-ttu-id="0ce11-195">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="0ce11-195">Renders the loading state.</span></span> |
| <span data-ttu-id="0ce11-196">рендернодата</span><span class="sxs-lookup"><span data-stu-id="0ce11-196">renderNoData</span></span> | <span data-ttu-id="0ce11-197">Отображает состояние, если результаты поискового запроса не найдены.</span><span class="sxs-lookup"><span data-stu-id="0ce11-197">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="0ce11-198">рендерсеарчресултс</span><span class="sxs-lookup"><span data-stu-id="0ce11-198">renderSearchResults</span></span> | <span data-ttu-id="0ce11-199">Отрисовывает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="0ce11-199">Renders the list of search results.</span></span> |
| <span data-ttu-id="0ce11-200">рендерперсонресулт</span><span class="sxs-lookup"><span data-stu-id="0ce11-200">renderPersonResult</span></span> | <span data-ttu-id="0ce11-201">Отображает результат поиска отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="0ce11-201">Renders an individual person search result.</span></span> |
