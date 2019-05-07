---
title: Список заданий синхронизации
description: Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).
localization_priority: Normal
ms.openlocfilehash: eb933168d3f3673f076e275ad99e56b8a46888e0
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638076"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="1d6c7-103">Список заданий синхронизации</span><span class="sxs-lookup"><span data-stu-id="1d6c7-103">List synchronization jobs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d6c7-104">Перечисление существующих заданий для определенного экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="1d6c7-104">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d6c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d6c7-105">Permissions</span></span>
<span data-ttu-id="1d6c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d6c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d6c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d6c7-108">Permission type</span></span>                        | <span data-ttu-id="1d6c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d6c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d6c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d6c7-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="1d6c7-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d6c7-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="1d6c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d6c7-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="1d6c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-113">Not supported.</span></span> |
|<span data-ttu-id="1d6c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d6c7-114">Application</span></span>                            |<span data-ttu-id="1d6c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1d6c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d6c7-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="1d6c7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d6c7-117">Request headers</span></span>

| <span data-ttu-id="1d6c7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1d6c7-118">Name</span></span>           | <span data-ttu-id="1d6c7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1d6c7-119">Type</span></span>    | <span data-ttu-id="1d6c7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1d6c7-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="1d6c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d6c7-121">Authorization</span></span>  | <span data-ttu-id="1d6c7-122">string</span><span class="sxs-lookup"><span data-stu-id="1d6c7-122">string</span></span>  | <span data-ttu-id="1d6c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d6c7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d6c7-125">Request body</span></span>

<span data-ttu-id="1d6c7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d6c7-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d6c7-127">Response</span></span>

<span data-ttu-id="1d6c7-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-128">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d6c7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1d6c7-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1d6c7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d6c7-130">Request</span></span>
<span data-ttu-id="1d6c7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="1d6c7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d6c7-132">Response</span></span>
<span data-ttu-id="1d6c7-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-133">The following is an example of a response.</span></span> 

><span data-ttu-id="1d6c7-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1d6c7-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d6c7-135">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1d6c7-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="1d6c7-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1d6c7-137">Языках</span><span class="sxs-lookup"><span data-stu-id="1d6c7-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_jobs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d6c7-138">Язык</span><span class="sxs-lookup"><span data-stu-id="1d6c7-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_jobs-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
