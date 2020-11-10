---
title: Список заданий синхронизации
description: Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c59a3414d1e480caee34023b6ad0bd5fd7773684
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974220"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="bb033-103">Список заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="bb033-103">List synchronization jobs</span></span>

<span data-ttu-id="bb033-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb033-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb033-105">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="bb033-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb033-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb033-106">Permissions</span></span>
<span data-ttu-id="bb033-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb033-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb033-109">Permission type</span></span>                        | <span data-ttu-id="bb033-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb033-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb033-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb033-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="bb033-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb033-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bb033-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb033-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bb033-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb033-114">Not supported.</span></span> |
|<span data-ttu-id="bb033-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb033-115">Application</span></span>                            |<span data-ttu-id="bb033-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb033-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bb033-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb033-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="bb033-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb033-118">Request headers</span></span>

| <span data-ttu-id="bb033-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bb033-119">Name</span></span>           | <span data-ttu-id="bb033-120">Тип</span><span class="sxs-lookup"><span data-stu-id="bb033-120">Type</span></span>    | <span data-ttu-id="bb033-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bb033-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bb033-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb033-122">Authorization</span></span>  | <span data-ttu-id="bb033-123">string</span><span class="sxs-lookup"><span data-stu-id="bb033-123">string</span></span>  | <span data-ttu-id="bb033-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb033-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb033-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb033-126">Request body</span></span>

<span data-ttu-id="bb033-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb033-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb033-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb033-128">Response</span></span>

<span data-ttu-id="bb033-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb033-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb033-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bb033-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bb033-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb033-131">Request</span></span>
<span data-ttu-id="bb033-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb033-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb033-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb033-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="bb033-134">C#</span><span class="sxs-lookup"><span data-stu-id="bb033-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb033-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb033-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb033-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb033-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb033-137">Java</span><span class="sxs-lookup"><span data-stu-id="bb033-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb033-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb033-138">Response</span></span>
<span data-ttu-id="bb033-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb033-139">The following is an example of a response.</span></span> 

><span data-ttu-id="bb033-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb033-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


