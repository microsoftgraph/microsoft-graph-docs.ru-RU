---
title: Получение компонента в наборе инструментов Microsoft Graph
description: Компонент Get позволяет создавать любой запрос GET из Microsoft Graph непосредственно в HTML-коде.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 77beb3940eb29a2c9158fba88d78084639e433ed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921704"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="df1a2-103">Получение компонента в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df1a2-103">Get component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="df1a2-104">Вы можете использовать `mgt-get` , чтобы сделать любой запрос GET от Microsoft Graph непосредственно в HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="df1a2-104">You can use `mgt-get` to make any GET query from Microsoft Graph directly in your HTML.</span></span> <span data-ttu-id="df1a2-105">Компонент не предоставляет пользовательский интерфейс по умолчанию и требует написания шаблона.</span><span class="sxs-lookup"><span data-stu-id="df1a2-105">The component does not provide a default UI and requires that you write a template.</span></span>

## <a name="example"></a><span data-ttu-id="df1a2-106">Пример</span><span class="sxs-lookup"><span data-stu-id="df1a2-106">Example</span></span>

```html
<mgt-get resource="/me/messages" version="beta" scopes="mail.read" max-pages="2">
  <template>
    emails: {{value.length}}
  </template>
  <template data-type="loading">
    loading
  </template>
</mgt-get>
```

## <a name="properties-and-attributes"></a><span data-ttu-id="df1a2-107">Свойства и атрибуты</span><span class="sxs-lookup"><span data-stu-id="df1a2-107">Properties and attributes</span></span>

<span data-ttu-id="df1a2-108">Для изменения поведения компонента можно использовать несколько атрибутов.</span><span class="sxs-lookup"><span data-stu-id="df1a2-108">You can use several attributes to change the behavior of the component.</span></span> <span data-ttu-id="df1a2-109">Единственный обязательный атрибут `resource`.</span><span class="sxs-lookup"><span data-stu-id="df1a2-109">The only required attribute is `resource`.</span></span>

| <span data-ttu-id="df1a2-110">Атрибут</span><span class="sxs-lookup"><span data-stu-id="df1a2-110">Attribute</span></span> | <span data-ttu-id="df1a2-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="df1a2-111">Property</span></span>  | <span data-ttu-id="df1a2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="df1a2-112">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="df1a2-113">resource</span><span class="sxs-lookup"><span data-stu-id="df1a2-113">resource</span></span> | <span data-ttu-id="df1a2-114">resource</span><span class="sxs-lookup"><span data-stu-id="df1a2-114">resource</span></span> | <span data-ttu-id="df1a2-115">Ресурс, который требуется получить из Microsoft Graph (например, `/me`).</span><span class="sxs-lookup"><span data-stu-id="df1a2-115">The resource to get from Microsoft Graph (for example, `/me`).</span></span> |
| <span data-ttu-id="df1a2-116">scopes</span><span class="sxs-lookup"><span data-stu-id="df1a2-116">scopes</span></span> | <span data-ttu-id="df1a2-117">scopes</span><span class="sxs-lookup"><span data-stu-id="df1a2-117">scopes</span></span> | <span data-ttu-id="df1a2-118">Необязательный массив строк, если используется свойство или область с разделителями запятые, если используется атрибут.</span><span class="sxs-lookup"><span data-stu-id="df1a2-118">Optional array of strings if using the property or a comma delimited scope if using the attribute.</span></span> <span data-ttu-id="df1a2-119">Компонент будет использовать эти области (с поддерживаемым поставщиком), чтобы убедиться, что пользователь отправил их в нужное разрешение.</span><span class="sxs-lookup"><span data-stu-id="df1a2-119">The component will use these scopes (with a supported provider) to ensure that the user has consented to the right permission.</span></span> |
| <span data-ttu-id="df1a2-120">version</span><span class="sxs-lookup"><span data-stu-id="df1a2-120">version</span></span> | <span data-ttu-id="df1a2-121">version</span><span class="sxs-lookup"><span data-stu-id="df1a2-121">version</span></span> | <span data-ttu-id="df1a2-122">Необязательный версия API, используемая при выполнении запроса GET.</span><span class="sxs-lookup"><span data-stu-id="df1a2-122">Optional API version to use when making the GET request.</span></span> <span data-ttu-id="df1a2-123">Значение по умолчанию: `v1.0`.</span><span class="sxs-lookup"><span data-stu-id="df1a2-123">Default is `v1.0`.</span></span>  |
| <span data-ttu-id="df1a2-124">Максимальное число страниц</span><span class="sxs-lookup"><span data-stu-id="df1a2-124">max-pages</span></span> | <span data-ttu-id="df1a2-125">макспажес</span><span class="sxs-lookup"><span data-stu-id="df1a2-125">maxPages</span></span> | <span data-ttu-id="df1a2-126">Необязательное количество страниц (для ресурсов, поддерживающих разбиение по страницам).</span><span class="sxs-lookup"><span data-stu-id="df1a2-126">Optional number of pages (for resources that support paging).</span></span> <span data-ttu-id="df1a2-127">Значение по умолчанию — 3.</span><span class="sxs-lookup"><span data-stu-id="df1a2-127">Default is 3.</span></span> <span data-ttu-id="df1a2-128">Если задать для этого параметра значение 0, будут получены все страницы.</span><span class="sxs-lookup"><span data-stu-id="df1a2-128">Setting this value to 0 will get all pages.</span></span>  |
| <span data-ttu-id="df1a2-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="df1a2-129">N/A</span></span> | <span data-ttu-id="df1a2-130">response</span><span class="sxs-lookup"><span data-stu-id="df1a2-130">response</span></span> | <span data-ttu-id="df1a2-131">Отклик только для чтения от Microsoft Graph, если запрос был успешным.</span><span class="sxs-lookup"><span data-stu-id="df1a2-131">Read-only response from Microsoft Graph if request was successful.</span></span>  |
| <span data-ttu-id="df1a2-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="df1a2-132">N/A</span></span> |<span data-ttu-id="df1a2-133">error</span><span class="sxs-lookup"><span data-stu-id="df1a2-133">error</span></span>| <span data-ttu-id="df1a2-134">Ошибка, доступная только для чтения, из Microsoft Graph, если запрос завершился неудачно.</span><span class="sxs-lookup"><span data-stu-id="df1a2-134">Read-only error from Microsoft Graph if request was not successful.</span></span> |

## <a name="events"></a><span data-ttu-id="df1a2-135">События</span><span class="sxs-lookup"><span data-stu-id="df1a2-135">Events</span></span>
| <span data-ttu-id="df1a2-136">Событие</span><span class="sxs-lookup"><span data-stu-id="df1a2-136">Event</span></span> | <span data-ttu-id="df1a2-137">Detail (Сведения)</span><span class="sxs-lookup"><span data-stu-id="df1a2-137">Detail</span></span> | <span data-ttu-id="df1a2-138">Описание</span><span class="sxs-lookup"><span data-stu-id="df1a2-138">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="df1a2-139">dataChange</span><span class="sxs-lookup"><span data-stu-id="df1a2-139">dataChange</span></span> | <span data-ttu-id="df1a2-140">Сведения содержит объекты `response` и `error` .</span><span class="sxs-lookup"><span data-stu-id="df1a2-140">The detail contains the `response` and `error` objects.</span></span> | <span data-ttu-id="df1a2-141">Возникает при изменении ответа или ошибки.</span><span class="sxs-lookup"><span data-stu-id="df1a2-141">Fired when the response or error change.</span></span> |

## <a name="templates"></a><span data-ttu-id="df1a2-142">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="df1a2-142">Templates</span></span>

<span data-ttu-id="df1a2-143">`mgt-get` Компонент поддерживает несколько [шаблонов](../templates.md) , которые можно использовать для определения внешнего вида и функций.</span><span class="sxs-lookup"><span data-stu-id="df1a2-143">The `mgt-get` component supports several [templates](../templates.md) that you can use to define the look and feel.</span></span> <span data-ttu-id="df1a2-144">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="df1a2-144">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="df1a2-145">Тип данных</span><span class="sxs-lookup"><span data-stu-id="df1a2-145">Data type</span></span> | <span data-ttu-id="df1a2-146">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="df1a2-146">Data context</span></span> | <span data-ttu-id="df1a2-147">Описание</span><span class="sxs-lookup"><span data-stu-id="df1a2-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="df1a2-148">умолчани</span><span class="sxs-lookup"><span data-stu-id="df1a2-148">default</span></span> | <span data-ttu-id="df1a2-149">Отклик от Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="df1a2-149">The response from Microsoft Graph.</span></span> | <span data-ttu-id="df1a2-150">Для отображения данных, поступающих из Microsoft Graph, необходим шаблон по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="df1a2-150">The default template is required to render the data coming from Microsoft Graph.</span></span> |
| <span data-ttu-id="df1a2-151">error</span><span class="sxs-lookup"><span data-stu-id="df1a2-151">error</span></span> | <span data-ttu-id="df1a2-152">Ошибка в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="df1a2-152">The error from Microsoft Graph.</span></span> | <span data-ttu-id="df1a2-153">Этот шаблон будет использоваться, если при выполнении запроса возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="df1a2-153">This template will be used if there is an error making the request.</span></span> |
| <span data-ttu-id="df1a2-154">загрузки</span><span class="sxs-lookup"><span data-stu-id="df1a2-154">loading</span></span> | <span data-ttu-id="df1a2-155">Н/Д</span><span class="sxs-lookup"><span data-stu-id="df1a2-155">N/A</span></span> | <span data-ttu-id="df1a2-156">Этот шаблон используется, пока выполняется запрос.</span><span class="sxs-lookup"><span data-stu-id="df1a2-156">This template is used while the request is being made.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="df1a2-157">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df1a2-157">Microsoft Graph permissions</span></span>

<span data-ttu-id="df1a2-158">Для получения дополнительных сведений о разрешениях обратитесь к разделу " [Справка по разрешениям](https://docs.microsoft.com/graph/permissions-reference)Microsoft Graph".</span><span class="sxs-lookup"><span data-stu-id="df1a2-158">For more information about permissions, see the Microsoft Graph [permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span> 

## <a name="authentication"></a><span data-ttu-id="df1a2-159">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="df1a2-159">Authentication</span></span>

<span data-ttu-id="df1a2-160">Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке подлинности](./../providers.md) .</span><span class="sxs-lookup"><span data-stu-id="df1a2-160">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
