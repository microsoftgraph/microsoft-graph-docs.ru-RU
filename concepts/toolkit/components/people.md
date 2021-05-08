---
title: Компонент People в Microsoft Graph Toolkit
description: Вы можете использовать веб-компонент `mgt-people`, чтобы отображать группу людей или контактов с помощью фотографий и инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0cdade8720112dc623e617514f31ab63151b80ff
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266852"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f1bca-103">Компонент People в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f1bca-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f1bca-104">Вы можете использовать веб-компонент `mgt-people`, чтобы отображать группу людей или контактов с помощью фотографий и инициалов.</span><span class="sxs-lookup"><span data-stu-id="f1bca-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="f1bca-105">По умолчанию отображаются наиболее популярные контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="f1bca-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="f1bca-106">Этот компонент использует несколько элементов управления [mgt-person](./person.md), но его можно связать с набором дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="f1bca-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="f1bca-107">Если нужно отобразить больше людей, чем значение `show-max`, будет добавлено число, чтобы указать количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="f1bca-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="f1bca-108">Пример</span><span class="sxs-lookup"><span data-stu-id="f1bca-108">Example</span></span>

<span data-ttu-id="f1bca-109">В следующем примере показана группа людей, отображенная с помощью компонента `mgt-people`.</span><span class="sxs-lookup"><span data-stu-id="f1bca-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="f1bca-110">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="f1bca-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="f1bca-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="f1bca-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="f1bca-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1bca-112">Properties</span></span>

<span data-ttu-id="f1bca-113">По умолчанию компонент `mgt-people` извлекает события из конечной точки `/me/people` с помощью фильтра `personType/class eq 'Person'`, чтобы отобразить пользователей, часто выступающих в роли контактов.</span><span class="sxs-lookup"><span data-stu-id="f1bca-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="f1bca-114">Это поведение можно изменить с помощью нескольких свойств.</span><span class="sxs-lookup"><span data-stu-id="f1bca-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="f1bca-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="f1bca-115">Attribute</span></span> | <span data-ttu-id="f1bca-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1bca-116">Property</span></span> | <span data-ttu-id="f1bca-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f1bca-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f1bca-118">show-max</span><span class="sxs-lookup"><span data-stu-id="f1bca-118">show-max</span></span> | <span data-ttu-id="f1bca-119">showMax</span><span class="sxs-lookup"><span data-stu-id="f1bca-119">showMax</span></span> | <span data-ttu-id="f1bca-120">Указывает максимальное количество пользователей для отображения.</span><span class="sxs-lookup"><span data-stu-id="f1bca-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="f1bca-121">Значение по умолчанию: 3.</span><span class="sxs-lookup"><span data-stu-id="f1bca-121">Default value is 3.</span></span> |
| <span data-ttu-id="f1bca-122">people</span><span class="sxs-lookup"><span data-stu-id="f1bca-122">people</span></span> | <span data-ttu-id="f1bca-123">people</span><span class="sxs-lookup"><span data-stu-id="f1bca-123">people</span></span> | <span data-ttu-id="f1bca-124">Массив людей для получения или настройки списка людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="f1bca-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="f1bca-125">Это свойство используется для доступа к людям, загружаемым компонентом.</span><span class="sxs-lookup"><span data-stu-id="f1bca-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="f1bca-126">Настройте это значение, чтобы загружать своих людей.</span><span class="sxs-lookup"><span data-stu-id="f1bca-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="f1bca-127">group-id</span><span class="sxs-lookup"><span data-stu-id="f1bca-127">group-id</span></span> | <span data-ttu-id="f1bca-128">groupId</span><span class="sxs-lookup"><span data-stu-id="f1bca-128">groupId</span></span> | <span data-ttu-id="f1bca-129">Получает людей из определенного интерфейса Microsoft Graph по соответствующему идентификатору.</span><span class="sxs-lookup"><span data-stu-id="f1bca-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="f1bca-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="f1bca-130">user-ids</span></span> | <span data-ttu-id="f1bca-131">userIds</span><span class="sxs-lookup"><span data-stu-id="f1bca-131">userIds</span></span> | <span data-ttu-id="f1bca-132">При наличии массива пользовательских `ids` Microsoft Graph компонент отображает этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="f1bca-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="f1bca-133">people-queries</span><span class="sxs-lookup"><span data-stu-id="f1bca-133">people-queries</span></span> | <span data-ttu-id="f1bca-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="f1bca-134">peopleQueries</span></span> | <span data-ttu-id="f1bca-135">При наличии массива запросов пользователей (имена, UPN, адреса электронной почты) компонент отображает этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="f1bca-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="f1bca-136">person-card</span><span class="sxs-lookup"><span data-stu-id="f1bca-136">person-card</span></span> | <span data-ttu-id="f1bca-137">personCard</span><span class="sxs-lookup"><span data-stu-id="f1bca-137">personCard</span></span> | <span data-ttu-id="f1bca-138">Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`.</span><span class="sxs-lookup"><span data-stu-id="f1bca-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="f1bca-139">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="f1bca-139">Default value is `none`.</span></span> |
| <span data-ttu-id="f1bca-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="f1bca-140">show-presence</span></span> | <span data-ttu-id="f1bca-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="f1bca-141">showPresence</span></span> | <span data-ttu-id="f1bca-142">Логическое значение, определяющее, нужно ли отображать значок присутствия пользователя на изображении пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1bca-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="f1bca-143">В следующем примере задается максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="f1bca-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="f1bca-144">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="f1bca-144">CSS custom properties</span></span>

<span data-ttu-id="f1bca-145">Компонент `mgt-people` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="f1bca-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="f1bca-146">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="f1bca-146">Templates</span></span>

<span data-ttu-id="f1bca-147">`mgt-people` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="f1bca-147">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="f1bca-148">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="f1bca-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f1bca-149">Тип данных</span><span class="sxs-lookup"><span data-stu-id="f1bca-149">Data type</span></span> | <span data-ttu-id="f1bca-150">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="f1bca-150">Data context</span></span> | <span data-ttu-id="f1bca-151">Описание</span><span class="sxs-lookup"><span data-stu-id="f1bca-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="f1bca-152">`people`: список объектов пользователей</span><span class="sxs-lookup"><span data-stu-id="f1bca-152">`people`: list of person objects</span></span> | <span data-ttu-id="f1bca-153">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="f1bca-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="f1bca-154">`person`: объект пользователя</span><span class="sxs-lookup"><span data-stu-id="f1bca-154">`person`: person object</span></span> | <span data-ttu-id="f1bca-155">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1bca-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="f1bca-156">`people`: список объектов пользователей</span><span class="sxs-lookup"><span data-stu-id="f1bca-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="f1bca-157">`max`: количество отображенных людей</span><span class="sxs-lookup"><span data-stu-id="f1bca-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="f1bca-158">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="f1bca-158">`extra`: number of extra people</span></span> | <span data-ttu-id="f1bca-159">Шаблон, используемый для отображения количества, превышающего максимальное значение, справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="f1bca-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="f1bca-160">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="f1bca-160">No data context is passed</span></span> | <span data-ttu-id="f1bca-161">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="f1bca-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="f1bca-162">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="f1bca-162">No data context is passed</span></span> | <span data-ttu-id="f1bca-163">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="f1bca-163">The template used while the component loads state.</span></span>

<span data-ttu-id="f1bca-164">В следующих примерах показано, как использовать шаблон `person`.</span><span class="sxs-lookup"><span data-stu-id="f1bca-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f1bca-165">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f1bca-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="f1bca-166">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f1bca-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="f1bca-167">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f1bca-167">Resource</span></span> | <span data-ttu-id="f1bca-168">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f1bca-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="f1bca-169">/me/people</span><span class="sxs-lookup"><span data-stu-id="f1bca-169">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="f1bca-170">Когда вы используете шаблоны по умолчанию, требуются дополнительные API и разрешения.</span><span class="sxs-lookup"><span data-stu-id="f1bca-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="f1bca-171">Шаблон по умолчанию для этого компонента использует компонент [mgt-person](person.md), для которого требуются следующие элементы.</span><span class="sxs-lookup"><span data-stu-id="f1bca-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="f1bca-172">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f1bca-172">Resource</span></span> | <span data-ttu-id="f1bca-173">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f1bca-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="f1bca-174">/users</span><span class="sxs-lookup"><span data-stu-id="f1bca-174">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="f1bca-175">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f1bca-175">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="f1bca-176">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="f1bca-176">Authentication</span></span>

<span data-ttu-id="f1bca-177">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="f1bca-177">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="f1bca-178">Кэш</span><span class="sxs-lookup"><span data-stu-id="f1bca-178">Cache</span></span>

|<span data-ttu-id="f1bca-179">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="f1bca-179">Object store</span></span>|<span data-ttu-id="f1bca-180">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="f1bca-180">Cached data</span></span>|<span data-ttu-id="f1bca-181">Примечания</span><span class="sxs-lookup"><span data-stu-id="f1bca-181">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="f1bca-182">Сведения о пользователях, совпадающих с запросом</span><span class="sxs-lookup"><span data-stu-id="f1bca-182">Information about people matching the query</span></span>|<span data-ttu-id="f1bca-183">Используется при `resource` указании</span><span class="sxs-lookup"><span data-stu-id="f1bca-183">Used when `resource` specified</span></span>|
|`users`|<span data-ttu-id="f1bca-184">Сведения о пользователях, совпадающих с запросом</span><span class="sxs-lookup"><span data-stu-id="f1bca-184">Information about users matching the query</span></span>|<span data-ttu-id="f1bca-185">Используется `groupId` при указании свойств или без `userIds` `peopleQueries` указанных свойств</span><span class="sxs-lookup"><span data-stu-id="f1bca-185">Used when `groupId`, `userIds`, `peopleQueries` or no properties specified</span></span>|
|`presence`|<span data-ttu-id="f1bca-186">Присутствие для указанного набора людей</span><span class="sxs-lookup"><span data-stu-id="f1bca-186">Presence for the specified set of people</span></span>|<span data-ttu-id="f1bca-187">Используется при `showPresence` наборе `true`</span><span class="sxs-lookup"><span data-stu-id="f1bca-187">Used when `showPresence` set to `true`</span></span>|

> [!NOTE]
> <span data-ttu-id="f1bca-188">По умолчанию компонент `mgt-people` использует компонент для отображения [`mgt-person`](./person.md) сведений о человеке.</span><span class="sxs-lookup"><span data-stu-id="f1bca-188">By default, the `mgt-people` component uses the [`mgt-person`](./person.md) component to display information about people.</span></span> <span data-ttu-id="f1bca-189">Компонент `mgt-person` автоматически загружает и кэшируется фотографию для каждого человека.</span><span class="sxs-lookup"><span data-stu-id="f1bca-189">The `mgt-person` component automatically downloads and caches the photo for each person.</span></span>

<span data-ttu-id="f1bca-190">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="f1bca-190">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="f1bca-191">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="f1bca-191">Extend for more control</span></span>

<span data-ttu-id="f1bca-192">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="f1bca-192">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="f1bca-193">Метод</span><span class="sxs-lookup"><span data-stu-id="f1bca-193">Method</span></span> | <span data-ttu-id="f1bca-194">Описание</span><span class="sxs-lookup"><span data-stu-id="f1bca-194">Description</span></span> |
| - | - |
| <span data-ttu-id="f1bca-195">renderLoading</span><span class="sxs-lookup"><span data-stu-id="f1bca-195">renderLoading</span></span> | <span data-ttu-id="f1bca-196">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="f1bca-196">Renders the loading state.</span></span> |
| <span data-ttu-id="f1bca-197">renderNoData</span><span class="sxs-lookup"><span data-stu-id="f1bca-197">renderNoData</span></span> | <span data-ttu-id="f1bca-198">Отображает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="f1bca-198">Renders the empty data state.</span></span> |
| <span data-ttu-id="f1bca-199">renderPeople</span><span class="sxs-lookup"><span data-stu-id="f1bca-199">renderPeople</span></span> | <span data-ttu-id="f1bca-200">Отображает список людей до значения `show-max`.</span><span class="sxs-lookup"><span data-stu-id="f1bca-200">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="f1bca-201">renderPerson</span><span class="sxs-lookup"><span data-stu-id="f1bca-201">renderPerson</span></span> | <span data-ttu-id="f1bca-202">Отображает отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1bca-202">Renders an individual person.</span></span> |
| <span data-ttu-id="f1bca-203">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="f1bca-203">renderOverflow</span></span> | <span data-ttu-id="f1bca-204">Отображает представление оставшегося количества людей, превышающего значение `show-max`.</span><span class="sxs-lookup"><span data-stu-id="f1bca-204">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
