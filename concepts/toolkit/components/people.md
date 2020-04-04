---
title: Компонент "люди" в наборе инструментов Microsoft Graph
description: Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 34b7877b16d7f97d201e7bd96e1378c1e542bbcf
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144298"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="7b24d-103">Компонент "люди" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7b24d-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="7b24d-104">Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="7b24d-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="7b24d-105">По умолчанию отображаются наиболее часто используемые контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="7b24d-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="7b24d-106">Этот компонент использует несколько элементов управления " [центр](./person.md) управления", но их можно привязать к набору дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="7b24d-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="7b24d-107">Если количество людей для отображения больше, чем `show-max` значение, будет добавлено число, указывающее количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="7b24d-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="7b24d-108">Пример</span><span class="sxs-lookup"><span data-stu-id="7b24d-108">Example</span></span>

<span data-ttu-id="7b24d-109">В приведенном ниже примере показана группа людей, отображаемая с помощью `mgt-people` компонента.</span><span class="sxs-lookup"><span data-stu-id="7b24d-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="7b24d-110">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="7b24d-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="7b24d-111">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="7b24d-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="7b24d-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b24d-112">Properties</span></span>

<span data-ttu-id="7b24d-113">По умолчанию `mgt-people` компонент получает события от `/me/people` конечной точки с `personType/class eq 'Person'` фильтром для отображения часто обращенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b24d-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="7b24d-114">Для изменения этого поведения можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="7b24d-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="7b24d-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="7b24d-115">Attribute</span></span> | <span data-ttu-id="7b24d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b24d-116">Property</span></span> | <span data-ttu-id="7b24d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7b24d-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="7b24d-118">Show — Max</span><span class="sxs-lookup"><span data-stu-id="7b24d-118">show-max</span></span> | <span data-ttu-id="7b24d-119">шовмакс</span><span class="sxs-lookup"><span data-stu-id="7b24d-119">showMax</span></span> | <span data-ttu-id="7b24d-120">Указывает максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="7b24d-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="7b24d-121">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="7b24d-121">Default value is 3.</span></span> |
| <span data-ttu-id="7b24d-122">people</span><span class="sxs-lookup"><span data-stu-id="7b24d-122">people</span></span> | <span data-ttu-id="7b24d-123">people</span><span class="sxs-lookup"><span data-stu-id="7b24d-123">people</span></span> | <span data-ttu-id="7b24d-124">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="7b24d-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="7b24d-125">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="7b24d-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="7b24d-126">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b24d-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="7b24d-127">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="7b24d-127">group-id</span></span> | <span data-ttu-id="7b24d-128">groupId</span><span class="sxs-lookup"><span data-stu-id="7b24d-128">groupId</span></span> | <span data-ttu-id="7b24d-129">Извлекает пользователей из определенного идентификатора Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7b24d-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="7b24d-130">идентификаторы пользователей</span><span class="sxs-lookup"><span data-stu-id="7b24d-130">user-ids</span></span> | <span data-ttu-id="7b24d-131">userIds</span><span class="sxs-lookup"><span data-stu-id="7b24d-131">userIds</span></span> | <span data-ttu-id="7b24d-132">При наличии массива пользователей `ids`Microsoft Graph компонент будет отображать этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b24d-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="7b24d-133">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="7b24d-133">person-card</span></span> | <span data-ttu-id="7b24d-134">персонкард</span><span class="sxs-lookup"><span data-stu-id="7b24d-134">personCard</span></span> | <span data-ttu-id="7b24d-135">Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели.</span><span class="sxs-lookup"><span data-stu-id="7b24d-135">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="7b24d-136">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="7b24d-136">Default value is `none`.</span></span> |


<span data-ttu-id="7b24d-137">В приведенном ниже примере задается максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="7b24d-137">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="7b24d-138">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="7b24d-138">CSS custom properties</span></span>

<span data-ttu-id="7b24d-139">`mgt-people` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="7b24d-139">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="7b24d-140">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="7b24d-140">Templates</span></span>

<span data-ttu-id="7b24d-141">`mgt-people` Поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="7b24d-141">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="7b24d-142">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="7b24d-142">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="7b24d-143">Тип данных</span><span class="sxs-lookup"><span data-stu-id="7b24d-143">Data type</span></span> | <span data-ttu-id="7b24d-144">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="7b24d-144">Data context</span></span> | <span data-ttu-id="7b24d-145">Описание</span><span class="sxs-lookup"><span data-stu-id="7b24d-145">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="7b24d-146">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="7b24d-146">`people`: list of person objects</span></span> | <span data-ttu-id="7b24d-147">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="7b24d-147">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="7b24d-148">`person`: объект Person</span><span class="sxs-lookup"><span data-stu-id="7b24d-148">`person`: person object</span></span> | <span data-ttu-id="7b24d-149">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b24d-149">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="7b24d-150">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="7b24d-150">`people`: list of person objects</span></span> <br> <span data-ttu-id="7b24d-151">`max`: количество показанных пользователей</span><span class="sxs-lookup"><span data-stu-id="7b24d-151">`max`: number of shown people</span></span> <br> <span data-ttu-id="7b24d-152">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="7b24d-152">`extra`: number of extra people</span></span> | <span data-ttu-id="7b24d-153">Шаблон, используемый для отображения числа за пределами максимального значения справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="7b24d-153">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="7b24d-154">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="7b24d-154">No data context is passed</span></span> | <span data-ttu-id="7b24d-155">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="7b24d-155">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="7b24d-156">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="7b24d-156">No data context is passed</span></span> | <span data-ttu-id="7b24d-157">Шаблон, используемый при загрузке состояния компонента.</span><span class="sxs-lookup"><span data-stu-id="7b24d-157">The template used while the component loads state.</span></span>

<span data-ttu-id="7b24d-158">В приведенных ниже примерах показано, `person` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="7b24d-158">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="7b24d-159">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7b24d-159">Microsoft Graph permissions</span></span>

<span data-ttu-id="7b24d-160">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="7b24d-160">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="7b24d-161">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7b24d-161">Resource</span></span> | <span data-ttu-id="7b24d-162">Разрешение</span><span class="sxs-lookup"><span data-stu-id="7b24d-162">Permission</span></span> |
| - | - |
| [<span data-ttu-id="7b24d-163">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="7b24d-163">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="7b24d-164">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="7b24d-164">Authentication</span></span>

<span data-ttu-id="7b24d-165">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="7b24d-165">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="7b24d-166">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="7b24d-166">Extend for more control</span></span>

<span data-ttu-id="7b24d-167">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="7b24d-167">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="7b24d-168">Метод</span><span class="sxs-lookup"><span data-stu-id="7b24d-168">Method</span></span> | <span data-ttu-id="7b24d-169">Описание</span><span class="sxs-lookup"><span data-stu-id="7b24d-169">Description</span></span> |
| - | - |
| <span data-ttu-id="7b24d-170">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="7b24d-170">renderLoading</span></span> | <span data-ttu-id="7b24d-171">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="7b24d-171">Renders the loading state.</span></span> |
| <span data-ttu-id="7b24d-172">рендернодата</span><span class="sxs-lookup"><span data-stu-id="7b24d-172">renderNoData</span></span> | <span data-ttu-id="7b24d-173">Отрисовывает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="7b24d-173">Renders the empty data state.</span></span> |
| <span data-ttu-id="7b24d-174">рендерпеопле</span><span class="sxs-lookup"><span data-stu-id="7b24d-174">renderPeople</span></span> | <span data-ttu-id="7b24d-175">Отрисовывает список людей вплоть до `show-max` значения.</span><span class="sxs-lookup"><span data-stu-id="7b24d-175">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="7b24d-176">рендерперсон</span><span class="sxs-lookup"><span data-stu-id="7b24d-176">renderPerson</span></span> | <span data-ttu-id="7b24d-177">Отрисовывает отдельного человека.</span><span class="sxs-lookup"><span data-stu-id="7b24d-177">Renders an individual person.</span></span> |
| <span data-ttu-id="7b24d-178">рендероверфлов</span><span class="sxs-lookup"><span data-stu-id="7b24d-178">renderOverflow</span></span> | <span data-ttu-id="7b24d-179">Отрисовывает представление оставшихся пользователей за пределами `show-max` значения.</span><span class="sxs-lookup"><span data-stu-id="7b24d-179">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
