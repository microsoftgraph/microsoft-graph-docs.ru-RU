---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Получение аналитики
localization_priority: Normal
ms.openlocfilehash: 6105d9ba900e3f7e985ef277f820ed6e6d9331b3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264619"
---
# <a name="get-analytics"></a><span data-ttu-id="4e4b7-102">Получение аналитики</span><span class="sxs-lookup"><span data-stu-id="4e4b7-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e4b7-103">Получение [итеманалитикс][] о представлениях, которые были выполнены для этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="4e4b7-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="4e4b7-104">Ресурс **итеманалитикс** — это удобный способ получения статистики действий `allTime` и. `lastSevenDays`</span><span class="sxs-lookup"><span data-stu-id="4e4b7-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="4e4b7-105">Для настраиваемого диапазона или интервала времени используйте API [getActivitiesByInterval][] .</span><span class="sxs-lookup"><span data-stu-id="4e4b7-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="4e4b7-106">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="4e4b7-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="4e4b7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e4b7-109">Permissions</span></span>

<span data-ttu-id="4e4b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e4b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e4b7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e4b7-112">Permission type</span></span>                        | <span data-ttu-id="4e4b7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e4b7-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="4e4b7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e4b7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e4b7-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e4b7-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="4e4b7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e4b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e4b7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e4b7-117">Not supported.</span></span>
|<span data-ttu-id="4e4b7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e4b7-118">Application</span></span>                            | <span data-ttu-id="4e4b7-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e4b7-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4e4b7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e4b7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="4e4b7-121">Пример</span><span class="sxs-lookup"><span data-stu-id="4e4b7-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4e4b7-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e4b7-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="4e4b7-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e4b7-123">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4e4b7-124">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4e4b7-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4e4b7-125">C#</span><span class="sxs-lookup"><span data-stu-id="4e4b7-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-analytics-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e4b7-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="4e4b7-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-analytics-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4e4b7-127">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4e4b7-127">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-analytics-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
