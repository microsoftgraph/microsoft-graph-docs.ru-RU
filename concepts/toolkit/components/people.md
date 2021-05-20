---
title: Компонент People в Microsoft Graph Toolkit
description: Вы можете использовать веб-компонент `mgt-people`, чтобы отображать группу людей или контактов с помощью фотографий и инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 6bed8f2c06e3c6834533b8e881016c4bc6d54bac
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52580017"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f347d-103">Компонент People в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f347d-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f347d-104">Вы можете использовать веб-компонент `mgt-people`, чтобы отображать группу людей или контактов с помощью фотографий и инициалов.</span><span class="sxs-lookup"><span data-stu-id="f347d-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="f347d-105">По умолчанию отображаются наиболее популярные контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="f347d-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="f347d-106">Этот компонент использует несколько элементов управления [mgt-person](./person.md), но его можно связать с набором дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="f347d-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="f347d-107">Если нужно отобразить больше людей, чем значение `show-max`, будет добавлено число, чтобы указать количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="f347d-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="f347d-108">Пример</span><span class="sxs-lookup"><span data-stu-id="f347d-108">Example</span></span>

<span data-ttu-id="f347d-109">В следующем примере показана группа людей, отображенная с помощью компонента `mgt-people`.</span><span class="sxs-lookup"><span data-stu-id="f347d-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="f347d-110">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="f347d-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="f347d-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="f347d-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="f347d-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="f347d-112">Properties</span></span>

<span data-ttu-id="f347d-113">По умолчанию компонент `mgt-people` извлекает события из конечной точки `/me/people` с помощью фильтра `personType/class eq 'Person'`, чтобы отобразить пользователей, часто выступающих в роли контактов.</span><span class="sxs-lookup"><span data-stu-id="f347d-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="f347d-114">Это поведение можно изменить с помощью нескольких свойств.</span><span class="sxs-lookup"><span data-stu-id="f347d-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="f347d-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="f347d-115">Attribute</span></span> | <span data-ttu-id="f347d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="f347d-116">Property</span></span> | <span data-ttu-id="f347d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f347d-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f347d-118">show-max</span><span class="sxs-lookup"><span data-stu-id="f347d-118">show-max</span></span> | <span data-ttu-id="f347d-119">showMax</span><span class="sxs-lookup"><span data-stu-id="f347d-119">showMax</span></span> | <span data-ttu-id="f347d-120">Указывает максимальное количество пользователей для отображения.</span><span class="sxs-lookup"><span data-stu-id="f347d-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="f347d-121">Значение по умолчанию: 3.</span><span class="sxs-lookup"><span data-stu-id="f347d-121">Default value is 3.</span></span> |
| <span data-ttu-id="f347d-122">people</span><span class="sxs-lookup"><span data-stu-id="f347d-122">people</span></span> | <span data-ttu-id="f347d-123">people</span><span class="sxs-lookup"><span data-stu-id="f347d-123">people</span></span> | <span data-ttu-id="f347d-124">Массив людей для получения или настройки списка людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="f347d-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="f347d-125">Это свойство используется для доступа к людям, загружаемым компонентом.</span><span class="sxs-lookup"><span data-stu-id="f347d-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="f347d-126">Настройте это значение, чтобы загружать своих людей.</span><span class="sxs-lookup"><span data-stu-id="f347d-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="f347d-127">group-id</span><span class="sxs-lookup"><span data-stu-id="f347d-127">group-id</span></span> | <span data-ttu-id="f347d-128">groupId</span><span class="sxs-lookup"><span data-stu-id="f347d-128">groupId</span></span> | <span data-ttu-id="f347d-129">Получает людей из определенного интерфейса Microsoft Graph по соответствующему идентификатору.</span><span class="sxs-lookup"><span data-stu-id="f347d-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="f347d-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="f347d-130">user-ids</span></span> | <span data-ttu-id="f347d-131">userIds</span><span class="sxs-lookup"><span data-stu-id="f347d-131">userIds</span></span> | <span data-ttu-id="f347d-132">При наличии массива пользовательских `ids` Microsoft Graph компонент отображает этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="f347d-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="f347d-133">people-queries</span><span class="sxs-lookup"><span data-stu-id="f347d-133">people-queries</span></span> | <span data-ttu-id="f347d-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="f347d-134">peopleQueries</span></span> | <span data-ttu-id="f347d-135">При наличии массива запросов пользователей (имена, UPN, адреса электронной почты) компонент отображает этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="f347d-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="f347d-136">person-card</span><span class="sxs-lookup"><span data-stu-id="f347d-136">person-card</span></span> | <span data-ttu-id="f347d-137">personCard</span><span class="sxs-lookup"><span data-stu-id="f347d-137">personCard</span></span> | <span data-ttu-id="f347d-138">Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`.</span><span class="sxs-lookup"><span data-stu-id="f347d-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="f347d-139">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="f347d-139">Default value is `none`.</span></span> |
| <span data-ttu-id="f347d-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="f347d-140">show-presence</span></span> | <span data-ttu-id="f347d-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="f347d-141">showPresence</span></span> | <span data-ttu-id="f347d-142">Логическое значение, определяющее, нужно ли отображать значок присутствия пользователя на изображении пользователя.</span><span class="sxs-lookup"><span data-stu-id="f347d-142">A boolean to determine whether to show person presence badge on person image.</span></span> |
| <span data-ttu-id="f347d-143">resource</span><span class="sxs-lookup"><span data-stu-id="f347d-143">resource</span></span> | <span data-ttu-id="f347d-144">resource</span><span class="sxs-lookup"><span data-stu-id="f347d-144">resource</span></span> | <span data-ttu-id="f347d-145">Ресурс, который требуется получить из Microsoft Graph (например, `/me/people`).</span><span class="sxs-lookup"><span data-stu-id="f347d-145">The resource to get from Microsoft Graph (for example, `/me/people`).</span></span> |
| <span data-ttu-id="f347d-146">scopes</span><span class="sxs-lookup"><span data-stu-id="f347d-146">scopes</span></span> | <span data-ttu-id="f347d-147">scopes</span><span class="sxs-lookup"><span data-stu-id="f347d-147">scopes</span></span> | <span data-ttu-id="f347d-148">Необязательный массив строк, если используется свойство либо область с разделителями-запятыми, при использовании атрибута.</span><span class="sxs-lookup"><span data-stu-id="f347d-148">Optional array of strings if using the property or a comma delimited scope if using the attribute.</span></span> <span data-ttu-id="f347d-149">Эти области используются компонентом (с поддерживаемым поставщиком), чтобы убедиться в том, что пользователь дал согласие на нужное разрешение.</span><span class="sxs-lookup"><span data-stu-id="f347d-149">The component will use these scopes (with a supported provider) to ensure that the user has consented to the right permission.</span></span> |
| <span data-ttu-id="f347d-150">version</span><span class="sxs-lookup"><span data-stu-id="f347d-150">version</span></span> | <span data-ttu-id="f347d-151">version</span><span class="sxs-lookup"><span data-stu-id="f347d-151">version</span></span> | <span data-ttu-id="f347d-152">Необязательная версия API, используемая при выполнении GET-запроса.</span><span class="sxs-lookup"><span data-stu-id="f347d-152">Optional API version to use when making the GET request.</span></span> <span data-ttu-id="f347d-153">Значение по умолчанию: `v1.0`.</span><span class="sxs-lookup"><span data-stu-id="f347d-153">Default is `v1.0`.</span></span>  |


<span data-ttu-id="f347d-154">В следующем примере задается максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="f347d-154">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="f347d-155">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="f347d-155">CSS custom properties</span></span>

<span data-ttu-id="f347d-156">Компонент `mgt-people` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="f347d-156">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="f347d-157">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="f347d-157">Templates</span></span>

<span data-ttu-id="f347d-158">`mgt-people` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="f347d-158">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="f347d-159">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="f347d-159">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f347d-160">Тип данных</span><span class="sxs-lookup"><span data-stu-id="f347d-160">Data type</span></span> | <span data-ttu-id="f347d-161">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="f347d-161">Data context</span></span> | <span data-ttu-id="f347d-162">Описание</span><span class="sxs-lookup"><span data-stu-id="f347d-162">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="f347d-163">`people`: список объектов пользователей</span><span class="sxs-lookup"><span data-stu-id="f347d-163">`people`: list of person objects</span></span> | <span data-ttu-id="f347d-164">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="f347d-164">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="f347d-165">`person`: объект пользователя</span><span class="sxs-lookup"><span data-stu-id="f347d-165">`person`: person object</span></span> | <span data-ttu-id="f347d-166">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f347d-166">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="f347d-167">`people`: список объектов пользователей</span><span class="sxs-lookup"><span data-stu-id="f347d-167">`people`: list of person objects</span></span> <br> <span data-ttu-id="f347d-168">`max`: количество отображенных людей</span><span class="sxs-lookup"><span data-stu-id="f347d-168">`max`: number of shown people</span></span> <br> <span data-ttu-id="f347d-169">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="f347d-169">`extra`: number of extra people</span></span> | <span data-ttu-id="f347d-170">Шаблон, используемый для отображения количества, превышающего максимальное значение, справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="f347d-170">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="f347d-171">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="f347d-171">No data context is passed</span></span> | <span data-ttu-id="f347d-172">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="f347d-172">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="f347d-173">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="f347d-173">No data context is passed</span></span> | <span data-ttu-id="f347d-174">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="f347d-174">The template used while the component loads state.</span></span>

<span data-ttu-id="f347d-175">В следующих примерах показано, как использовать шаблон `person`.</span><span class="sxs-lookup"><span data-stu-id="f347d-175">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f347d-176">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f347d-176">Microsoft Graph permissions</span></span>

<span data-ttu-id="f347d-177">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f347d-177">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="f347d-178">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f347d-178">Resource</span></span> | <span data-ttu-id="f347d-179">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f347d-179">Permission</span></span> |
| - | - |
| [<span data-ttu-id="f347d-180">/me/people</span><span class="sxs-lookup"><span data-stu-id="f347d-180">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="f347d-181">Когда вы используете шаблоны по умолчанию, требуются дополнительные API и разрешения.</span><span class="sxs-lookup"><span data-stu-id="f347d-181">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="f347d-182">Шаблон по умолчанию для этого компонента использует компонент [mgt-person](person.md), для которого требуются следующие элементы.</span><span class="sxs-lookup"><span data-stu-id="f347d-182">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="f347d-183">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f347d-183">Resource</span></span> | <span data-ttu-id="f347d-184">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f347d-184">Permission</span></span> |
| - | - |
| [<span data-ttu-id="f347d-185">/users</span><span class="sxs-lookup"><span data-stu-id="f347d-185">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="f347d-186">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f347d-186">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="f347d-187">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="f347d-187">Authentication</span></span>

<span data-ttu-id="f347d-188">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="f347d-188">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="f347d-189">Кэш</span><span class="sxs-lookup"><span data-stu-id="f347d-189">Cache</span></span>

|<span data-ttu-id="f347d-190">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="f347d-190">Object store</span></span>|<span data-ttu-id="f347d-191">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="f347d-191">Cached data</span></span>|<span data-ttu-id="f347d-192">Примечания</span><span class="sxs-lookup"><span data-stu-id="f347d-192">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="f347d-193">Сведения о пользователях, совпадающих с запросом</span><span class="sxs-lookup"><span data-stu-id="f347d-193">Information about people matching the query</span></span>|<span data-ttu-id="f347d-194">Используется при `resource` указании</span><span class="sxs-lookup"><span data-stu-id="f347d-194">Used when `resource` specified</span></span>|
|`users`|<span data-ttu-id="f347d-195">Сведения о пользователях, совпадающих с запросом</span><span class="sxs-lookup"><span data-stu-id="f347d-195">Information about users matching the query</span></span>|<span data-ttu-id="f347d-196">Используется `groupId` при указании свойств или без `userIds` `peopleQueries` указанных свойств</span><span class="sxs-lookup"><span data-stu-id="f347d-196">Used when `groupId`, `userIds`, `peopleQueries` or no properties specified</span></span>|
|`presence`|<span data-ttu-id="f347d-197">Присутствие для указанного набора людей</span><span class="sxs-lookup"><span data-stu-id="f347d-197">Presence for the specified set of people</span></span>|<span data-ttu-id="f347d-198">Используется при `showPresence` наборе `true`</span><span class="sxs-lookup"><span data-stu-id="f347d-198">Used when `showPresence` set to `true`</span></span>|

> [!NOTE]
> <span data-ttu-id="f347d-199">По умолчанию компонент `mgt-people` использует компонент для отображения [`mgt-person`](./person.md) сведений о человеке.</span><span class="sxs-lookup"><span data-stu-id="f347d-199">By default, the `mgt-people` component uses the [`mgt-person`](./person.md) component to display information about people.</span></span> <span data-ttu-id="f347d-200">Компонент `mgt-person` автоматически загружает и кэшируется фотографию для каждого человека.</span><span class="sxs-lookup"><span data-stu-id="f347d-200">The `mgt-person` component automatically downloads and caches the photo for each person.</span></span>

<span data-ttu-id="f347d-201">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="f347d-201">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="f347d-202">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="f347d-202">Extend for more control</span></span>

<span data-ttu-id="f347d-203">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="f347d-203">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="f347d-204">Метод</span><span class="sxs-lookup"><span data-stu-id="f347d-204">Method</span></span> | <span data-ttu-id="f347d-205">Описание</span><span class="sxs-lookup"><span data-stu-id="f347d-205">Description</span></span> |
| - | - |
| <span data-ttu-id="f347d-206">renderLoading</span><span class="sxs-lookup"><span data-stu-id="f347d-206">renderLoading</span></span> | <span data-ttu-id="f347d-207">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="f347d-207">Renders the loading state.</span></span> |
| <span data-ttu-id="f347d-208">renderNoData</span><span class="sxs-lookup"><span data-stu-id="f347d-208">renderNoData</span></span> | <span data-ttu-id="f347d-209">Отображает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="f347d-209">Renders the empty data state.</span></span> |
| <span data-ttu-id="f347d-210">renderPeople</span><span class="sxs-lookup"><span data-stu-id="f347d-210">renderPeople</span></span> | <span data-ttu-id="f347d-211">Отображает список людей до значения `show-max`.</span><span class="sxs-lookup"><span data-stu-id="f347d-211">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="f347d-212">renderPerson</span><span class="sxs-lookup"><span data-stu-id="f347d-212">renderPerson</span></span> | <span data-ttu-id="f347d-213">Отображает отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f347d-213">Renders an individual person.</span></span> |
| <span data-ttu-id="f347d-214">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="f347d-214">renderOverflow</span></span> | <span data-ttu-id="f347d-215">Отображает представление оставшегося количества людей, превышающего значение `show-max`.</span><span class="sxs-lookup"><span data-stu-id="f347d-215">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
