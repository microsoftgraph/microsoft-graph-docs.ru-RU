---
title: Рекомендации по работе с API OneNote в Microsoft Graph
description: В этой статье содержатся рекомендации по работе с API OneNote в Microsoft Graph. Эти рекомендации основаны на ответах на распространенные вопросы в Microsoft Q&a и Twitter.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8ceb848e4d48954d9a08c8bc9f7b28e2521c9aed
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472806"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a><span data-ttu-id="13607-104">Рекомендации по работе с API OneNote в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="13607-104">Best practices for working with the OneNote API in Microsoft Graph</span></span>

<span data-ttu-id="13607-105">В этой статье содержатся рекомендации по работе с API OneNote в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="13607-105">This article provides recommendations for working with the OneNote APIs in Microsoft Graph.</span></span> <span data-ttu-id="13607-106">Эти рекомендации основаны на ответах на распространенные вопросы в [Microsoft Q&a и](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)  Twitter.</span><span class="sxs-lookup"><span data-stu-id="13607-106">These recommendations are based on answers to common questions on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)  and Twitter.</span></span>

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a><span data-ttu-id="13607-107">Используйте оператор $select, чтобы выбрать минимальный набор необходимых свойств</span><span class="sxs-lookup"><span data-stu-id="13607-107">Use $select to select the minimum set of properties you need</span></span>

<span data-ttu-id="13607-108">Если вам необходимо отправить запрос к ресурсу (например, к разделам в записной книжке), создайте запрос, аналогичный указанному ниже.</span><span class="sxs-lookup"><span data-stu-id="13607-108">When you query for a resource (for example, sections inside a notebook), you make a request similar to the following.</span></span>

```http
GET ~/notebooks/{id}/sections
```

<span data-ttu-id="13607-109">С его помощью можно получить все свойства разделов.</span><span class="sxs-lookup"><span data-stu-id="13607-109">This retrieves all the properties of the sections.</span></span> <span data-ttu-id="13607-110">Возможно, вам нужны не все свойства.</span><span class="sxs-lookup"><span data-stu-id="13607-110">However, you might not need all properties.</span></span> <span data-ttu-id="13607-111">Вы можете использовать параметр запроса `$select`, чтобы возвращать только необходимые вам свойства, как показано в примере ниже.</span><span class="sxs-lookup"><span data-stu-id="13607-111">You can use the `$select` query parameter to return just the properties that you want, as shown in the following example.</span></span>

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

<span data-ttu-id="13607-112">Такой же подход применяется к другим API OneNote.</span><span class="sxs-lookup"><span data-stu-id="13607-112">The same approach applies to other OneNote APIs.</span></span>

## <a name="use-expand-instead-of-making-multiple-api-calls"></a><span data-ttu-id="13607-113">Вместо нескольких запросов к API используйте оператор $expand</span><span class="sxs-lookup"><span data-stu-id="13607-113">Use $expand instead of making multiple API calls</span></span>

<span data-ttu-id="13607-114">Предположим, вы хотите получить все записные книжки, разделы и группы разделов пользователя в виде иерархического представления.</span><span class="sxs-lookup"><span data-stu-id="13607-114">Suppose you want to retrieve all of the user’s notebooks, sections, and section groups in a hierarchical view.</span></span> <span data-ttu-id="13607-115">Это можно сделать следующим образом:</span><span class="sxs-lookup"><span data-stu-id="13607-115">You might accomplish that by doing the following:</span></span>

* <span data-ttu-id="13607-116">Совершите вызов `GET ~/notebooks`, чтобы получить список записных книжек.</span><span class="sxs-lookup"><span data-stu-id="13607-116">Call `GET ~/notebooks` to get the list of notebooks.</span></span>

* <span data-ttu-id="13607-117">Для каждой полученной записной книжки совершите вызов `GET ~/notebooks/{notebookId}/sections`, чтобы получить список разделов в ней.</span><span class="sxs-lookup"><span data-stu-id="13607-117">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sections` to retrieve the list of sections.</span></span>

* <span data-ttu-id="13607-118">Для каждой полученной записной книжки совершите вызов `GET ~/notebooks/{notebookId}/sectionGroups`, чтобы получить список групп разделов в ней.</span><span class="sxs-lookup"><span data-stu-id="13607-118">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sectionGroups` to retrieve the list of section groups.</span></span>

* <span data-ttu-id="13607-119">При необходимости выполните рекурсивные итерации в группах разделов.</span><span class="sxs-lookup"><span data-stu-id="13607-119">Optionally recursively iterate through section groups.</span></span>

<span data-ttu-id="13607-120">Несмотря на то что это будет работать (с несколькими дополнительными последовательными циклическими обращениями к службе), лучше использовать параметр запроса `$expand`.</span><span class="sxs-lookup"><span data-stu-id="13607-120">While this will work (with a few extra sequential roundtrips to the service), a better approach is to use the `$expand` query parameter.</span></span> 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

<span data-ttu-id="13607-121">Он даст те же результаты за одно циклическое обращение по сети, но с более высокой производительностью.</span><span class="sxs-lookup"><span data-stu-id="13607-121">This will yield the same results in one network roundtrip, with better performance.</span></span>

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a><span data-ttu-id="13607-122">При получении всех страниц для пользователя выполните эти действия отдельно для каждого раздела</span><span class="sxs-lookup"><span data-stu-id="13607-122">When getting all pages for a user, do so for each section separately</span></span>

<span data-ttu-id="13607-123">Несмотря на то что Microsoft Graph предоставляет конечную точку для получения всех страниц, это не лучший способ получить все страницы, к которым у пользователя есть доступ.</span><span class="sxs-lookup"><span data-stu-id="13607-123">While Microsoft Graph exposes an endpoint to retrieve all pages, this isn't the best way to get all the pages the user has access to.</span></span> <span data-ttu-id="13607-124">Если у пользователя слишком много разделов, это может привести к задержкам или снижению производительности.</span><span class="sxs-lookup"><span data-stu-id="13607-124">When the user has too many sections, this can lead to timeouts or bad performance.</span></span> <span data-ttu-id="13607-125">Лучше выполнять итерации для каждого раздела, получая страницы отдельно для каждого раздела.</span><span class="sxs-lookup"><span data-stu-id="13607-125">It is better to iterate each section, getting pages for each one separately.</span></span>

<span data-ttu-id="13607-126">Например, вместо использования этого вызова (это постраничный API, поэтому вам не удастся получить все страницы за один раз):</span><span class="sxs-lookup"><span data-stu-id="13607-126">For example, instead of using this call (this API is paged, so you won't be able to fetch the pages all at once):</span></span>

```http
GET ~/pages
```

<span data-ttu-id="13607-127">Лучше несколько раз использовать следующий вызов (особенно если вам не нужны все разделы):</span><span class="sxs-lookup"><span data-stu-id="13607-127">It is better to use the following call several times (especially if you don't need all sections):</span></span>

```http
GET ~/sections/{id}/pages
```

<span data-ttu-id="13607-128">При получении метаданных страницы переопределите способ упорядочивания `lastModifiedDateTime`, используемый по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="13607-128">When getting page metadata, override the default `lastModifiedDateTime` ordering.</span></span> <span data-ttu-id="13607-129">Страницы можно получить быстрее, если не нужно сортировать их по `lastModifiedDateTime`.</span><span class="sxs-lookup"><span data-stu-id="13607-129">It is faster to get pages when you don't have to sort them by `lastModifiedDateTime`.</span></span> <span data-ttu-id="13607-130">Для этого вы можете выполнить сортировку по любому другому свойству. Пример:</span><span class="sxs-lookup"><span data-stu-id="13607-130">To do this, you can sort by any other property; for example:</span></span>

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
