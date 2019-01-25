---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Получение элементов активности Статистика по интервал
localization_priority: Normal
ms.openlocfilehash: f9601538d825efe346ab57fdbecd6c74dc9978d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516457"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="4b8f1-102">Получение элементов активности Статистика по интервал</span><span class="sxs-lookup"><span data-stu-id="4b8f1-102">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b8f1-103">Получите [itemActivityStats][] для выполнения действий, выполняемых в разделе этого ресурса в течение указанного временного интервала.</span><span class="sxs-lookup"><span data-stu-id="4b8f1-103">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="4b8f1-104">**Примечание:** **ItemAnalytics** ресурсов, пока недоступна во всех [Национальный развертываний](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="4b8f1-104">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="4b8f1-105">Статистические выражения на аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="4b8f1-105">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="4b8f1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b8f1-107">Permissions</span></span>

<span data-ttu-id="4b8f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b8f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b8f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b8f1-110">Permission type</span></span>                        | <span data-ttu-id="4b8f1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b8f1-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="4b8f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b8f1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b8f1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b8f1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="4b8f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b8f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b8f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b8f1-115">Not supported.</span></span>
|<span data-ttu-id="4b8f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b8f1-116">Application</span></span>                            | <span data-ttu-id="4b8f1-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b8f1-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4b8f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b8f1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="4b8f1-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4b8f1-119">Function parameters</span></span>

| <span data-ttu-id="4b8f1-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b8f1-120">Parameter</span></span>      | <span data-ttu-id="4b8f1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4b8f1-121">Type</span></span>               | <span data-ttu-id="4b8f1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4b8f1-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="4b8f1-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4b8f1-123">startDateTime</span></span>  | <span data-ttu-id="4b8f1-124">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="4b8f1-124">string (timestamp)</span></span> | <span data-ttu-id="4b8f1-125">Время начала развертываемыми статистической обработки действий.</span><span class="sxs-lookup"><span data-stu-id="4b8f1-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="4b8f1-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4b8f1-126">endDateTime</span></span>    | <span data-ttu-id="4b8f1-127">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="4b8f1-127">string (timestamp)</span></span> | <span data-ttu-id="4b8f1-128">Время окончания развертываемыми статистические действиям.</span><span class="sxs-lookup"><span data-stu-id="4b8f1-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="4b8f1-129">interval</span><span class="sxs-lookup"><span data-stu-id="4b8f1-129">interval</span></span>       | <span data-ttu-id="4b8f1-130">string</span><span class="sxs-lookup"><span data-stu-id="4b8f1-130">string</span></span>             | <span data-ttu-id="4b8f1-131">Интервал статистической обработки.</span><span class="sxs-lookup"><span data-stu-id="4b8f1-131">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="4b8f1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4b8f1-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4b8f1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b8f1-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="4b8f1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b8f1-134">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/itemactivity-getbyinterval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
