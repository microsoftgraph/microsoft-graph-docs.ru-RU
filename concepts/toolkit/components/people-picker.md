---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 2a0680a70ddfd5410e82911e5280c0b1a7e7dcaf
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822797"
---
# <a name="people-picker-component"></a><span data-ttu-id="f99ce-103">Компонент "Выбор людей"</span><span class="sxs-lookup"><span data-stu-id="f99ce-103">People-Picker component</span></span>

<span data-ttu-id="f99ce-104">Вы можете использовать поиск `mgt-people-picker` в веб-компоненте для указанного числа людей и отобразить список результатов с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f99ce-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="f99ce-105">По умолчанию компонент будет выполнять поиск всех пользователей; Кроме того, можно определить свойство Group, чтобы отфильтровать результаты.</span><span class="sxs-lookup"><span data-stu-id="f99ce-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="f99ce-106">Если количество отображаемых людей превышает `show-max` значение, в списке поиска будут отображаться не все возвращенные пользователи.</span><span class="sxs-lookup"><span data-stu-id="f99ce-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="f99ce-107">Пример</span><span class="sxs-lookup"><span data-stu-id="f99ce-107">Example</span></span>

[<span data-ttu-id="f99ce-108">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="f99ce-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![Центр управления "Выбор людей"](./images/mgt-people-picker-image.png)

## <a name="properties"></a><span data-ttu-id="f99ce-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f99ce-110">Properties</span></span>

<span data-ttu-id="f99ce-111">По умолчанию `mgt-people-picker` компонент получает события от `/me/people` конечной точки.</span><span class="sxs-lookup"><span data-stu-id="f99ce-111">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="f99ce-112">Используйте следующие атрибуты, чтобы изменить это поведение.</span><span class="sxs-lookup"><span data-stu-id="f99ce-112">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="f99ce-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="f99ce-113">Property</span></span> | <span data-ttu-id="f99ce-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="f99ce-114">Attribute</span></span> | <span data-ttu-id="f99ce-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f99ce-115">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f99ce-116">шовмакс</span><span class="sxs-lookup"><span data-stu-id="f99ce-116">showMax</span></span>  | <span data-ttu-id="f99ce-117">Show — Max</span><span class="sxs-lookup"><span data-stu-id="f99ce-117">show-max</span></span>  | <span data-ttu-id="f99ce-118">Целое значение, указывающее максимальное число отображаемых людей.</span><span class="sxs-lookup"><span data-stu-id="f99ce-118">An integer value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="f99ce-119">значение по умолчанию — 6.</span><span class="sxs-lookup"><span data-stu-id="f99ce-119">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="f99ce-120">people</span><span class="sxs-lookup"><span data-stu-id="f99ce-120">people</span></span>   | <span data-ttu-id="f99ce-121">people</span><span class="sxs-lookup"><span data-stu-id="f99ce-121">people</span></span>    | <span data-ttu-id="f99ce-122">Массив пользователей, который получает или задает список людей, отображаемых компонентом.</span><span class="sxs-lookup"><span data-stu-id="f99ce-122">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="f99ce-123">Используйте это свойство для доступа к пользователям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="f99ce-123">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="f99ce-124">Присвойте этому параметру значение загрузка собственных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f99ce-124">Set this value to load your own people.</span></span> |
| <span data-ttu-id="f99ce-125">group</span><span class="sxs-lookup"><span data-stu-id="f99ce-125">group</span></span>    | <span data-ttu-id="f99ce-126">group</span><span class="sxs-lookup"><span data-stu-id="f99ce-126">group</span></span>     | <span data-ttu-id="f99ce-127">Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="f99ce-127">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |

<span data-ttu-id="f99ce-128">Ниже приведен пример.</span><span class="sxs-lookup"><span data-stu-id="f99ce-128">The following is an example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="css-custom-properties"></a><span data-ttu-id="f99ce-129">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="f99ce-129">CSS custom properties</span></span>

<span data-ttu-id="f99ce-130">`mgt-people-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="f99ce-130">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f99ce-131">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f99ce-131">Microsoft Graph permissions</span></span>

<span data-ttu-id="f99ce-132">Этот компонент использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f99ce-132">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="f99ce-133">API</span><span class="sxs-lookup"><span data-stu-id="f99ce-133">API</span></span>                                                                                                              | <span data-ttu-id="f99ce-134">Разрешение</span><span class="sxs-lookup"><span data-stu-id="f99ce-134">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="f99ce-135">/ме/пеопле</span><span class="sxs-lookup"><span data-stu-id="f99ce-135">/me/people</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="f99ce-136">People.Read</span><span class="sxs-lookup"><span data-stu-id="f99ce-136">People.Read</span></span> |
| [<span data-ttu-id="f99ce-137">/граупс/\${groupId}/мемберс</span><span class="sxs-lookup"><span data-stu-id="f99ce-137">/groups/\${groupId}/members</span></span>](https://docs.microsoft.com/en-us/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="f99ce-138">People.Read</span><span class="sxs-lookup"><span data-stu-id="f99ce-138">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="f99ce-139">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="f99ce-139">Authentication</span></span>

<span data-ttu-id="f99ce-140">Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="f99ce-140">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
