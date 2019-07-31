---
title: Получение Синчронизатионжоб
description: Получение существующего задания синхронизации и его свойств.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0977a3b771e92b95356c238d699d0b42576c4aaa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977781"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="7e244-103">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="7e244-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e244-104">Получение существующего задания синхронизации и его свойств.</span><span class="sxs-lookup"><span data-stu-id="7e244-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e244-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e244-105">Permissions</span></span>
<span data-ttu-id="7e244-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e244-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e244-108">Permission type</span></span>                        | <span data-ttu-id="7e244-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e244-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e244-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e244-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="7e244-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e244-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7e244-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e244-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7e244-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e244-113">Not supported.</span></span>  |
|<span data-ttu-id="7e244-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e244-114">Application</span></span>                            |<span data-ttu-id="7e244-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e244-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7e244-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e244-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="7e244-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e244-117">Request headers</span></span>

| <span data-ttu-id="7e244-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e244-118">Name</span></span>           | <span data-ttu-id="7e244-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7e244-119">Type</span></span>    | <span data-ttu-id="7e244-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7e244-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7e244-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e244-121">Authorization</span></span>  | <span data-ttu-id="7e244-122">string</span><span class="sxs-lookup"><span data-stu-id="7e244-122">string</span></span>  | <span data-ttu-id="7e244-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e244-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e244-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e244-125">Request body</span></span>

<span data-ttu-id="7e244-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e244-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e244-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e244-127">Response</span></span>

<span data-ttu-id="7e244-128">В случае успеха возвращает `200 OK` ответ с [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e244-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e244-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7e244-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e244-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e244-130">Request</span></span>
<span data-ttu-id="7e244-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e244-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7e244-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e244-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e244-133">C#</span><span class="sxs-lookup"><span data-stu-id="7e244-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e244-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e244-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e244-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7e244-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e244-136">Java</span><span class="sxs-lookup"><span data-stu-id="7e244-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e244-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e244-137">Response</span></span>
<span data-ttu-id="7e244-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e244-138">The following is an example of a response.</span></span> 

><span data-ttu-id="7e244-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e244-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
