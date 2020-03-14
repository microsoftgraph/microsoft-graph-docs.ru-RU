---
title: Компонент "люди" в наборе инструментов Microsoft Graph
description: Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 78dc1504d7f46756809abcf922dfcea431fd796c
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639963"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="770f8-103">Компонент "люди" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="770f8-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="770f8-104">Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="770f8-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="770f8-105">По умолчанию отображаются наиболее часто используемые контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="770f8-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="770f8-106">Этот компонент использует несколько элементов управления " [центр](./person.md) управления", но их можно привязать к набору дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="770f8-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="770f8-107">Если количество людей для отображения больше, чем `show-max` значение, будет добавлено число, указывающее количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="770f8-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="770f8-108">Пример</span><span class="sxs-lookup"><span data-stu-id="770f8-108">Example</span></span>

<span data-ttu-id="770f8-109">В приведенном ниже примере показана группа людей, отображаемая с помощью `mgt-people` компонента.</span><span class="sxs-lookup"><span data-stu-id="770f8-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="770f8-110">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="770f8-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="770f8-111">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="770f8-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="770f8-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="770f8-112">Properties</span></span>

<span data-ttu-id="770f8-113">По умолчанию `mgt-people` компонент получает события от `/me/people` конечной точки с `personType/class eq 'Person'` фильтром для отображения часто обращенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="770f8-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="770f8-114">Для изменения этого поведения можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="770f8-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="770f8-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="770f8-115">Attribute</span></span> | <span data-ttu-id="770f8-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="770f8-116">Property</span></span> | <span data-ttu-id="770f8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="770f8-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="770f8-118">Show — Max</span><span class="sxs-lookup"><span data-stu-id="770f8-118">show-max</span></span> | <span data-ttu-id="770f8-119">шовмакс</span><span class="sxs-lookup"><span data-stu-id="770f8-119">showMax</span></span> | <span data-ttu-id="770f8-120">Указывает максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="770f8-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="770f8-121">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="770f8-121">Default value is 3.</span></span> |
| <span data-ttu-id="770f8-122">people</span><span class="sxs-lookup"><span data-stu-id="770f8-122">people</span></span> | <span data-ttu-id="770f8-123">people</span><span class="sxs-lookup"><span data-stu-id="770f8-123">people</span></span> | <span data-ttu-id="770f8-124">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="770f8-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="770f8-125">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="770f8-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="770f8-126">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="770f8-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="770f8-127">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="770f8-127">group-id</span></span> | <span data-ttu-id="770f8-128">groupId</span><span class="sxs-lookup"><span data-stu-id="770f8-128">groupId</span></span> | <span data-ttu-id="770f8-129">Извлекает пользователей из определенного идентификатора Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="770f8-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="770f8-130">идентификаторы пользователей</span><span class="sxs-lookup"><span data-stu-id="770f8-130">user-ids</span></span> | <span data-ttu-id="770f8-131">userIds</span><span class="sxs-lookup"><span data-stu-id="770f8-131">userIds</span></span> | <span data-ttu-id="770f8-132">При наличии массива пользователей `ids`Microsoft Graph компонент будет отображать этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="770f8-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="770f8-133">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="770f8-133">person-card</span></span> | <span data-ttu-id="770f8-134">персонкард</span><span class="sxs-lookup"><span data-stu-id="770f8-134">personCard</span></span> | <span data-ttu-id="770f8-135">Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели.</span><span class="sxs-lookup"><span data-stu-id="770f8-135">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="770f8-136">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="770f8-136">Default value is `none`.</span></span> |


<span data-ttu-id="770f8-137">В приведенном ниже примере задается максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="770f8-137">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="770f8-138">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="770f8-138">CSS custom properties</span></span>

<span data-ttu-id="770f8-139">`mgt-people` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="770f8-139">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="770f8-140">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="770f8-140">Templates</span></span>

<span data-ttu-id="770f8-141">`mgt-people` Поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="770f8-141">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="770f8-142">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="770f8-142">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="770f8-143">Тип данных</span><span class="sxs-lookup"><span data-stu-id="770f8-143">Data type</span></span> | <span data-ttu-id="770f8-144">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="770f8-144">Data context</span></span> | <span data-ttu-id="770f8-145">Описание</span><span class="sxs-lookup"><span data-stu-id="770f8-145">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="770f8-146">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="770f8-146">`people`: list of person objects</span></span> | <span data-ttu-id="770f8-147">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="770f8-147">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="770f8-148">`person`: объект Person</span><span class="sxs-lookup"><span data-stu-id="770f8-148">`person`: person object</span></span> | <span data-ttu-id="770f8-149">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="770f8-149">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="770f8-150">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="770f8-150">`people`: list of person objects</span></span> <br> <span data-ttu-id="770f8-151">`max`: количество показанных пользователей</span><span class="sxs-lookup"><span data-stu-id="770f8-151">`max`: number of shown people</span></span> <br> <span data-ttu-id="770f8-152">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="770f8-152">`extra`: number of extra people</span></span> | <span data-ttu-id="770f8-153">Шаблон, используемый для отображения числа за пределами максимального значения справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="770f8-153">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="770f8-154">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="770f8-154">No data context is passed</span></span> | <span data-ttu-id="770f8-155">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="770f8-155">The template used when no data is available.</span></span> |

<span data-ttu-id="770f8-156">В приведенных ниже примерах показано, `person` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="770f8-156">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="770f8-157">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="770f8-157">Microsoft Graph permissions</span></span>

<span data-ttu-id="770f8-158">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="770f8-158">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="770f8-159">Resource</span><span class="sxs-lookup"><span data-stu-id="770f8-159">Resource</span></span> | <span data-ttu-id="770f8-160">Разрешение</span><span class="sxs-lookup"><span data-stu-id="770f8-160">Permission</span></span> |
| - | - |
| [<span data-ttu-id="770f8-161">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="770f8-161">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="770f8-162">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="770f8-162">Authentication</span></span>

<span data-ttu-id="770f8-163">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="770f8-163">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
