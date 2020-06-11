---
title: Компонент "люди" в наборе инструментов Microsoft Graph
description: Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: aa51f6d0c459425cdb9a01dbd3a61f5613e58678
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682028"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="af2a8-103">Компонент "люди" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="af2a8-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="af2a8-104">Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="af2a8-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="af2a8-105">По умолчанию отображаются наиболее часто используемые контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="af2a8-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="af2a8-106">Этот компонент использует несколько элементов управления " [центр](./person.md) управления", но их можно привязать к набору дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="af2a8-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="af2a8-107">Если количество людей для отображения больше `show-max` , чем значение, будет добавлено число, указывающее количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="af2a8-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="af2a8-108">Пример</span><span class="sxs-lookup"><span data-stu-id="af2a8-108">Example</span></span>

<span data-ttu-id="af2a8-109">В приведенном ниже примере показана группа людей, отображаемая с помощью `mgt-people` компонента.</span><span class="sxs-lookup"><span data-stu-id="af2a8-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="af2a8-110">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="af2a8-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="af2a8-111">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="af2a8-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="af2a8-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="af2a8-112">Properties</span></span>

<span data-ttu-id="af2a8-113">По умолчанию `mgt-people` компонент получает события от `/me/people` конечной точки с `personType/class eq 'Person'` фильтром для отображения часто обращенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="af2a8-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="af2a8-114">Для изменения этого поведения можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="af2a8-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="af2a8-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="af2a8-115">Attribute</span></span> | <span data-ttu-id="af2a8-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="af2a8-116">Property</span></span> | <span data-ttu-id="af2a8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="af2a8-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="af2a8-118">Show — Max</span><span class="sxs-lookup"><span data-stu-id="af2a8-118">show-max</span></span> | <span data-ttu-id="af2a8-119">шовмакс</span><span class="sxs-lookup"><span data-stu-id="af2a8-119">showMax</span></span> | <span data-ttu-id="af2a8-120">Указывает максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="af2a8-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="af2a8-121">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="af2a8-121">Default value is 3.</span></span> |
| <span data-ttu-id="af2a8-122">people</span><span class="sxs-lookup"><span data-stu-id="af2a8-122">people</span></span> | <span data-ttu-id="af2a8-123">people</span><span class="sxs-lookup"><span data-stu-id="af2a8-123">people</span></span> | <span data-ttu-id="af2a8-124">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="af2a8-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="af2a8-125">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="af2a8-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="af2a8-126">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="af2a8-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="af2a8-127">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="af2a8-127">group-id</span></span> | <span data-ttu-id="af2a8-128">groupId</span><span class="sxs-lookup"><span data-stu-id="af2a8-128">groupId</span></span> | <span data-ttu-id="af2a8-129">Извлекает пользователей из определенного идентификатора Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af2a8-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="af2a8-130">идентификаторы пользователей</span><span class="sxs-lookup"><span data-stu-id="af2a8-130">user-ids</span></span> | <span data-ttu-id="af2a8-131">userIds</span><span class="sxs-lookup"><span data-stu-id="af2a8-131">userIds</span></span> | <span data-ttu-id="af2a8-132">При наличии массива пользователей Microsoft Graph `ids` компонент будет отображать этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="af2a8-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="af2a8-133">люди — запросы</span><span class="sxs-lookup"><span data-stu-id="af2a8-133">people-queries</span></span> | <span data-ttu-id="af2a8-134">пеоплекуериес</span><span class="sxs-lookup"><span data-stu-id="af2a8-134">peopleQueries</span></span> | <span data-ttu-id="af2a8-135">При наличии массива запросов Person (Names, UPN, сообщений электронной почты) компонент будет отображать этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="af2a8-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="af2a8-136">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="af2a8-136">person-card</span></span> | <span data-ttu-id="af2a8-137">персонкард</span><span class="sxs-lookup"><span data-stu-id="af2a8-137">personCard</span></span> | <span data-ttu-id="af2a8-138">Перечисление для определения действия пользователя, необходимого для активации всплывающей панели `hover` `click` .</span><span class="sxs-lookup"><span data-stu-id="af2a8-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="af2a8-139">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="af2a8-139">Default value is `none`.</span></span> |
| <span data-ttu-id="af2a8-140">Показать — присутствие</span><span class="sxs-lookup"><span data-stu-id="af2a8-140">show-presence</span></span> | <span data-ttu-id="af2a8-141">шовпресенце</span><span class="sxs-lookup"><span data-stu-id="af2a8-141">showPresence</span></span> | <span data-ttu-id="af2a8-142">Логическое значение, определяющее, следует ли отображать значок присутствия пользователя на изображении пользователя.</span><span class="sxs-lookup"><span data-stu-id="af2a8-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="af2a8-143">В приведенном ниже примере задается максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="af2a8-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="af2a8-144">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="af2a8-144">CSS custom properties</span></span>

<span data-ttu-id="af2a8-145">`mgt-people`Компонент определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="af2a8-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="af2a8-146">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="af2a8-146">Templates</span></span>

<span data-ttu-id="af2a8-147">`mgt-people`Поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="af2a8-147">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="af2a8-148">Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="af2a8-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="af2a8-149">Тип данных</span><span class="sxs-lookup"><span data-stu-id="af2a8-149">Data type</span></span> | <span data-ttu-id="af2a8-150">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="af2a8-150">Data context</span></span> | <span data-ttu-id="af2a8-151">Description</span><span class="sxs-lookup"><span data-stu-id="af2a8-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="af2a8-152">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="af2a8-152">`people`: list of person objects</span></span> | <span data-ttu-id="af2a8-153">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="af2a8-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="af2a8-154">`person`: объект Person</span><span class="sxs-lookup"><span data-stu-id="af2a8-154">`person`: person object</span></span> | <span data-ttu-id="af2a8-155">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="af2a8-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="af2a8-156">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="af2a8-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="af2a8-157">`max`: количество показанных пользователей</span><span class="sxs-lookup"><span data-stu-id="af2a8-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="af2a8-158">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="af2a8-158">`extra`: number of extra people</span></span> | <span data-ttu-id="af2a8-159">Шаблон, используемый для отображения числа за пределами максимального значения справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="af2a8-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="af2a8-160">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="af2a8-160">No data context is passed</span></span> | <span data-ttu-id="af2a8-161">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="af2a8-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="af2a8-162">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="af2a8-162">No data context is passed</span></span> | <span data-ttu-id="af2a8-163">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="af2a8-163">The template used while the component loads state.</span></span>

<span data-ttu-id="af2a8-164">В приведенных ниже примерах показано, как использовать `person` шаблон.</span><span class="sxs-lookup"><span data-stu-id="af2a8-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="af2a8-165">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="af2a8-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="af2a8-166">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="af2a8-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="af2a8-167">Resource</span><span class="sxs-lookup"><span data-stu-id="af2a8-167">Resource</span></span> | <span data-ttu-id="af2a8-168">Permission</span><span class="sxs-lookup"><span data-stu-id="af2a8-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="af2a8-169">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="af2a8-169">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="af2a8-170">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="af2a8-170">Authentication</span></span>

<span data-ttu-id="af2a8-171">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="af2a8-171">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="af2a8-172">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="af2a8-172">Extend for more control</span></span>

<span data-ttu-id="af2a8-173">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected render*` способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="af2a8-173">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="af2a8-174">Метод</span><span class="sxs-lookup"><span data-stu-id="af2a8-174">Method</span></span> | <span data-ttu-id="af2a8-175">Описание</span><span class="sxs-lookup"><span data-stu-id="af2a8-175">Description</span></span> |
| - | - |
| <span data-ttu-id="af2a8-176">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="af2a8-176">renderLoading</span></span> | <span data-ttu-id="af2a8-177">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="af2a8-177">Renders the loading state.</span></span> |
| <span data-ttu-id="af2a8-178">рендернодата</span><span class="sxs-lookup"><span data-stu-id="af2a8-178">renderNoData</span></span> | <span data-ttu-id="af2a8-179">Отрисовывает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="af2a8-179">Renders the empty data state.</span></span> |
| <span data-ttu-id="af2a8-180">рендерпеопле</span><span class="sxs-lookup"><span data-stu-id="af2a8-180">renderPeople</span></span> | <span data-ttu-id="af2a8-181">Отрисовывает список людей вплоть до `show-max` значения.</span><span class="sxs-lookup"><span data-stu-id="af2a8-181">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="af2a8-182">рендерперсон</span><span class="sxs-lookup"><span data-stu-id="af2a8-182">renderPerson</span></span> | <span data-ttu-id="af2a8-183">Отрисовывает отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="af2a8-183">Renders an individual person.</span></span> |
| <span data-ttu-id="af2a8-184">рендероверфлов</span><span class="sxs-lookup"><span data-stu-id="af2a8-184">renderOverflow</span></span> | <span data-ttu-id="af2a8-185">Отрисовывает представление оставшихся пользователей за пределами `show-max` значения.</span><span class="sxs-lookup"><span data-stu-id="af2a8-185">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
