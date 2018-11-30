---
title: Список заданий синхронизации
description: Список существующих заданий для экземпляра данного приложения (участников-служб).
ms.openlocfilehash: 179a6906936fddbfc31ffc7b016de05908f2383a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081232"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="1b578-103">Список заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="1b578-103">List synchronization jobs</span></span>

> <span data-ttu-id="1b578-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b578-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b578-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b578-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b578-106">Список существующих заданий для экземпляра данного приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="1b578-106">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b578-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b578-107">Permissions</span></span>
<span data-ttu-id="1b578-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b578-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b578-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b578-110">Permission type</span></span>                        | <span data-ttu-id="1b578-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b578-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b578-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b578-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="1b578-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b578-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1b578-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b578-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1b578-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b578-115">Not supported.</span></span> |
|<span data-ttu-id="1b578-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b578-116">Application</span></span>                            |<span data-ttu-id="1b578-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b578-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1b578-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b578-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="1b578-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b578-119">Request headers</span></span>

| <span data-ttu-id="1b578-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1b578-120">Name</span></span>           | <span data-ttu-id="1b578-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1b578-121">Type</span></span>    | <span data-ttu-id="1b578-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1b578-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1b578-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b578-123">Authorization</span></span>  | <span data-ttu-id="1b578-124">string</span><span class="sxs-lookup"><span data-stu-id="1b578-124">string</span></span>  | <span data-ttu-id="1b578-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b578-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b578-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b578-127">Request body</span></span>

<span data-ttu-id="1b578-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b578-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b578-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b578-129">Response</span></span>

<span data-ttu-id="1b578-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [synchronizationJob](../resources/synchronization-synchronizationjob.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1b578-130">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b578-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1b578-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1b578-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b578-132">Request</span></span>
<span data-ttu-id="1b578-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b578-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="1b578-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b578-134">Response</span></span>
<span data-ttu-id="1b578-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1b578-135">The following is an example of a response.</span></span> 

><span data-ttu-id="1b578-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b578-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->