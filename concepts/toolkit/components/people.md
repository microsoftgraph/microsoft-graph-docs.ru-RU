---
title: Компонент "Люди" в microsoft Graph набор средств
description: Веб-компонент можно использовать для отображения группы людей или контактов с помощью фотографий `mgt-people` или инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9e19636c6f69784984d7438d53f57bac78fc6675
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660060"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0686c-103">Компонент "Люди" в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="0686c-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0686c-104">Веб-компонент можно использовать для отображения группы людей или контактов с помощью фотографий `mgt-people` или инициалов.</span><span class="sxs-lookup"><span data-stu-id="0686c-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="0686c-105">По умолчанию отображаются наиболее частые контакты для пользователя, выписав его.</span><span class="sxs-lookup"><span data-stu-id="0686c-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="0686c-106">Этот компонент использует несколько [элементов управления mgt-person,](./person.md) но его можно привязить к набору дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="0686c-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="0686c-107">Если отображается больше людей, чем значение, будет добавлено число, чтобы указать количество `show-max` дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="0686c-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="0686c-108">Пример</span><span class="sxs-lookup"><span data-stu-id="0686c-108">Example</span></span>

<span data-ttu-id="0686c-109">В следующем примере показана группа людей, отображаемая с помощью `mgt-people` компонента.</span><span class="sxs-lookup"><span data-stu-id="0686c-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="0686c-110">С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="0686c-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="0686c-111">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="0686c-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="0686c-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="0686c-112">Properties</span></span>

<span data-ttu-id="0686c-113">По умолчанию компонент получает события из конечной точки с фильтром для отображения `mgt-people` `/me/people` часто `personType/class eq 'Person'` используемых пользователей.</span><span class="sxs-lookup"><span data-stu-id="0686c-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="0686c-114">Для изменения этого поведения можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="0686c-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="0686c-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="0686c-115">Attribute</span></span> | <span data-ttu-id="0686c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0686c-116">Property</span></span> | <span data-ttu-id="0686c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0686c-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="0686c-118">show-max</span><span class="sxs-lookup"><span data-stu-id="0686c-118">show-max</span></span> | <span data-ttu-id="0686c-119">showMax</span><span class="sxs-lookup"><span data-stu-id="0686c-119">showMax</span></span> | <span data-ttu-id="0686c-120">Указывает максимальное количество людей, которые необходимо показать.</span><span class="sxs-lookup"><span data-stu-id="0686c-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="0686c-121">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="0686c-121">Default value is 3.</span></span> |
| <span data-ttu-id="0686c-122">people</span><span class="sxs-lookup"><span data-stu-id="0686c-122">people</span></span> | <span data-ttu-id="0686c-123">people</span><span class="sxs-lookup"><span data-stu-id="0686c-123">people</span></span> | <span data-ttu-id="0686c-124">Массив людей, которые будут получать или устанавливать список людей, отрисовав их с помощью компонента.</span><span class="sxs-lookup"><span data-stu-id="0686c-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="0686c-125">Используйте это свойство для доступа к людям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="0686c-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="0686c-126">Установите это значение для загрузки собственных людей.</span><span class="sxs-lookup"><span data-stu-id="0686c-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="0686c-127">group-id</span><span class="sxs-lookup"><span data-stu-id="0686c-127">group-id</span></span> | <span data-ttu-id="0686c-128">groupId</span><span class="sxs-lookup"><span data-stu-id="0686c-128">groupId</span></span> | <span data-ttu-id="0686c-129">Извлекает людей из определенного Microsoft Graph из соответствующего ИД.</span><span class="sxs-lookup"><span data-stu-id="0686c-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="0686c-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="0686c-130">user-ids</span></span> | <span data-ttu-id="0686c-131">userIds</span><span class="sxs-lookup"><span data-stu-id="0686c-131">userIds</span></span> | <span data-ttu-id="0686c-132">С учетом массива пользователей Microsoft Graph `ids` компонент будет отрисовки этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="0686c-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="0686c-133">people-queries</span><span class="sxs-lookup"><span data-stu-id="0686c-133">people-queries</span></span> | <span data-ttu-id="0686c-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="0686c-134">peopleQueries</span></span> | <span data-ttu-id="0686c-135">С учетом массива запросов пользователей (имен, имен и сообщений электронной почты) компонент будет отрисовки этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="0686c-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="0686c-136">person-card</span><span class="sxs-lookup"><span data-stu-id="0686c-136">person-card</span></span> | <span data-ttu-id="0686c-137">personCard</span><span class="sxs-lookup"><span data-stu-id="0686c-137">personCard</span></span> | <span data-ttu-id="0686c-138">Enumeration to determine user action necessary to activate flyout panel - `hover` or `click` .</span><span class="sxs-lookup"><span data-stu-id="0686c-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="0686c-139">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="0686c-139">Default value is `none`.</span></span> |
| <span data-ttu-id="0686c-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="0686c-140">show-presence</span></span> | <span data-ttu-id="0686c-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="0686c-141">showPresence</span></span> | <span data-ttu-id="0686c-142">Boolean, чтобы определить, следует ли показывать эмблему присутствия человека на изображении человека.</span><span class="sxs-lookup"><span data-stu-id="0686c-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="0686c-143">В следующем примере устанавливается максимальное число пользователей для показа.</span><span class="sxs-lookup"><span data-stu-id="0686c-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="0686c-144">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="0686c-144">CSS custom properties</span></span>

<span data-ttu-id="0686c-145">Компонент `mgt-people` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="0686c-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="0686c-146">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="0686c-146">Templates</span></span>

<span data-ttu-id="0686c-147">Поддерживаются `mgt-people` несколько [шаблонов,](../customize-components/templates.md) которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="0686c-147">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="0686c-148">Чтобы указать шаблон, включив элемент в `<template>` компонент, закажите одно из `data-type` следующих значений.</span><span class="sxs-lookup"><span data-stu-id="0686c-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="0686c-149">Тип данных</span><span class="sxs-lookup"><span data-stu-id="0686c-149">Data type</span></span> | <span data-ttu-id="0686c-150">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="0686c-150">Data context</span></span> | <span data-ttu-id="0686c-151">Описание</span><span class="sxs-lookup"><span data-stu-id="0686c-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="0686c-152">`people`: список объектов person</span><span class="sxs-lookup"><span data-stu-id="0686c-152">`people`: list of person objects</span></span> | <span data-ttu-id="0686c-153">Шаблон по умолчанию заменяет весь компонент на собственный.</span><span class="sxs-lookup"><span data-stu-id="0686c-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="0686c-154">`person`: объект person</span><span class="sxs-lookup"><span data-stu-id="0686c-154">`person`: person object</span></span> | <span data-ttu-id="0686c-155">Шаблон, используемый для отображения каждого человека.</span><span class="sxs-lookup"><span data-stu-id="0686c-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="0686c-156">`people`: список объектов person</span><span class="sxs-lookup"><span data-stu-id="0686c-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="0686c-157">`max`: количество показанных людей</span><span class="sxs-lookup"><span data-stu-id="0686c-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="0686c-158">`extra`: количество дополнительных пользователей</span><span class="sxs-lookup"><span data-stu-id="0686c-158">`extra`: number of extra people</span></span> | <span data-ttu-id="0686c-159">Шаблон, используемый для отрисовки числа, пре пре преставливаемого справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="0686c-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="0686c-160">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="0686c-160">No data context is passed</span></span> | <span data-ttu-id="0686c-161">Шаблон, используемый, когда данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="0686c-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="0686c-162">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="0686c-162">No data context is passed</span></span> | <span data-ttu-id="0686c-163">Шаблон, используемый во время загрузки состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="0686c-163">The template used while the component loads state.</span></span>

<span data-ttu-id="0686c-164">В следующих примерах показано, как использовать `person` шаблон.</span><span class="sxs-lookup"><span data-stu-id="0686c-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="0686c-165">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0686c-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="0686c-166">Этот компонент использует следующие API Microsoft Graph и разрешения:</span><span class="sxs-lookup"><span data-stu-id="0686c-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="0686c-167">Ресурс</span><span class="sxs-lookup"><span data-stu-id="0686c-167">Resource</span></span> | <span data-ttu-id="0686c-168">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0686c-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="0686c-169">/me/people</span><span class="sxs-lookup"><span data-stu-id="0686c-169">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="0686c-170">При использовании шаблонов по умолчанию требуются дополнительные API и разрешения.</span><span class="sxs-lookup"><span data-stu-id="0686c-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="0686c-171">Шаблон по умолчанию для этого компонента использует компонент [mgt-person,](person.md) для чего требуется следующее.</span><span class="sxs-lookup"><span data-stu-id="0686c-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="0686c-172">Ресурс</span><span class="sxs-lookup"><span data-stu-id="0686c-172">Resource</span></span> | <span data-ttu-id="0686c-173">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0686c-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="0686c-174">/users</span><span class="sxs-lookup"><span data-stu-id="0686c-174">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="0686c-175">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="0686c-175">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="0686c-176">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="0686c-176">Authentication</span></span>

<span data-ttu-id="0686c-177">В этом контроле используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="0686c-177">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="0686c-178">Расширение для большего контроля</span><span class="sxs-lookup"><span data-stu-id="0686c-178">Extend for more control</span></span>

<span data-ttu-id="0686c-179">Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="0686c-179">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="0686c-180">Метод</span><span class="sxs-lookup"><span data-stu-id="0686c-180">Method</span></span> | <span data-ttu-id="0686c-181">Описание</span><span class="sxs-lookup"><span data-stu-id="0686c-181">Description</span></span> |
| - | - |
| <span data-ttu-id="0686c-182">renderLoading</span><span class="sxs-lookup"><span data-stu-id="0686c-182">renderLoading</span></span> | <span data-ttu-id="0686c-183">Отрисовка состояния загрузки.</span><span class="sxs-lookup"><span data-stu-id="0686c-183">Renders the loading state.</span></span> |
| <span data-ttu-id="0686c-184">renderNoData</span><span class="sxs-lookup"><span data-stu-id="0686c-184">renderNoData</span></span> | <span data-ttu-id="0686c-185">Отрисовка пустого состояния данных.</span><span class="sxs-lookup"><span data-stu-id="0686c-185">Renders the empty data state.</span></span> |
| <span data-ttu-id="0686c-186">renderPeople</span><span class="sxs-lookup"><span data-stu-id="0686c-186">renderPeople</span></span> | <span data-ttu-id="0686c-187">Отрисовка списка людей в до `show-max` значения.</span><span class="sxs-lookup"><span data-stu-id="0686c-187">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="0686c-188">renderPerson</span><span class="sxs-lookup"><span data-stu-id="0686c-188">renderPerson</span></span> | <span data-ttu-id="0686c-189">Отрисовка отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="0686c-189">Renders an individual person.</span></span> |
| <span data-ttu-id="0686c-190">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="0686c-190">renderOverflow</span></span> | <span data-ttu-id="0686c-191">Отрисовка представления оставшихся людей за `show-max` пределами значения.</span><span class="sxs-lookup"><span data-stu-id="0686c-191">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
