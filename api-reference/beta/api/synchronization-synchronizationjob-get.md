---
title: Получение Синчронизатионжоб
description: Получение существующего задания синхронизации и его свойств.
localization_priority: Normal
ms.openlocfilehash: 6e21f1b86736286c624f77d4ce305d02791dfd26
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457053"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="f221e-103">Получение Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="f221e-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f221e-104">Получение существующего задания синхронизации и его свойств.</span><span class="sxs-lookup"><span data-stu-id="f221e-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f221e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f221e-105">Permissions</span></span>
<span data-ttu-id="f221e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f221e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f221e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f221e-108">Permission type</span></span>                        | <span data-ttu-id="f221e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f221e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f221e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f221e-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="f221e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f221e-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f221e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f221e-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f221e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f221e-113">Not supported.</span></span>  |
|<span data-ttu-id="f221e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f221e-114">Application</span></span>                            |<span data-ttu-id="f221e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f221e-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f221e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f221e-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="f221e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f221e-117">Request headers</span></span>

| <span data-ttu-id="f221e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f221e-118">Name</span></span>           | <span data-ttu-id="f221e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f221e-119">Type</span></span>    | <span data-ttu-id="f221e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f221e-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f221e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f221e-121">Authorization</span></span>  | <span data-ttu-id="f221e-122">string</span><span class="sxs-lookup"><span data-stu-id="f221e-122">string</span></span>  | <span data-ttu-id="f221e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f221e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f221e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f221e-125">Request body</span></span>

<span data-ttu-id="f221e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f221e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f221e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f221e-127">Response</span></span>

<span data-ttu-id="f221e-128">В случае успеха возвращает `200 OK` ответ с [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f221e-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f221e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f221e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f221e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f221e-130">Request</span></span>
<span data-ttu-id="f221e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f221e-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f221e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f221e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f221e-133">C#</span><span class="sxs-lookup"><span data-stu-id="f221e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f221e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f221e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f221e-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f221e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f221e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f221e-136">Response</span></span>
<span data-ttu-id="f221e-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f221e-137">The following is an example of a response.</span></span> 

><span data-ttu-id="f221e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f221e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
