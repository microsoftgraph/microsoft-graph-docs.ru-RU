---
title: Получение synchronizationJob
description: Получение существующее задание синхронизации и его свойства.
localization_priority: Normal
ms.openlocfilehash: bb7c61192b165e5d05c0bb3434488ed2ff7ee8c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521693"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="3143f-103">Получение synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3143f-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3143f-104">Получение существующее задание синхронизации и его свойства.</span><span class="sxs-lookup"><span data-stu-id="3143f-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3143f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3143f-105">Permissions</span></span>
<span data-ttu-id="3143f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3143f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3143f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3143f-108">Permission type</span></span>                        | <span data-ttu-id="3143f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3143f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3143f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3143f-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="3143f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3143f-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3143f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3143f-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3143f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3143f-113">Not supported.</span></span>  |
|<span data-ttu-id="3143f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3143f-114">Application</span></span>                            |<span data-ttu-id="3143f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3143f-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3143f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3143f-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="3143f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3143f-117">Request headers</span></span>

| <span data-ttu-id="3143f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3143f-118">Name</span></span>           | <span data-ttu-id="3143f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3143f-119">Type</span></span>    | <span data-ttu-id="3143f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3143f-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3143f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3143f-121">Authorization</span></span>  | <span data-ttu-id="3143f-122">string</span><span class="sxs-lookup"><span data-stu-id="3143f-122">string</span></span>  | <span data-ttu-id="3143f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3143f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3143f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3143f-125">Request body</span></span>

<span data-ttu-id="3143f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3143f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3143f-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3143f-127">Response</span></span>

<span data-ttu-id="3143f-128">В случае успеха возвращает `200 OK` ответа с помощью [synchronizationJob](../resources/synchronization-synchronizationjob.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3143f-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3143f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3143f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3143f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3143f-130">Request</span></span>
<span data-ttu-id="3143f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3143f-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="3143f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="3143f-132">Response</span></span>
<span data-ttu-id="3143f-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3143f-133">The following is an example of a response.</span></span> 

><span data-ttu-id="3143f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3143f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2577

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "Paused",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "progress": [],
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
