---
author: daspek
description: Получение Итемактивитистатс для действий, выполненных с этим ресурсом в течение указанного интервала времени.
ms.date: 10/06/2017
title: Получение статистики по действиям элемента по интервалу
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f2c3158fbc7ac8c925bc0bf2556623d01aa7b48d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123206"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="0d9a2-103">Получение статистики по действиям элемента по интервалу</span><span class="sxs-lookup"><span data-stu-id="0d9a2-103">Get item activity stats by interval</span></span>

<span data-ttu-id="0d9a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d9a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d9a2-105">Получение [итемактивитистатс][] для действий, выполненных с этим ресурсом в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="0d9a2-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="0d9a2-106">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="0d9a2-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="0d9a2-107">Статистические функции аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="0d9a2-107">Analytics aggregates might not be available for all action types.</span></span>

[итемактивитистатс]: ../resources/itemactivitystat.md
[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="0d9a2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d9a2-109">Permissions</span></span>

<span data-ttu-id="0d9a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d9a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d9a2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d9a2-112">Permission type</span></span>                        | <span data-ttu-id="0d9a2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d9a2-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="0d9a2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d9a2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d9a2-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d9a2-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="0d9a2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d9a2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d9a2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d9a2-117">Not supported.</span></span>
|<span data-ttu-id="0d9a2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d9a2-118">Application</span></span>                            | <span data-ttu-id="0d9a2-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d9a2-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="0d9a2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d9a2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="0d9a2-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0d9a2-121">Function parameters</span></span>

| <span data-ttu-id="0d9a2-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="0d9a2-122">Parameter</span></span>      | <span data-ttu-id="0d9a2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0d9a2-123">Type</span></span>               | <span data-ttu-id="0d9a2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0d9a2-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="0d9a2-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d9a2-125">startDateTime</span></span>  | <span data-ttu-id="0d9a2-126">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="0d9a2-126">string (timestamp)</span></span> | <span data-ttu-id="0d9a2-127">Время начала агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="0d9a2-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="0d9a2-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0d9a2-128">endDateTime</span></span>    | <span data-ttu-id="0d9a2-129">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="0d9a2-129">string (timestamp)</span></span> | <span data-ttu-id="0d9a2-130">Время окончания агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="0d9a2-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="0d9a2-131">interval</span><span class="sxs-lookup"><span data-stu-id="0d9a2-131">interval</span></span>       | <span data-ttu-id="0d9a2-132">string</span><span class="sxs-lookup"><span data-stu-id="0d9a2-132">string</span></span>             | <span data-ttu-id="0d9a2-133">Интервал объединения.</span><span class="sxs-lookup"><span data-stu-id="0d9a2-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="0d9a2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0d9a2-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0d9a2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d9a2-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0d9a2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d9a2-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="0d9a2-137">C#</span><span class="sxs-lookup"><span data-stu-id="0d9a2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d9a2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d9a2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d9a2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d9a2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d9a2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d9a2-140">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
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
