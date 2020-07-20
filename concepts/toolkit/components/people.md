---
title: Компонент "люди" в наборе инструментов Microsoft Graph
description: Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8e942ad0cca446dc8bf982249a7593b8299fe22e
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183976"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="953a6-103">Компонент "люди" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="953a6-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="953a6-104">Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="953a6-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="953a6-105">По умолчанию отображаются наиболее часто используемые контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="953a6-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="953a6-106">Этот компонент использует несколько элементов управления " [центр](./person.md) управления", но их можно привязать к набору дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="953a6-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="953a6-107">Если количество людей для отображения больше `show-max` , чем значение, будет добавлено число, указывающее количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="953a6-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="953a6-108">Пример</span><span class="sxs-lookup"><span data-stu-id="953a6-108">Example</span></span>

<span data-ttu-id="953a6-109">В приведенном ниже примере показана группа людей, отображаемая с помощью `mgt-people` компонента.</span><span class="sxs-lookup"><span data-stu-id="953a6-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="953a6-110">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="953a6-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="953a6-111">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="953a6-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="953a6-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="953a6-112">Properties</span></span>

<span data-ttu-id="953a6-113">По умолчанию `mgt-people` компонент получает события от `/me/people` конечной точки с `personType/class eq 'Person'` фильтром для отображения часто обращенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="953a6-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="953a6-114">Для изменения этого поведения можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="953a6-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="953a6-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="953a6-115">Attribute</span></span> | <span data-ttu-id="953a6-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="953a6-116">Property</span></span> | <span data-ttu-id="953a6-117">Описание</span><span class="sxs-lookup"><span data-stu-id="953a6-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="953a6-118">Show — Max</span><span class="sxs-lookup"><span data-stu-id="953a6-118">show-max</span></span> | <span data-ttu-id="953a6-119">шовмакс</span><span class="sxs-lookup"><span data-stu-id="953a6-119">showMax</span></span> | <span data-ttu-id="953a6-120">Указывает максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="953a6-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="953a6-121">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="953a6-121">Default value is 3.</span></span> |
| <span data-ttu-id="953a6-122">people</span><span class="sxs-lookup"><span data-stu-id="953a6-122">people</span></span> | <span data-ttu-id="953a6-123">people</span><span class="sxs-lookup"><span data-stu-id="953a6-123">people</span></span> | <span data-ttu-id="953a6-124">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="953a6-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="953a6-125">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="953a6-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="953a6-126">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="953a6-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="953a6-127">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="953a6-127">group-id</span></span> | <span data-ttu-id="953a6-128">groupId</span><span class="sxs-lookup"><span data-stu-id="953a6-128">groupId</span></span> | <span data-ttu-id="953a6-129">Извлекает пользователей из определенного идентификатора Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="953a6-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="953a6-130">идентификаторы пользователей</span><span class="sxs-lookup"><span data-stu-id="953a6-130">user-ids</span></span> | <span data-ttu-id="953a6-131">userIds</span><span class="sxs-lookup"><span data-stu-id="953a6-131">userIds</span></span> | <span data-ttu-id="953a6-132">При наличии массива пользователей Microsoft Graph `ids` компонент будет отображать этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="953a6-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="953a6-133">люди — запросы</span><span class="sxs-lookup"><span data-stu-id="953a6-133">people-queries</span></span> | <span data-ttu-id="953a6-134">пеоплекуериес</span><span class="sxs-lookup"><span data-stu-id="953a6-134">peopleQueries</span></span> | <span data-ttu-id="953a6-135">При наличии массива запросов Person (Names, UPN, сообщений электронной почты) компонент будет отображать этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="953a6-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="953a6-136">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="953a6-136">person-card</span></span> | <span data-ttu-id="953a6-137">персонкард</span><span class="sxs-lookup"><span data-stu-id="953a6-137">personCard</span></span> | <span data-ttu-id="953a6-138">Перечисление для определения действия пользователя, необходимого для активации всплывающей панели `hover` `click` .</span><span class="sxs-lookup"><span data-stu-id="953a6-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="953a6-139">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="953a6-139">Default value is `none`.</span></span> |
| <span data-ttu-id="953a6-140">Показать — присутствие</span><span class="sxs-lookup"><span data-stu-id="953a6-140">show-presence</span></span> | <span data-ttu-id="953a6-141">шовпресенце</span><span class="sxs-lookup"><span data-stu-id="953a6-141">showPresence</span></span> | <span data-ttu-id="953a6-142">Логическое значение, определяющее, следует ли отображать значок присутствия пользователя на изображении пользователя.</span><span class="sxs-lookup"><span data-stu-id="953a6-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="953a6-143">В приведенном ниже примере задается максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="953a6-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="953a6-144">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="953a6-144">CSS custom properties</span></span>

<span data-ttu-id="953a6-145">`mgt-people`Компонент определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="953a6-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="953a6-146">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="953a6-146">Templates</span></span>

<span data-ttu-id="953a6-147">`mgt-people`Поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="953a6-147">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="953a6-148">Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="953a6-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="953a6-149">Тип данных</span><span class="sxs-lookup"><span data-stu-id="953a6-149">Data type</span></span> | <span data-ttu-id="953a6-150">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="953a6-150">Data context</span></span> | <span data-ttu-id="953a6-151">Описание</span><span class="sxs-lookup"><span data-stu-id="953a6-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="953a6-152">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="953a6-152">`people`: list of person objects</span></span> | <span data-ttu-id="953a6-153">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="953a6-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="953a6-154">`person`: объект Person</span><span class="sxs-lookup"><span data-stu-id="953a6-154">`person`: person object</span></span> | <span data-ttu-id="953a6-155">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="953a6-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="953a6-156">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="953a6-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="953a6-157">`max`: количество показанных пользователей</span><span class="sxs-lookup"><span data-stu-id="953a6-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="953a6-158">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="953a6-158">`extra`: number of extra people</span></span> | <span data-ttu-id="953a6-159">Шаблон, используемый для отображения числа за пределами максимального значения справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="953a6-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="953a6-160">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="953a6-160">No data context is passed</span></span> | <span data-ttu-id="953a6-161">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="953a6-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="953a6-162">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="953a6-162">No data context is passed</span></span> | <span data-ttu-id="953a6-163">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="953a6-163">The template used while the component loads state.</span></span>

<span data-ttu-id="953a6-164">В приведенных ниже примерах показано, как использовать `person` шаблон.</span><span class="sxs-lookup"><span data-stu-id="953a6-164">The following examples shows how to use the `person` template.</span></span>

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="953a6-165">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="953a6-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="953a6-166">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="953a6-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="953a6-167">Ресурс</span><span class="sxs-lookup"><span data-stu-id="953a6-167">Resource</span></span> | <span data-ttu-id="953a6-168">Разрешение</span><span class="sxs-lookup"><span data-stu-id="953a6-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="953a6-169">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="953a6-169">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

<span data-ttu-id="953a6-170">При использовании шаблонов по умолчанию требуются дополнительные API и разрешения.</span><span class="sxs-lookup"><span data-stu-id="953a6-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="953a6-171">В шаблоне по умолчанию для этого компонента используется компонент " [упр. Person](person.md) ", для которого требуется следующее.</span><span class="sxs-lookup"><span data-stu-id="953a6-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="953a6-172">Ресурс</span><span class="sxs-lookup"><span data-stu-id="953a6-172">Resource</span></span> | <span data-ttu-id="953a6-173">Разрешение</span><span class="sxs-lookup"><span data-stu-id="953a6-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="953a6-174">/Users</span><span class="sxs-lookup"><span data-stu-id="953a6-174">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0) | <span data-ttu-id="953a6-175">Users. ReadBasic. ALL</span><span class="sxs-lookup"><span data-stu-id="953a6-175">Users.ReadBasic.All</span></span> |
| [<span data-ttu-id="953a6-176">/ме/календарвиев</span><span class="sxs-lookup"><span data-stu-id="953a6-176">/me/calendarview</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0) | <span data-ttu-id="953a6-177">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="953a6-177">Contacts.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="953a6-178">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="953a6-178">Authentication</span></span>

<span data-ttu-id="953a6-179">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="953a6-179">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="953a6-180">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="953a6-180">Extend for more control</span></span>

<span data-ttu-id="953a6-181">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected render*` способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="953a6-181">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="953a6-182">Метод</span><span class="sxs-lookup"><span data-stu-id="953a6-182">Method</span></span> | <span data-ttu-id="953a6-183">Описание</span><span class="sxs-lookup"><span data-stu-id="953a6-183">Description</span></span> |
| - | - |
| <span data-ttu-id="953a6-184">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="953a6-184">renderLoading</span></span> | <span data-ttu-id="953a6-185">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="953a6-185">Renders the loading state.</span></span> |
| <span data-ttu-id="953a6-186">рендернодата</span><span class="sxs-lookup"><span data-stu-id="953a6-186">renderNoData</span></span> | <span data-ttu-id="953a6-187">Отрисовывает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="953a6-187">Renders the empty data state.</span></span> |
| <span data-ttu-id="953a6-188">рендерпеопле</span><span class="sxs-lookup"><span data-stu-id="953a6-188">renderPeople</span></span> | <span data-ttu-id="953a6-189">Отрисовывает список людей вплоть до `show-max` значения.</span><span class="sxs-lookup"><span data-stu-id="953a6-189">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="953a6-190">рендерперсон</span><span class="sxs-lookup"><span data-stu-id="953a6-190">renderPerson</span></span> | <span data-ttu-id="953a6-191">Отрисовывает отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="953a6-191">Renders an individual person.</span></span> |
| <span data-ttu-id="953a6-192">рендероверфлов</span><span class="sxs-lookup"><span data-stu-id="953a6-192">renderOverflow</span></span> | <span data-ttu-id="953a6-193">Отрисовывает представление оставшихся пользователей за пределами `show-max` значения.</span><span class="sxs-lookup"><span data-stu-id="953a6-193">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
