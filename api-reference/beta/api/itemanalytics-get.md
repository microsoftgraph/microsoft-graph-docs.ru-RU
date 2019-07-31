---
author: daspek
description: Получение Итеманалитикс о представлениях, которые были выполнены для этого ресурса.
ms.date: 10/06/2017
title: Получение аналитики
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 47ee4b3d003c81b077e67cf8dca8e8cec047d37d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993181"
---
# <a name="get-analytics"></a><span data-ttu-id="c6e25-103">Получение аналитики</span><span class="sxs-lookup"><span data-stu-id="c6e25-103">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6e25-104">Получение [итеманалитикс][] о представлениях, которые были выполнены для этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="c6e25-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="c6e25-105">Ресурс **итеманалитикс** — это удобный способ получения статистики действий `allTime` и. `lastSevenDays`</span><span class="sxs-lookup"><span data-stu-id="c6e25-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="c6e25-106">Для настраиваемого диапазона или интервала времени используйте API [getActivitiesByInterval][] .</span><span class="sxs-lookup"><span data-stu-id="c6e25-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="c6e25-107">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="c6e25-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="c6e25-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6e25-110">Permissions</span></span>

<span data-ttu-id="c6e25-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6e25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6e25-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6e25-113">Permission type</span></span>                        | <span data-ttu-id="c6e25-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6e25-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c6e25-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6e25-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6e25-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6e25-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c6e25-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6e25-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6e25-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6e25-118">Not supported.</span></span>
|<span data-ttu-id="c6e25-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6e25-119">Application</span></span>                            | <span data-ttu-id="c6e25-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6e25-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c6e25-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6e25-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="c6e25-122">Пример</span><span class="sxs-lookup"><span data-stu-id="c6e25-122">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6e25-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6e25-123">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c6e25-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6e25-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c6e25-125">C#</span><span class="sxs-lookup"><span data-stu-id="c6e25-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6e25-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6e25-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c6e25-127">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6e25-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c6e25-128">Java</span><span class="sxs-lookup"><span data-stu-id="c6e25-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c6e25-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6e25-129">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
  ]
}
-->
