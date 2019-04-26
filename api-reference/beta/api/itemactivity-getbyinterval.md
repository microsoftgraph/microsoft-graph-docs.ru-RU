---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Получение статистики по действиям элемента по интервалу
localization_priority: Normal
ms.openlocfilehash: 3a05488aefbb01ab147dfff1da0e8d432259b248
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333551"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="d5b0b-102">Получение статистики по действиям элемента по интервалу</span><span class="sxs-lookup"><span data-stu-id="d5b0b-102">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5b0b-103">Получение [итемактивитистатс][] для действий, выполненных с этим ресурсом в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="d5b0b-103">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="d5b0b-104">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="d5b0b-104">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="d5b0b-105">Статистические функции аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="d5b0b-105">Analytics aggregates might not be available for all action types.</span></span>

[Итемактивитистатс]: ../resources/itemactivitystat.md
[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="d5b0b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5b0b-107">Permissions</span></span>

<span data-ttu-id="d5b0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5b0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5b0b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5b0b-110">Permission type</span></span>                        | <span data-ttu-id="d5b0b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5b0b-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d5b0b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5b0b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5b0b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b0b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d5b0b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5b0b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5b0b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5b0b-115">Not supported.</span></span>
|<span data-ttu-id="d5b0b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5b0b-116">Application</span></span>                            | <span data-ttu-id="d5b0b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b0b-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d5b0b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5b0b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="d5b0b-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d5b0b-119">Function parameters</span></span>

| <span data-ttu-id="d5b0b-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="d5b0b-120">Parameter</span></span>      | <span data-ttu-id="d5b0b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d5b0b-121">Type</span></span>               | <span data-ttu-id="d5b0b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d5b0b-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="d5b0b-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d5b0b-123">startDateTime</span></span>  | <span data-ttu-id="d5b0b-124">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="d5b0b-124">string (timestamp)</span></span> | <span data-ttu-id="d5b0b-125">Время начала агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="d5b0b-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="d5b0b-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d5b0b-126">endDateTime</span></span>    | <span data-ttu-id="d5b0b-127">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="d5b0b-127">string (timestamp)</span></span> | <span data-ttu-id="d5b0b-128">Время окончания агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="d5b0b-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="d5b0b-129">interval</span><span class="sxs-lookup"><span data-stu-id="d5b0b-129">interval</span></span>       | <span data-ttu-id="d5b0b-130">string</span><span class="sxs-lookup"><span data-stu-id="d5b0b-130">string</span></span>             | <span data-ttu-id="d5b0b-131">Интервал объединения.</span><span class="sxs-lookup"><span data-stu-id="d5b0b-131">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="d5b0b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d5b0b-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d5b0b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5b0b-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="d5b0b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5b0b-134">Response</span></span>

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
