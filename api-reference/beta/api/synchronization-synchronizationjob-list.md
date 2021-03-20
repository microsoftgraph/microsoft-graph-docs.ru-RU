---
title: Задания синхронизации списков
description: Список существующих заданий для данного экземпляра приложения (основной службы).
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d51a49267d9e280abd59423af251561234b557ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953007"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="ed120-103">Задания синхронизации списков</span><span class="sxs-lookup"><span data-stu-id="ed120-103">List synchronization jobs</span></span>

<span data-ttu-id="ed120-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed120-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed120-105">Список существующих заданий для данного экземпляра приложения (основной службы).</span><span class="sxs-lookup"><span data-stu-id="ed120-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed120-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed120-106">Permissions</span></span>
<span data-ttu-id="ed120-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed120-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed120-109">Permission type</span></span>                        | <span data-ttu-id="ed120-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed120-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed120-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed120-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="ed120-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed120-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ed120-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed120-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ed120-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed120-114">Not supported.</span></span> |
|<span data-ttu-id="ed120-115">Application</span><span class="sxs-lookup"><span data-stu-id="ed120-115">Application</span></span>                            |<span data-ttu-id="ed120-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed120-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ed120-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed120-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="ed120-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ed120-118">Request headers</span></span>

| <span data-ttu-id="ed120-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ed120-119">Name</span></span>           | <span data-ttu-id="ed120-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ed120-120">Type</span></span>    | <span data-ttu-id="ed120-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ed120-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ed120-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed120-122">Authorization</span></span>  | <span data-ttu-id="ed120-123">string</span><span class="sxs-lookup"><span data-stu-id="ed120-123">string</span></span>  | <span data-ttu-id="ed120-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed120-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed120-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed120-126">Request body</span></span>

<span data-ttu-id="ed120-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed120-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed120-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed120-128">Response</span></span>

<span data-ttu-id="ed120-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [синхронизацииJob](../resources/synchronization-synchronizationjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ed120-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed120-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ed120-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ed120-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed120-131">Request</span></span>
<span data-ttu-id="ed120-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed120-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed120-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed120-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="ed120-134">C#</span><span class="sxs-lookup"><span data-stu-id="ed120-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed120-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed120-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed120-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed120-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed120-137">Java</span><span class="sxs-lookup"><span data-stu-id="ed120-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed120-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed120-138">Response</span></span>
<span data-ttu-id="ed120-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed120-139">The following is an example of a response.</span></span> 

><span data-ttu-id="ed120-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed120-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2958

{
    "value": [
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
                "lastSuccessfulExecutionWithExports": null,
                "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
                "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
                "quarantine": null,
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


