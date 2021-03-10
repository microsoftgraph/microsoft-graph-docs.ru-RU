---
author: daspek
description: Получите itemActivityStats для действий, которые проходили в этом ресурсе в течение указанного интервала времени.
ms.date: 10/06/2017
title: Получать статистику активности элементов по интервалу
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 112c08515e053cde7ff3e2d30965f1c9b1400629
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626105"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="6c028-103">Получать статистику активности элементов по интервалу</span><span class="sxs-lookup"><span data-stu-id="6c028-103">Get item activity stats by interval</span></span>

<span data-ttu-id="6c028-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c028-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c028-105">Получите [itemActivityStats][] для действий, которые проходили в этом ресурсе в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="6c028-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="6c028-106">**Примечание:** Ресурс **itemAnalytics** еще не доступен во всех [национальных развертываниях.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="6c028-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="6c028-107">Агрегаты аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="6c028-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="6c028-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c028-109">Permissions</span></span>

<span data-ttu-id="6c028-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c028-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c028-112">Permission type</span></span>                        | <span data-ttu-id="6c028-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c028-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="6c028-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c028-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c028-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c028-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="6c028-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c028-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c028-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c028-117">Not supported.</span></span>
|<span data-ttu-id="6c028-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c028-118">Application</span></span>                            | <span data-ttu-id="6c028-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c028-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6c028-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c028-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',endDateTime='2017-05-20',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="6c028-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6c028-121">Function parameters</span></span>

| <span data-ttu-id="6c028-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="6c028-122">Parameter</span></span>      | <span data-ttu-id="6c028-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6c028-123">Type</span></span>               | <span data-ttu-id="6c028-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6c028-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="6c028-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6c028-125">startDateTime</span></span>  | <span data-ttu-id="6c028-126">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="6c028-126">string (timestamp)</span></span> | <span data-ttu-id="6c028-127">Время начала, за которое можно агрегировать действия.</span><span class="sxs-lookup"><span data-stu-id="6c028-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="6c028-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6c028-128">endDateTime</span></span>    | <span data-ttu-id="6c028-129">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="6c028-129">string (timestamp)</span></span> | <span data-ttu-id="6c028-130">Конечный период, за который можно агрегировать действия.</span><span class="sxs-lookup"><span data-stu-id="6c028-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="6c028-131">interval</span><span class="sxs-lookup"><span data-stu-id="6c028-131">interval</span></span>       | <span data-ttu-id="6c028-132">Строка</span><span class="sxs-lookup"><span data-stu-id="6c028-132">string</span></span>             | <span data-ttu-id="6c028-133">Интервал агрегации.</span><span class="sxs-lookup"><span data-stu-id="6c028-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="6c028-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6c028-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6c028-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c028-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c028-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c028-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="6c028-137">C#</span><span class="sxs-lookup"><span data-stu-id="6c028-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c028-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c028-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c028-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c028-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c028-140">Java</span><span class="sxs-lookup"><span data-stu-id="6c028-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c028-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c028-141">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
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
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": []
}
-->


