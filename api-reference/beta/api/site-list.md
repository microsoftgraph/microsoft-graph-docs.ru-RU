---
title: Перечисление сайтов
description: Перечислите доступные [сайты] [] в Организации, которые совпадают с предоставленными критериями фильтра и параметрами запроса.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: ''
ms.openlocfilehash: 0cf51ec84ae506935d30c5e3d1722a1b26a9f1aa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409994"
---
# <a name="enumerate-sites"></a><span data-ttu-id="04e7f-103">Перечисление сайтов</span><span class="sxs-lookup"><span data-stu-id="04e7f-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04e7f-104">Список доступных [сайтов][] в Организации, которые отвечают предоставленным условиям фильтра и параметрам запроса.</span><span class="sxs-lookup"><span data-stu-id="04e7f-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="04e7f-105">В настоящее время поддерживаются только следующие параметры запросов:</span><span class="sxs-lookup"><span data-stu-id="04e7f-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="04e7f-106">Оператор Filter</span><span class="sxs-lookup"><span data-stu-id="04e7f-106">Filter statement</span></span>             | <span data-ttu-id="04e7f-107">Оператор SELECT</span><span class="sxs-lookup"><span data-stu-id="04e7f-107">Select statement</span></span>        | <span data-ttu-id="04e7f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="04e7f-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="04e7f-109">Перечисление всех семейств сайтов корневого уровня в Организации.</span><span class="sxs-lookup"><span data-stu-id="04e7f-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="04e7f-110">Полезен для обнаружения домашнего сайта для каждого из географических регионов.</span><span class="sxs-lookup"><span data-stu-id="04e7f-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="04e7f-111">Кроме того, вы можете использовать **[поисковый][]** запрос в семействе "" "" "" "" "" "" "" "" "" "" "</span><span class="sxs-lookup"><span data-stu-id="04e7f-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[выполнять]: site-search.md
[search]: site-search.md
[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="04e7f-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04e7f-114">Permissions</span></span>

<span data-ttu-id="04e7f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04e7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e7f-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04e7f-117">Permission type</span></span>                        | <span data-ttu-id="04e7f-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04e7f-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="04e7f-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04e7f-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="04e7f-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e7f-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="04e7f-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04e7f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04e7f-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04e7f-122">Not supported.</span></span>
|<span data-ttu-id="04e7f-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04e7f-123">Application</span></span>                            | <span data-ttu-id="04e7f-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e7f-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="04e7f-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04e7f-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="04e7f-126">Пример</span><span class="sxs-lookup"><span data-stu-id="04e7f-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="04e7f-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="04e7f-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="04e7f-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="04e7f-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04e7f-129">C#</span><span class="sxs-lookup"><span data-stu-id="04e7f-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04e7f-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04e7f-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04e7f-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="04e7f-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="04e7f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="04e7f-132">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->
