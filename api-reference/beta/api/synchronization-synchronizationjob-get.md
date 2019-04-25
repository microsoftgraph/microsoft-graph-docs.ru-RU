---
title: Получение Синчронизатионжоб
description: Получение существующего задания синхронизации и его свойств.
localization_priority: Normal
ms.openlocfilehash: bb7c61192b165e5d05c0bb3434488ed2ff7ee8c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537183"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="5679b-103">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="5679b-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5679b-104">Получение существующего задания синхронизации и его свойств.</span><span class="sxs-lookup"><span data-stu-id="5679b-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5679b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5679b-105">Permissions</span></span>
<span data-ttu-id="5679b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5679b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5679b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5679b-108">Permission type</span></span>                        | <span data-ttu-id="5679b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5679b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5679b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5679b-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="5679b-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5679b-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5679b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5679b-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5679b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5679b-113">Not supported.</span></span>  |
|<span data-ttu-id="5679b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5679b-114">Application</span></span>                            |<span data-ttu-id="5679b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5679b-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5679b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5679b-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="5679b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5679b-117">Request headers</span></span>

| <span data-ttu-id="5679b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5679b-118">Name</span></span>           | <span data-ttu-id="5679b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5679b-119">Type</span></span>    | <span data-ttu-id="5679b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5679b-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5679b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5679b-121">Authorization</span></span>  | <span data-ttu-id="5679b-122">string</span><span class="sxs-lookup"><span data-stu-id="5679b-122">string</span></span>  | <span data-ttu-id="5679b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5679b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5679b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5679b-125">Request body</span></span>

<span data-ttu-id="5679b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5679b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5679b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5679b-127">Response</span></span>

<span data-ttu-id="5679b-128">В случае успеха возвращает `200 OK` ответ с [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5679b-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5679b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5679b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5679b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5679b-130">Request</span></span>
<span data-ttu-id="5679b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5679b-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="5679b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5679b-132">Response</span></span>
<span data-ttu-id="5679b-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5679b-133">The following is an example of a response.</span></span> 

><span data-ttu-id="5679b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5679b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
