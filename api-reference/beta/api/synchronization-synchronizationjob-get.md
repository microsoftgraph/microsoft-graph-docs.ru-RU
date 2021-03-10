---
title: Получить синхронизациюJob
description: Извлечение существующего задания синхронизации и его свойств.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 64d5b801b7529b94cbc6a02bf20315cf4374eff4
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625985"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="36e0e-103">Получить синхронизациюJob</span><span class="sxs-lookup"><span data-stu-id="36e0e-103">Get synchronizationJob</span></span>

<span data-ttu-id="36e0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36e0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e0e-105">Извлечение существующего задания синхронизации и его свойств.</span><span class="sxs-lookup"><span data-stu-id="36e0e-105">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="36e0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36e0e-106">Permissions</span></span>
<span data-ttu-id="36e0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36e0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36e0e-109">Permission type</span></span>                        | <span data-ttu-id="36e0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36e0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="36e0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36e0e-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="36e0e-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="36e0e-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="36e0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36e0e-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="36e0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e0e-114">Not supported.</span></span>  |
|<span data-ttu-id="36e0e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="36e0e-115">Application</span></span>                            |<span data-ttu-id="36e0e-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36e0e-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36e0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36e0e-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="36e0e-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36e0e-118">Request headers</span></span>

| <span data-ttu-id="36e0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="36e0e-119">Name</span></span>           | <span data-ttu-id="36e0e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="36e0e-120">Type</span></span>    | <span data-ttu-id="36e0e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="36e0e-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="36e0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36e0e-122">Authorization</span></span>  | <span data-ttu-id="36e0e-123">string</span><span class="sxs-lookup"><span data-stu-id="36e0e-123">string</span></span>  | <span data-ttu-id="36e0e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36e0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36e0e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36e0e-126">Request body</span></span>

<span data-ttu-id="36e0e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36e0e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36e0e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e0e-128">Response</span></span>

<span data-ttu-id="36e0e-129">В случае успешного ответа `200 OK` возвращается ответ с [синхронизациейJob](../resources/synchronization-synchronizationjob.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36e0e-129">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36e0e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="36e0e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="36e0e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e0e-131">Request</span></span>
<span data-ttu-id="36e0e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36e0e-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36e0e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="36e0e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="36e0e-134">C#</span><span class="sxs-lookup"><span data-stu-id="36e0e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36e0e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36e0e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36e0e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36e0e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36e0e-137">Java</span><span class="sxs-lookup"><span data-stu-id="36e0e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36e0e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e0e-138">Response</span></span>
<span data-ttu-id="36e0e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36e0e-139">The following is an example of a response.</span></span> 

><span data-ttu-id="36e0e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36e0e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "quarantine": {
            "currentBegan": "",
            "nextAttempt": "",
            "reason": "",
            "seriesBegan": "",
            "seriesCount": 2,
            "error": {
                "code": "SalesforceInvalidCredentials",
                "message": "Your Salesforce.com credentials are invalid.  Please obtain a current Salesforce.com administrative user name, password and security token, and enter those in the screen for configuring user provisioning",
                "tenantActionable": true
            }
        },
        "troubleshootingUrl": null
    },
    "synchronizationJobSettings": [
      {
          "name": "QuarantineTooManyDeletesThreshold",
          "value": "500"
      }
    ]
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
  ]
}
-->


