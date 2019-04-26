---
title: Список заданий синхронизации
description: ПереЧисление существующих заданий для определенного экземпляра приложения (субъекта-службы).
localization_priority: Normal
ms.openlocfilehash: 7f4098b0df22daacca6a2de50b2c41e4e8dea0fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335698"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="f6575-103">Список заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="f6575-103">List synchronization jobs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6575-104">ПереЧисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="f6575-104">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6575-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6575-105">Permissions</span></span>
<span data-ttu-id="f6575-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6575-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6575-108">Permission type</span></span>                        | <span data-ttu-id="f6575-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6575-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6575-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6575-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="f6575-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6575-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f6575-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6575-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f6575-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6575-113">Not supported.</span></span> |
|<span data-ttu-id="f6575-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6575-114">Application</span></span>                            |<span data-ttu-id="f6575-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6575-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f6575-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6575-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="f6575-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6575-117">Request headers</span></span>

| <span data-ttu-id="f6575-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f6575-118">Name</span></span>           | <span data-ttu-id="f6575-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f6575-119">Type</span></span>    | <span data-ttu-id="f6575-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f6575-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f6575-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6575-121">Authorization</span></span>  | <span data-ttu-id="f6575-122">string</span><span class="sxs-lookup"><span data-stu-id="f6575-122">string</span></span>  | <span data-ttu-id="f6575-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6575-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6575-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6575-125">Request body</span></span>

<span data-ttu-id="f6575-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6575-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6575-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6575-127">Response</span></span>

<span data-ttu-id="f6575-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6575-128">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6575-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f6575-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f6575-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6575-130">Request</span></span>
<span data-ttu-id="f6575-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6575-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="f6575-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6575-132">Response</span></span>
<span data-ttu-id="f6575-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6575-133">The following is an example of a response.</span></span> 

><span data-ttu-id="f6575-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6575-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
