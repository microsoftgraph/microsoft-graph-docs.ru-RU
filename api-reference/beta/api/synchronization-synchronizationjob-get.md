---
title: Получение synchronizationJob
description: Получение существующее задание синхронизации и его свойства.
ms.openlocfilehash: c0c999d5b9ce168ba3f21af20ec5cff026d68f8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082306"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="aac20-103">Получение synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="aac20-103">Get synchronizationJob</span></span>

> <span data-ttu-id="aac20-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aac20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aac20-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aac20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aac20-106">Получение существующее задание синхронизации и его свойства.</span><span class="sxs-lookup"><span data-stu-id="aac20-106">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="aac20-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aac20-107">Permissions</span></span>
<span data-ttu-id="aac20-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aac20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aac20-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aac20-110">Permission type</span></span>                        | <span data-ttu-id="aac20-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aac20-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aac20-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aac20-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="aac20-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac20-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="aac20-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aac20-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="aac20-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aac20-115">Not supported.</span></span>  |
|<span data-ttu-id="aac20-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aac20-116">Application</span></span>                            |<span data-ttu-id="aac20-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aac20-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aac20-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aac20-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="aac20-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aac20-119">Request headers</span></span>

| <span data-ttu-id="aac20-120">Имя</span><span class="sxs-lookup"><span data-stu-id="aac20-120">Name</span></span>           | <span data-ttu-id="aac20-121">Тип</span><span class="sxs-lookup"><span data-stu-id="aac20-121">Type</span></span>    | <span data-ttu-id="aac20-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aac20-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="aac20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac20-123">Authorization</span></span>  | <span data-ttu-id="aac20-124">string</span><span class="sxs-lookup"><span data-stu-id="aac20-124">string</span></span>  | <span data-ttu-id="aac20-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aac20-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aac20-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aac20-127">Request body</span></span>

<span data-ttu-id="aac20-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aac20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aac20-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="aac20-129">Response</span></span>

<span data-ttu-id="aac20-130">В случае успеха возвращает `200 OK` ответа с помощью [synchronizationJob](../resources/synchronization-synchronizationjob.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aac20-130">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac20-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aac20-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aac20-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aac20-132">Request</span></span>
<span data-ttu-id="aac20-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aac20-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="aac20-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="aac20-134">Response</span></span>
<span data-ttu-id="aac20-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aac20-135">The following is an example of a response.</span></span> 

><span data-ttu-id="aac20-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aac20-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->