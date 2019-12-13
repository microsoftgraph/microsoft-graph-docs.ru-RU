---
title: Компонент "люди" в наборе инструментов Microsoft Graph
description: Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5f85f0a72e8658a8fc734728ae76d79157da39de
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955878"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="cf066-103">Компонент "люди" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cf066-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cf066-104">Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="cf066-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="cf066-105">По умолчанию отображаются наиболее часто используемые контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="cf066-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="cf066-106">Этот компонент использует несколько элементов управления " [центр](./person.md) управления", но их можно привязать к набору дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="cf066-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="cf066-107">Если количество людей для отображения больше, чем `show-max` значение, будет добавлено число, указывающее количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="cf066-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="cf066-108">Пример</span><span class="sxs-lookup"><span data-stu-id="cf066-108">Example</span></span>

[<span data-ttu-id="cf066-109">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="cf066-109">jsfiddle example</span></span>](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![упр. польз.](./images/mgt-people.png)

## <a name="properties"></a><span data-ttu-id="cf066-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf066-111">Properties</span></span>

<span data-ttu-id="cf066-112">По умолчанию `mgt-people` компонент получает события от `/me/people` конечной точки с `personType/class eq 'Person'` фильтром для отображения часто обращенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="cf066-112">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="cf066-113">Для изменения этого поведения можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="cf066-113">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="cf066-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="cf066-114">Attribute</span></span> | <span data-ttu-id="cf066-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf066-115">Property</span></span> | <span data-ttu-id="cf066-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cf066-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="cf066-117">Show — Max</span><span class="sxs-lookup"><span data-stu-id="cf066-117">show-max</span></span> | <span data-ttu-id="cf066-118">шовмакс</span><span class="sxs-lookup"><span data-stu-id="cf066-118">showMax</span></span> | <span data-ttu-id="cf066-119">Указывает максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="cf066-119">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="cf066-120">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="cf066-120">Default value is 3.</span></span> |
| <span data-ttu-id="cf066-121">people</span><span class="sxs-lookup"><span data-stu-id="cf066-121">people</span></span> | <span data-ttu-id="cf066-122">people</span><span class="sxs-lookup"><span data-stu-id="cf066-122">people</span></span> | <span data-ttu-id="cf066-123">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="cf066-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="cf066-124">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="cf066-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="cf066-125">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="cf066-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="cf066-126">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="cf066-126">group-id</span></span> | <span data-ttu-id="cf066-127">groupId</span><span class="sxs-lookup"><span data-stu-id="cf066-127">groupId</span></span> | <span data-ttu-id="cf066-128">Извлекает пользователей из определенного идентификатора Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cf066-128">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="cf066-129">идентификаторы пользователей</span><span class="sxs-lookup"><span data-stu-id="cf066-129">user-ids</span></span> | <span data-ttu-id="cf066-130">userIds</span><span class="sxs-lookup"><span data-stu-id="cf066-130">userIds</span></span> | <span data-ttu-id="cf066-131">При наличии массива пользователей `ids`Microsoft Graph компонент будет отображать этих пользователей.</span><span class="sxs-lookup"><span data-stu-id="cf066-131">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="cf066-132">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="cf066-132">person-card</span></span> | <span data-ttu-id="cf066-133">персонкард</span><span class="sxs-lookup"><span data-stu-id="cf066-133">personCard</span></span> | <span data-ttu-id="cf066-134">Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели.</span><span class="sxs-lookup"><span data-stu-id="cf066-134">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="cf066-135">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="cf066-135">Default value is `none`.</span></span> |


<span data-ttu-id="cf066-136">В приведенном ниже примере задается максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="cf066-136">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="cf066-137">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="cf066-137">CSS custom properties</span></span>

<span data-ttu-id="cf066-138">`mgt-people` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="cf066-138">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="cf066-139">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="cf066-139">Templates</span></span>

<span data-ttu-id="cf066-140">`mgt-people` Поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="cf066-140">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="cf066-141">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="cf066-141">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="cf066-142">Тип данных</span><span class="sxs-lookup"><span data-stu-id="cf066-142">Data type</span></span> | <span data-ttu-id="cf066-143">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="cf066-143">Data context</span></span> | <span data-ttu-id="cf066-144">Описание</span><span class="sxs-lookup"><span data-stu-id="cf066-144">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="cf066-145">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="cf066-145">`people`: list of person objects</span></span> | <span data-ttu-id="cf066-146">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="cf066-146">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="cf066-147">`person`: объект Person</span><span class="sxs-lookup"><span data-stu-id="cf066-147">`person`: person object</span></span> | <span data-ttu-id="cf066-148">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cf066-148">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="cf066-149">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="cf066-149">`people`: list of person objects</span></span> <br> <span data-ttu-id="cf066-150">`max`: количество показанных пользователей</span><span class="sxs-lookup"><span data-stu-id="cf066-150">`max`: number of shown people</span></span> <br> <span data-ttu-id="cf066-151">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="cf066-151">`extra`: number of extra people</span></span> | <span data-ttu-id="cf066-152">Шаблон, используемый для отображения числа за пределами максимального значения справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="cf066-152">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="cf066-153">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="cf066-153">No data context is passed</span></span> | <span data-ttu-id="cf066-154">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="cf066-154">The template used when no data is available.</span></span> |

<span data-ttu-id="cf066-155">В приведенных ниже примерах показано, `person` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="cf066-155">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="cf066-156">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cf066-156">Microsoft Graph permissions</span></span>

<span data-ttu-id="cf066-157">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="cf066-157">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="cf066-158">Resource</span><span class="sxs-lookup"><span data-stu-id="cf066-158">Resource</span></span> | <span data-ttu-id="cf066-159">Разрешение</span><span class="sxs-lookup"><span data-stu-id="cf066-159">Permission</span></span> |
| - | - |
| [<span data-ttu-id="cf066-160">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="cf066-160">/me/people</span></span>](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="cf066-161">People.Read</span><span class="sxs-lookup"><span data-stu-id="cf066-161">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="cf066-162">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="cf066-162">Authentication</span></span>

<span data-ttu-id="cf066-163">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="cf066-163">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
