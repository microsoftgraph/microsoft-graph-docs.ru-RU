---
title: Получить синхронизациюJob
description: Извлечение существующего задания синхронизации и его свойств.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 7fd473b0d289f92a28ef92d094d7450ecac8431d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054842"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="78817-103">Получить синхронизациюJob</span><span class="sxs-lookup"><span data-stu-id="78817-103">Get synchronizationJob</span></span>

<span data-ttu-id="78817-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78817-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78817-105">Извлечение существующего задания синхронизации и его свойств.</span><span class="sxs-lookup"><span data-stu-id="78817-105">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="78817-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78817-106">Permissions</span></span>
<span data-ttu-id="78817-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78817-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78817-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78817-109">Permission type</span></span>                        | <span data-ttu-id="78817-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78817-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="78817-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78817-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="78817-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="78817-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="78817-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78817-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="78817-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78817-114">Not supported.</span></span>  |
|<span data-ttu-id="78817-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="78817-115">Application</span></span>                            |<span data-ttu-id="78817-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78817-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="78817-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78817-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="78817-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="78817-118">Request headers</span></span>

| <span data-ttu-id="78817-119">Имя</span><span class="sxs-lookup"><span data-stu-id="78817-119">Name</span></span>           | <span data-ttu-id="78817-120">Тип</span><span class="sxs-lookup"><span data-stu-id="78817-120">Type</span></span>    | <span data-ttu-id="78817-121">Описание</span><span class="sxs-lookup"><span data-stu-id="78817-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="78817-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78817-122">Authorization</span></span>  | <span data-ttu-id="78817-123">string</span><span class="sxs-lookup"><span data-stu-id="78817-123">string</span></span>  | <span data-ttu-id="78817-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78817-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78817-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78817-126">Request body</span></span>

<span data-ttu-id="78817-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78817-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78817-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="78817-128">Response</span></span>

<span data-ttu-id="78817-129">В случае успешного ответа `200 OK` возвращается ответ с [синхронизациейJob](../resources/synchronization-synchronizationjob.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="78817-129">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78817-130">Пример</span><span class="sxs-lookup"><span data-stu-id="78817-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="78817-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="78817-131">Request</span></span>
<span data-ttu-id="78817-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78817-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78817-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="78817-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="78817-134">C#</span><span class="sxs-lookup"><span data-stu-id="78817-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78817-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78817-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78817-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78817-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78817-137">Java</span><span class="sxs-lookup"><span data-stu-id="78817-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="78817-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="78817-138">Response</span></span>
<span data-ttu-id="78817-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="78817-139">The following is an example of a response.</span></span> 

><span data-ttu-id="78817-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="78817-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


