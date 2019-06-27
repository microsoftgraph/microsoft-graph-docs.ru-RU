---
title: Компонент "люди" в наборе инструментов Microsoft Graph
description: Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: fcc44262f807d3f10f42e8af8e476975ad262cda
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243090"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="7172a-103">Компонент "люди" в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7172a-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="7172a-104">Вы можете использовать `mgt-people` веб-компонент для отображения группы людей или контактов с помощью фотографий или инициалов.</span><span class="sxs-lookup"><span data-stu-id="7172a-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="7172a-105">По умолчанию отображаются наиболее часто используемые контакты для пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="7172a-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="7172a-106">Этот компонент использует несколько элементов управления " [центр](./person.md) управления", но их можно привязать к набору дескрипторов людей.</span><span class="sxs-lookup"><span data-stu-id="7172a-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="7172a-107">Если количество людей для отображения больше, чем `show-max` значение, будет добавлено число, указывающее количество дополнительных контактов.</span><span class="sxs-lookup"><span data-stu-id="7172a-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="7172a-108">Пример</span><span class="sxs-lookup"><span data-stu-id="7172a-108">Example</span></span>

[<span data-ttu-id="7172a-109">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="7172a-109">jsfiddle example</span></span>](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![упр. польз.](./images/mgt-people.png)

## <a name="properties"></a><span data-ttu-id="7172a-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="7172a-111">Properties</span></span>

<span data-ttu-id="7172a-112">По умолчанию `mgt-people` компонент получает события от `/me/people` конечной точки с `personType/class eq 'Person'` фильтром для отображения часто обращенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7172a-112">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="7172a-113">Для изменения этого поведения можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="7172a-113">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="7172a-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="7172a-114">Property</span></span> | <span data-ttu-id="7172a-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="7172a-115">Attribute</span></span> | <span data-ttu-id="7172a-116">Описание</span><span class="sxs-lookup"><span data-stu-id="7172a-116">Description</span></span> |
| --- | --- | --- |
| `showMax` | `show-max` | <span data-ttu-id="7172a-117">Указывает максимальное количество людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="7172a-117">Indicate the maximum number of people to show.</span></span> <span data-ttu-id="7172a-118">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="7172a-118">Default value is 3.</span></span> |
| `people` | `people` | <span data-ttu-id="7172a-119">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="7172a-119">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="7172a-120">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="7172a-120">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="7172a-121">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7172a-121">Set this value to load your own people.</span></span> |

<span data-ttu-id="7172a-122">В приведенном ниже примере задается максимальное число людей для отображения.</span><span class="sxs-lookup"><span data-stu-id="7172a-122">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="7172a-123">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="7172a-123">CSS custom properties</span></span>

<span data-ttu-id="7172a-124">`mgt-people` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="7172a-124">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="7172a-125">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="7172a-125">Templates</span></span>

<span data-ttu-id="7172a-126">`mgt-people` Поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для замены определенных частей компонента.</span><span class="sxs-lookup"><span data-stu-id="7172a-126">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="7172a-127">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="7172a-127">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="7172a-128">Тип данных</span><span class="sxs-lookup"><span data-stu-id="7172a-128">Data type</span></span> | <span data-ttu-id="7172a-129">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="7172a-129">Data context</span></span> | <span data-ttu-id="7172a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7172a-130">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="7172a-131">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="7172a-131">`people`: list of person objects</span></span> | <span data-ttu-id="7172a-132">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="7172a-132">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="7172a-133">`person`: объект Person</span><span class="sxs-lookup"><span data-stu-id="7172a-133">`person`: person object</span></span> | <span data-ttu-id="7172a-134">Шаблон, используемый для отображения каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7172a-134">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="7172a-135">`people`: список объектов Person</span><span class="sxs-lookup"><span data-stu-id="7172a-135">`people`: list of person objects</span></span> <br> <span data-ttu-id="7172a-136">`max`: количество показанных пользователей</span><span class="sxs-lookup"><span data-stu-id="7172a-136">`max`: number of shown people</span></span> <br> <span data-ttu-id="7172a-137">`extra`: количество дополнительных людей</span><span class="sxs-lookup"><span data-stu-id="7172a-137">`extra`: number of extra people</span></span> | <span data-ttu-id="7172a-138">Шаблон, используемый для отображения числа за пределами максимального значения справа от списка людей.</span><span class="sxs-lookup"><span data-stu-id="7172a-138">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="7172a-139">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="7172a-139">No data context is passed</span></span> | <span data-ttu-id="7172a-140">Шаблон, используемый, если люди недоступны.</span><span class="sxs-lookup"><span data-stu-id="7172a-140">The template used when no people are available.</span></span> |

<span data-ttu-id="7172a-141">В приведенных ниже примерах показано, `person` как использовать шаблон.</span><span class="sxs-lookup"><span data-stu-id="7172a-141">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="7172a-142">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7172a-142">Microsoft Graph permissions</span></span>

<span data-ttu-id="7172a-143">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="7172a-143">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="7172a-144">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7172a-144">Resource</span></span> | <span data-ttu-id="7172a-145">Разрешение или область</span><span class="sxs-lookup"><span data-stu-id="7172a-145">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="7172a-146">/ме/Пеопле</span><span class="sxs-lookup"><span data-stu-id="7172a-146">/me/people</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="7172a-147">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="7172a-147">Authentication</span></span>

<span data-ttu-id="7172a-148">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке](./../providers.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="7172a-148">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
