---
title: Получение Синчронизатионжоб
description: Получение существующего задания синхронизации и его свойств.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a3e1ef3ae7d63dc3393bcf8641f1d598f549c2fe
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280626"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="0dadf-103">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="0dadf-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dadf-104">Получение существующего задания синхронизации и его свойств.</span><span class="sxs-lookup"><span data-stu-id="0dadf-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dadf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0dadf-105">Permissions</span></span>
<span data-ttu-id="0dadf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dadf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dadf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0dadf-108">Permission type</span></span>                        | <span data-ttu-id="0dadf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0dadf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dadf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0dadf-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="0dadf-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dadf-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0dadf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0dadf-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0dadf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dadf-113">Not supported.</span></span>  |
|<span data-ttu-id="0dadf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0dadf-114">Application</span></span>                            |<span data-ttu-id="0dadf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dadf-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0dadf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0dadf-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="0dadf-117">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0dadf-117">Request headers</span></span>

| <span data-ttu-id="0dadf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0dadf-118">Name</span></span>           | <span data-ttu-id="0dadf-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0dadf-119">Type</span></span>    | <span data-ttu-id="0dadf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0dadf-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0dadf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dadf-121">Authorization</span></span>  | <span data-ttu-id="0dadf-122">string</span><span class="sxs-lookup"><span data-stu-id="0dadf-122">string</span></span>  | <span data-ttu-id="0dadf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0dadf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dadf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0dadf-125">Request body</span></span>

<span data-ttu-id="0dadf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0dadf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dadf-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0dadf-127">Response</span></span>

<span data-ttu-id="0dadf-128">В случае успеха возвращает `200 OK` ответ с [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0dadf-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dadf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0dadf-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0dadf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dadf-130">Request</span></span>
<span data-ttu-id="0dadf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0dadf-131">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0dadf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dadf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="0dadf-133">C#</span><span class="sxs-lookup"><span data-stu-id="0dadf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dadf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dadf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dadf-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dadf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0dadf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dadf-136">Response</span></span>
<span data-ttu-id="0dadf-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0dadf-137">The following is an example of a response.</span></span> 

><span data-ttu-id="0dadf-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0dadf-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
