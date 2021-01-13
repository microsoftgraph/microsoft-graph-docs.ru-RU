---
title: Компонент People в Microsoft Graph Toolkit
description: Вы можете использовать веб-компонент `mgt-people`, чтобы отображать группу людей или контактов с помощью фотографий и инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9e19636c6f69784984d7438d53f57bac78fc6675
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660060"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="48ac4-103">Компонент People в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="48ac4-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="48ac4-104">Вы можете использовать веб-компонент `mgt-people`, чтобы отображать группу людей или контактов с помощью фотографий и инициалов.</span><span class="sxs-lookup"><span data-stu-id="48ac4-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="48ac4-105">По умолчанию отображаются наиболее популярные контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="48ac4-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="48ac4-106">Этот компонент использует несколько элементов управления [mgt-person](./person.md), но его можно связать с набором дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="48ac4-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="48ac4-107">Если нужно отобразить больше людей, чем значение `show-max`, будет добавлено число, чтобы указать количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="48ac4-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="48ac4-108">Пример</span><span class="sxs-lookup"><span data-stu-id="48ac4-108">Example</span></span>

<span data-ttu-id="48ac4-109">В следующем примере показана группа людей, отображенная с помощью компонента `mgt-people`.</span><span class="sxs-lookup"><span data-stu-id="48ac4-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="48ac4-110">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="48ac4-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="48ac4-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="48ac4-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="48ac4-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="48ac4-112">Properties</span></span>

<span data-ttu-id="48ac4-113">По умолчанию компонент `mgt-people` извлекает события из конечной точки `/me/people` с помощью фильтра `personType/class eq 'Person'`, чтобы отобразить пользователей, часто выступающих в роли контактов.</span><span class="sxs-lookup"><span data-stu-id="48ac4-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="48ac4-114">Это поведение можно изменить с помощью нескольких свойств.</span><span class="sxs-lookup"><span data-stu-id="48ac4-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="48ac4-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="48ac4-115">Attribute</span></span> | <span data-ttu-id="48ac4-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="48ac4-116">Property</span></span> | <span data-ttu-id="48ac4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="48ac4-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="48ac4-118">show-max</span><span class="sxs-lookup"><span data-stu-id="48ac4-118">show-max</span></span> | <span data-ttu-id="48ac4-119">showMax</span><span class="sxs-lookup"><span data-stu-id="48ac4-119">showMax</span></span> | <span data-ttu-id="48ac4-120">Указывает максимальное количество пользователей для отображения.</span><span class="sxs-lookup"><span data-stu-id="48ac4-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="48ac4-121">Значение по умолчанию: 3.</span><span class="sxs-lookup"><span data-stu-id="48ac4-121">Default value is 3.</span></span> |
| <span data-ttu-id="48ac4-122">people</span><span class="sxs-lookup"><span data-stu-id="48ac4-122">people</span></span> | <span data-ttu-id="48ac4-123">people</span><span class="sxs-lookup"><span data-stu-id="48ac4-123">people</span></span> | <span data-ttu-id="48ac4-124">Массив людей для получения или настройки списка людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="48ac4-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="48ac4-125">Это свойство используется для доступа к людям, загружаемым компонентом.</span><span class="sxs-lookup"><span data-stu-id="48ac4-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="48ac4-126">Настройте это значение, чтобы загружать своих людей.</span><span class="sxs-lookup"><span data-stu-id="48ac4-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="48ac4-127">group-id</span><span class="sxs-lookup"><span data-stu-id="48ac4-127">group-id</span></span> | <span data-ttu-id="48ac4-128">groupId</span><span class="sxs-lookup"><span data-stu-id="48ac4-128">groupId</span></span> | <span data-ttu-id="48ac4-129">Получает людей из определенного интерфейса Microsoft Graph по соответствующему идентификатору.</span><span class="sxs-lookup"><span data-stu-id="48ac4-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="48ac4-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="48ac4-130">user-ids</span></span> | <span data-ttu-id="48ac4-131">userIds</span><span class="sxs-lookup"><span data-stu-id="48ac4-131">userIds</span></span> | <span data-ttu-id="48ac4-132">При наличии массива пользовательских `ids` Microsoft Graph компонент отображает этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="48ac4-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="48ac4-133">people-queries</span><span class="sxs-lookup"><span data-stu-id="48ac4-133">people-queries</span></span> | <span data-ttu-id="48ac4-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="48ac4-134">peopleQueries</span></span> | <span data-ttu-id="48ac4-135">При наличии массива запросов пользователей (имена, UPN, адреса электронной почты) компонент отображает этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="48ac4-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="48ac4-136">person-card</span><span class="sxs-lookup"><span data-stu-id="48ac4-136">person-card</span></span> | <span data-ttu-id="48ac4-137">personCard</span><span class="sxs-lookup"><span data-stu-id="48ac4-137">personCard</span></span> | <span data-ttu-id="48ac4-138">Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`.</span><span class="sxs-lookup"><span data-stu-id="48ac4-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="48ac4-139">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="48ac4-139">Default value is `none`.</span></span> |
| <span data-ttu-id="48ac4-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="48ac4-140">show-presence</span></span> | <span data-ttu-id="48ac4-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="48ac4-141">showPresence</span></span> | <span data-ttu-id="48ac4-142">Логическое значение, определяющее, нужно ли отображать значок присутствия пользователя на изображении пользователя.</span><span class="sxs-lookup"><span data-stu-id="48ac4-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="48ac4-143">В следующем примере задается максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="48ac4-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="48ac4-144">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="48ac4-144">CSS custom properties</span></span>

<span data-ttu-id="48ac4-145">Компонент `mgt-people` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="48ac4-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="48ac4-146">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="48ac4-146">Templates</span></span>

<span data-ttu-id="48ac4-147">`mgt-people` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="48ac4-147">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="48ac4-148">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="48ac4-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="48ac4-149">Тип данных</span><span class="sxs-lookup"><span data-stu-id="48ac4-149">Data type</span></span> | <span data-ttu-id="48ac4-150">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="48ac4-150">Data context</span></span> | <span data-ttu-id="48ac4-151">Описание</span><span class="sxs-lookup"><span data-stu-id="48ac4-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="48ac4-152">`people`: список объектов пользователей</span><span class="sxs-lookup"><span data-stu-id="48ac4-152">`people`: list of person objects</span></span> | <span data-ttu-id="48ac4-153">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="48ac4-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="48ac4-154">`person`: объект пользователя</span><span class="sxs-lookup"><span data-stu-id="48ac4-154">`person`: person object</span></span> | <span data-ttu-id="48ac4-155">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="48ac4-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="48ac4-156">`people`: список объектов пользователей</span><span class="sxs-lookup"><span data-stu-id="48ac4-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="48ac4-157">`max`: количество отображенных людей</span><span class="sxs-lookup"><span data-stu-id="48ac4-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="48ac4-158">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="48ac4-158">`extra`: number of extra people</span></span> | <span data-ttu-id="48ac4-159">Шаблон, используемый для отображения количества, превышающего максимальное значение, справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="48ac4-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="48ac4-160">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="48ac4-160">No data context is passed</span></span> | <span data-ttu-id="48ac4-161">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="48ac4-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="48ac4-162">Контекст данных не передан</span><span class="sxs-lookup"><span data-stu-id="48ac4-162">No data context is passed</span></span> | <span data-ttu-id="48ac4-163">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="48ac4-163">The template used while the component loads state.</span></span>

<span data-ttu-id="48ac4-164">В следующих примерах показано, как использовать шаблон `person`.</span><span class="sxs-lookup"><span data-stu-id="48ac4-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="48ac4-165">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="48ac4-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="48ac4-166">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="48ac4-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="48ac4-167">Ресурс</span><span class="sxs-lookup"><span data-stu-id="48ac4-167">Resource</span></span> | <span data-ttu-id="48ac4-168">Разрешение</span><span class="sxs-lookup"><span data-stu-id="48ac4-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="48ac4-169">/me/people</span><span class="sxs-lookup"><span data-stu-id="48ac4-169">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="48ac4-170">Когда вы используете шаблоны по умолчанию, требуются дополнительные API и разрешения.</span><span class="sxs-lookup"><span data-stu-id="48ac4-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="48ac4-171">Шаблон по умолчанию для этого компонента использует компонент [mgt-person](person.md), для которого требуются следующие элементы.</span><span class="sxs-lookup"><span data-stu-id="48ac4-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="48ac4-172">Ресурс</span><span class="sxs-lookup"><span data-stu-id="48ac4-172">Resource</span></span> | <span data-ttu-id="48ac4-173">Разрешение</span><span class="sxs-lookup"><span data-stu-id="48ac4-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="48ac4-174">/users</span><span class="sxs-lookup"><span data-stu-id="48ac4-174">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="48ac4-175">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="48ac4-175">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="48ac4-176">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="48ac4-176">Authentication</span></span>

<span data-ttu-id="48ac4-177">В элементе управления используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="48ac4-177">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="48ac4-178">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="48ac4-178">Extend for more control</span></span>

<span data-ttu-id="48ac4-179">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="48ac4-179">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="48ac4-180">Метод</span><span class="sxs-lookup"><span data-stu-id="48ac4-180">Method</span></span> | <span data-ttu-id="48ac4-181">Описание</span><span class="sxs-lookup"><span data-stu-id="48ac4-181">Description</span></span> |
| - | - |
| <span data-ttu-id="48ac4-182">renderLoading</span><span class="sxs-lookup"><span data-stu-id="48ac4-182">renderLoading</span></span> | <span data-ttu-id="48ac4-183">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="48ac4-183">Renders the loading state.</span></span> |
| <span data-ttu-id="48ac4-184">renderNoData</span><span class="sxs-lookup"><span data-stu-id="48ac4-184">renderNoData</span></span> | <span data-ttu-id="48ac4-185">Отображает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="48ac4-185">Renders the empty data state.</span></span> |
| <span data-ttu-id="48ac4-186">renderPeople</span><span class="sxs-lookup"><span data-stu-id="48ac4-186">renderPeople</span></span> | <span data-ttu-id="48ac4-187">Отображает список людей до значения `show-max`.</span><span class="sxs-lookup"><span data-stu-id="48ac4-187">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="48ac4-188">renderPerson</span><span class="sxs-lookup"><span data-stu-id="48ac4-188">renderPerson</span></span> | <span data-ttu-id="48ac4-189">Отображает отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="48ac4-189">Renders an individual person.</span></span> |
| <span data-ttu-id="48ac4-190">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="48ac4-190">renderOverflow</span></span> | <span data-ttu-id="48ac4-191">Отображает представление оставшегося количества людей, превышающего значение `show-max`.</span><span class="sxs-lookup"><span data-stu-id="48ac4-191">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
