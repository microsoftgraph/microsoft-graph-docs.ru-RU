---
author: daspek
description: Получение Итемактивитистатс для действий, выполненных с этим ресурсом в течение указанного интервала времени.
ms.date: 10/06/2017
title: Получение статистики по действиям элемента по интервалу
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6d1f7a3b4e6a326f107a0d0ff33db59ed73f2794
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979108"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="791cc-103">Получение статистики по действиям элемента по интервалу</span><span class="sxs-lookup"><span data-stu-id="791cc-103">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="791cc-104">Получение [итемактивитистатс][] для действий, выполненных с этим ресурсом в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="791cc-104">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="791cc-105">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="791cc-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="791cc-106">Статистические функции аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="791cc-106">Analytics aggregates might not be available for all action types.</span></span>

[Итемактивитистатс]: ../resources/itemactivitystat.md
[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="791cc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="791cc-108">Permissions</span></span>

<span data-ttu-id="791cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="791cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="791cc-111">Permission type</span></span>                        | <span data-ttu-id="791cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="791cc-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="791cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="791cc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="791cc-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791cc-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="791cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="791cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="791cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791cc-116">Not supported.</span></span>
|<span data-ttu-id="791cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="791cc-117">Application</span></span>                            | <span data-ttu-id="791cc-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791cc-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="791cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="791cc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="791cc-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="791cc-120">Function parameters</span></span>

| <span data-ttu-id="791cc-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="791cc-121">Parameter</span></span>      | <span data-ttu-id="791cc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="791cc-122">Type</span></span>               | <span data-ttu-id="791cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="791cc-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="791cc-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="791cc-124">startDateTime</span></span>  | <span data-ttu-id="791cc-125">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="791cc-125">string (timestamp)</span></span> | <span data-ttu-id="791cc-126">Время начала агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="791cc-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="791cc-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="791cc-127">endDateTime</span></span>    | <span data-ttu-id="791cc-128">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="791cc-128">string (timestamp)</span></span> | <span data-ttu-id="791cc-129">Время окончания агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="791cc-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="791cc-130">interval</span><span class="sxs-lookup"><span data-stu-id="791cc-130">interval</span></span>       | <span data-ttu-id="791cc-131">string</span><span class="sxs-lookup"><span data-stu-id="791cc-131">string</span></span>             | <span data-ttu-id="791cc-132">Интервал объединения.</span><span class="sxs-lookup"><span data-stu-id="791cc-132">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="791cc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="791cc-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="791cc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="791cc-134">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="791cc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="791cc-135">Response</span></span>

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
