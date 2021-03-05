---
author: daspek
description: Получите itemAnalytics о представлениях, которые произошли в этом ресурсе.
ms.date: 10/06/2017
title: Получение аналитики
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6366106097b4f6b9b43d8fe0eacddeaeab53826d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475837"
---
# <a name="get-analytics"></a><span data-ttu-id="8a2b2-103">Получение аналитики</span><span class="sxs-lookup"><span data-stu-id="8a2b2-103">Get analytics</span></span>

<span data-ttu-id="8a2b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a2b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a2b2-105">Получите [itemAnalytics][] о представлениях, которые произошли в этом ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8a2b2-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="8a2b2-106">Ресурс **itemAnalytics** — это удобный способ получения статистики активности для `allTime` и `lastSevenDays` .</span><span class="sxs-lookup"><span data-stu-id="8a2b2-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="8a2b2-107">Для настраиваемого диапазона времени или интервала используйте [API getActivitiesByInterval.][]</span><span class="sxs-lookup"><span data-stu-id="8a2b2-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="8a2b2-108">**Примечание:** Ресурс **itemAnalytics** еще не доступен во всех [национальных развертываниях.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="8a2b2-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="8a2b2-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a2b2-111">Permissions</span></span>

<span data-ttu-id="8a2b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a2b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a2b2-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a2b2-114">Permission type</span></span>                        | <span data-ttu-id="8a2b2-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a2b2-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="8a2b2-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a2b2-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a2b2-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a2b2-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="8a2b2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a2b2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a2b2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a2b2-119">Not supported.</span></span>
|<span data-ttu-id="8a2b2-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a2b2-120">Application</span></span>                            | <span data-ttu-id="8a2b2-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a2b2-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8a2b2-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a2b2-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="8a2b2-123">Пример</span><span class="sxs-lookup"><span data-stu-id="8a2b2-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8a2b2-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a2b2-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8a2b2-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a2b2-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="8a2b2-126">C#</span><span class="sxs-lookup"><span data-stu-id="8a2b2-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a2b2-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a2b2-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a2b2-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a2b2-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a2b2-129">Java</span><span class="sxs-lookup"><span data-stu-id="8a2b2-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a2b2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a2b2-130">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```http
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


