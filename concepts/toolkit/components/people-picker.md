---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: bdfb4951151876d79dede974654747d25a54c833
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510884"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f7978-103">Компонент "Выбор людей" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f7978-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f7978-104">Вы можете использовать поиск `mgt-people-picker` в веб-компоненте для указанного числа людей и отобразить список результатов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7978-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="f7978-105">По умолчанию компонент будет выполнять поиск всех пользователей; Кроме того, можно определить свойство Group, чтобы отфильтровать результаты.</span><span class="sxs-lookup"><span data-stu-id="f7978-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="f7978-106">Если количество отображаемых людей превышает `show-max` значение, в списке поиска будут отображаться не все возвращенные пользователи.</span><span class="sxs-lookup"><span data-stu-id="f7978-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="f7978-107">Пример</span><span class="sxs-lookup"><span data-stu-id="f7978-107">Example</span></span>

<span data-ttu-id="f7978-108">В приведенном ниже примере `mgt-people-picker` показан компонент.</span><span class="sxs-lookup"><span data-stu-id="f7978-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="f7978-109">Начните поиск имени, чтобы увидеть результаты, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="f7978-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="f7978-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="f7978-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="f7978-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7978-111">Properties</span></span>

<span data-ttu-id="f7978-112">По умолчанию `mgt-people-picker` компонент получает пользователей от `/me/people` конечной точки.</span><span class="sxs-lookup"><span data-stu-id="f7978-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` endpoint.</span></span> <span data-ttu-id="f7978-113">Используйте следующие атрибуты, чтобы изменить это поведение.</span><span class="sxs-lookup"><span data-stu-id="f7978-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="f7978-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="f7978-114">Attribute</span></span> | <span data-ttu-id="f7978-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7978-115">Property</span></span> | <span data-ttu-id="f7978-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f7978-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f7978-117">Show — Max</span><span class="sxs-lookup"><span data-stu-id="f7978-117">show-max</span></span> | <span data-ttu-id="f7978-118">шовмакс</span><span class="sxs-lookup"><span data-stu-id="f7978-118">showMax</span></span>   | <span data-ttu-id="f7978-119">Числовое значение, указывающее максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="f7978-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="f7978-120">значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="f7978-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="f7978-121">people</span><span class="sxs-lookup"><span data-stu-id="f7978-121">people</span></span>   | <span data-ttu-id="f7978-122">people</span><span class="sxs-lookup"><span data-stu-id="f7978-122">people</span></span>    | <span data-ttu-id="f7978-123">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="f7978-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="f7978-124">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="f7978-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="f7978-125">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7978-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="f7978-126">group</span><span class="sxs-lookup"><span data-stu-id="f7978-126">group</span></span>    | <span data-ttu-id="f7978-127">group</span><span class="sxs-lookup"><span data-stu-id="f7978-127">group</span></span>     | <span data-ttu-id="f7978-128">Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="f7978-128">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="f7978-129">Выбранные пользователи</span><span class="sxs-lookup"><span data-stu-id="f7978-129">selected-people</span></span>  | <span data-ttu-id="f7978-130">селектедпеопле</span><span class="sxs-lookup"><span data-stu-id="f7978-130">selectedPeople</span></span>     | <span data-ttu-id="f7978-131">Массив типа `person`, представляющий людей, выбранных в компоненте.</span><span class="sxs-lookup"><span data-stu-id="f7978-131">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="f7978-132">Задайте для этого параметра значение выбранные пользователи по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7978-132">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="f7978-133">Ниже приведен `show-max` пример.</span><span class="sxs-lookup"><span data-stu-id="f7978-133">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="f7978-134">Выбранные люди</span><span class="sxs-lookup"><span data-stu-id="f7978-134">Selected people</span></span>

<span data-ttu-id="f7978-135">В разделе выбранные люди компонента отображается каждый пользователь, выбранный разработчиком или пользователем.</span><span class="sxs-lookup"><span data-stu-id="f7978-135">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![Центр управления "Выбор людей"](./images/selected-people.png)

<span data-ttu-id="f7978-137">Вы можете заполнить выбранные данные о людях, выполнив одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="f7978-137">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="f7978-138">Непосредственное `selectedPeople` задание свойства, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="f7978-138">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="f7978-139">С помощью `selectUsersById()` метода, который принимает массив [идентификаторов пользователей](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) Microsoft Graph, чтобы найти сведения о пользователе для выбора.</span><span class="sxs-lookup"><span data-stu-id="f7978-139">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="f7978-140">**Примечание:** Если для пользователя не найдено ни одного `id`пользователя, данные не будут отображены `id`.</span><span class="sxs-lookup"><span data-stu-id="f7978-140">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="f7978-141">События</span><span class="sxs-lookup"><span data-stu-id="f7978-141">Events</span></span>

<span data-ttu-id="f7978-142">Из компонента порождаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="f7978-142">The following events are fired from the component.</span></span>

| <span data-ttu-id="f7978-143">Событие</span><span class="sxs-lookup"><span data-stu-id="f7978-143">Event</span></span> | <span data-ttu-id="f7978-144">Описание</span><span class="sxs-lookup"><span data-stu-id="f7978-144">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="f7978-145">Пользователь добавил или удалил пользователя из списка выбранных/выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7978-145">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="f7978-146">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="f7978-146">CSS custom properties</span></span>

<span data-ttu-id="f7978-147">`mgt-people-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="f7978-147">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="f7978-148">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="f7978-148">Templates</span></span>

 <span data-ttu-id="f7978-149">`mgt-people-picker`поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="f7978-149">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="f7978-150">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="f7978-150">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f7978-151">Тип данных</span><span class="sxs-lookup"><span data-stu-id="f7978-151">Data type</span></span> | <span data-ttu-id="f7978-152">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="f7978-152">Data context</span></span> | <span data-ttu-id="f7978-153">Описание</span><span class="sxs-lookup"><span data-stu-id="f7978-153">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f7978-154">Значение  по умолчанию</span><span class="sxs-lookup"><span data-stu-id="f7978-154">default</span></span> | <span data-ttu-id="f7978-155">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="f7978-155">null: no data</span></span> | <span data-ttu-id="f7978-156">Шаблон, используемый для переопределения отображения всего компонента.</span><span class="sxs-lookup"><span data-stu-id="f7978-156">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="f7978-157">загрузки</span><span class="sxs-lookup"><span data-stu-id="f7978-157">loading</span></span> | <span data-ttu-id="f7978-158">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="f7978-158">null: no data</span></span> | <span data-ttu-id="f7978-159">Шаблон, используемый для отображения состояния средства выбора при запросе к Graph.</span><span class="sxs-lookup"><span data-stu-id="f7978-159">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="f7978-160">error</span><span class="sxs-lookup"><span data-stu-id="f7978-160">error</span></span> | <span data-ttu-id="f7978-161">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="f7978-161">null: no data</span></span> | <span data-ttu-id="f7978-162">Шаблон, используемый, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7978-162">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="f7978-163">нет данных</span><span class="sxs-lookup"><span data-stu-id="f7978-163">no-data</span></span> | <span data-ttu-id="f7978-164">NULL: нет данных</span><span class="sxs-lookup"><span data-stu-id="f7978-164">null: no data</span></span> | <span data-ttu-id="f7978-165">Альтернативный шаблон, используемый в случае, если поиск пользователей не возвращает пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7978-165">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="f7978-166">выбранное лицо</span><span class="sxs-lookup"><span data-stu-id="f7978-166">selected-person</span></span> | <span data-ttu-id="f7978-167">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="f7978-167">person: The person details object</span></span> | <span data-ttu-id="f7978-168">Шаблон для отображения выбранных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7978-168">The template to render selected people.</span></span> |
| <span data-ttu-id="f7978-169">которому</span><span class="sxs-lookup"><span data-stu-id="f7978-169">person</span></span> | <span data-ttu-id="f7978-170">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="f7978-170">person: The person details object</span></span> | <span data-ttu-id="f7978-171">Шаблон для отображения людей в раскрывающемся меню.</span><span class="sxs-lookup"><span data-stu-id="f7978-171">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="f7978-172">В приведенных ниже примерах показано, `error` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="f7978-172">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f7978-173">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f7978-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="f7978-174">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7978-174">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="f7978-175">API</span><span class="sxs-lookup"><span data-stu-id="f7978-175">API</span></span>                                                                                                              | <span data-ttu-id="f7978-176">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f7978-176">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="f7978-177">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="f7978-177">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="f7978-178">People.Read</span><span class="sxs-lookup"><span data-stu-id="f7978-178">People.Read</span></span>        |
| [<span data-ttu-id="f7978-179">/граупс/\${groupId}/мемберс</span><span class="sxs-lookup"><span data-stu-id="f7978-179">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="f7978-180">People.Read</span><span class="sxs-lookup"><span data-stu-id="f7978-180">People.Read</span></span>        |
| [<span data-ttu-id="f7978-181">/Users/$ {УсерпринЦипленаме}</span><span class="sxs-lookup"><span data-stu-id="f7978-181">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="f7978-182">User. Readbasic. ALL</span><span class="sxs-lookup"><span data-stu-id="f7978-182">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="f7978-183">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="f7978-183">Authentication</span></span>

<span data-ttu-id="f7978-184">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="f7978-184">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="f7978-185">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="f7978-185">Extend for more control</span></span>

<span data-ttu-id="f7978-186">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="f7978-186">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="f7978-187">Метод</span><span class="sxs-lookup"><span data-stu-id="f7978-187">Method</span></span> | <span data-ttu-id="f7978-188">Описание</span><span class="sxs-lookup"><span data-stu-id="f7978-188">Description</span></span> |
| - | - |
| <span data-ttu-id="f7978-189">рендеринпут</span><span class="sxs-lookup"><span data-stu-id="f7978-189">renderInput</span></span> | <span data-ttu-id="f7978-190">Отрисовывает текстовое поле ввода.</span><span class="sxs-lookup"><span data-stu-id="f7978-190">Renders the input text box.</span></span> |
| <span data-ttu-id="f7978-191">рендерселектедпеопле</span><span class="sxs-lookup"><span data-stu-id="f7978-191">renderSelectedPeople</span></span> | <span data-ttu-id="f7978-192">Отрисовывает выбранные маркеры людей.</span><span class="sxs-lookup"><span data-stu-id="f7978-192">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="f7978-193">рендерселектедперсон</span><span class="sxs-lookup"><span data-stu-id="f7978-193">renderSelectedPerson</span></span> | <span data-ttu-id="f7978-194">Отрисовывает маркер отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="f7978-194">Renders an individual person token.</span></span> |
| <span data-ttu-id="f7978-195">рендерфлйоут</span><span class="sxs-lookup"><span data-stu-id="f7978-195">renderFlyout</span></span> | <span data-ttu-id="f7978-196">Отрисовывает всплывающий хром.</span><span class="sxs-lookup"><span data-stu-id="f7978-196">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="f7978-197">рендерфлйоутконтент</span><span class="sxs-lookup"><span data-stu-id="f7978-197">renderFlyoutContent</span></span> | <span data-ttu-id="f7978-198">Отображает соответствующее состояние в всплывающем окне результаты.</span><span class="sxs-lookup"><span data-stu-id="f7978-198">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="f7978-199">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="f7978-199">renderLoading</span></span> | <span data-ttu-id="f7978-200">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="f7978-200">Renders the loading state.</span></span> |
| <span data-ttu-id="f7978-201">рендернодата</span><span class="sxs-lookup"><span data-stu-id="f7978-201">renderNoData</span></span> | <span data-ttu-id="f7978-202">Отображает состояние, если результаты поискового запроса не найдены.</span><span class="sxs-lookup"><span data-stu-id="f7978-202">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="f7978-203">рендерсеарчресултс</span><span class="sxs-lookup"><span data-stu-id="f7978-203">renderSearchResults</span></span> | <span data-ttu-id="f7978-204">Отрисовывает список результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="f7978-204">Renders the list of search results.</span></span> |
| <span data-ttu-id="f7978-205">рендерперсонресулт</span><span class="sxs-lookup"><span data-stu-id="f7978-205">renderPersonResult</span></span> | <span data-ttu-id="f7978-206">Отображает результат поиска отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="f7978-206">Renders an individual person search result.</span></span> |
