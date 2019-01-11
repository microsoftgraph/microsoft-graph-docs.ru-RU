---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Получение элементов активности Статистика по интервал
localization_priority: Normal
ms.openlocfilehash: 7ca0e4e4767073d37ebeabbab10e1f50ce323599
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826868"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="20119-102">Получение элементов активности Статистика по интервал</span><span class="sxs-lookup"><span data-stu-id="20119-102">Get item activity stats by interval</span></span>

> <span data-ttu-id="20119-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20119-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20119-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20119-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20119-105">Получите [itemActivityStats][] для выполнения действий, выполняемых в разделе этого ресурса в течение указанного временного интервала.</span><span class="sxs-lookup"><span data-stu-id="20119-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="20119-106">**Примечание:** **ItemAnalytics** ресурсов, пока недоступна во всех [Национальный развертываний](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="20119-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="20119-107">Статистические выражения на аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="20119-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="20119-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20119-109">Permissions</span></span>

<span data-ttu-id="20119-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20119-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20119-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20119-112">Permission type</span></span>                        | <span data-ttu-id="20119-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20119-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="20119-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20119-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="20119-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20119-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="20119-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20119-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20119-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20119-117">Not supported.</span></span>
|<span data-ttu-id="20119-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20119-118">Application</span></span>                            | <span data-ttu-id="20119-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20119-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="20119-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20119-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="20119-121">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="20119-121">Function parameters</span></span>

| <span data-ttu-id="20119-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="20119-122">Parameter</span></span>      | <span data-ttu-id="20119-123">Тип</span><span class="sxs-lookup"><span data-stu-id="20119-123">Type</span></span>               | <span data-ttu-id="20119-124">Описание</span><span class="sxs-lookup"><span data-stu-id="20119-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="20119-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="20119-125">startDateTime</span></span>  | <span data-ttu-id="20119-126">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="20119-126">string (timestamp)</span></span> | <span data-ttu-id="20119-127">Время начала развертываемыми статистической обработки действий.</span><span class="sxs-lookup"><span data-stu-id="20119-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="20119-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="20119-128">endDateTime</span></span>    | <span data-ttu-id="20119-129">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="20119-129">string (timestamp)</span></span> | <span data-ttu-id="20119-130">Время окончания развертываемыми статистические действиям.</span><span class="sxs-lookup"><span data-stu-id="20119-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="20119-131">interval</span><span class="sxs-lookup"><span data-stu-id="20119-131">interval</span></span>       | <span data-ttu-id="20119-132">string</span><span class="sxs-lookup"><span data-stu-id="20119-132">string</span></span>             | <span data-ttu-id="20119-133">Интервал статистической обработки.</span><span class="sxs-lookup"><span data-stu-id="20119-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="20119-134">Пример</span><span class="sxs-lookup"><span data-stu-id="20119-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="20119-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="20119-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="20119-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="20119-136">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval"
} -->
