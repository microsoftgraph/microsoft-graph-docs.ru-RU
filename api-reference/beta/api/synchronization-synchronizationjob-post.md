---
title: Создание Синчронизатионжоб
description: Создайте новое задание синхронизации с схемой синхронизации по умолчанию. Задание создано в отключенном состоянии. Запустите задание запуска, чтобы начать синхронизацию.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9af5006f078e6fc0673ccc69e239a0b904044ac
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409774"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="cac98-105">Создание Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="cac98-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cac98-106">Создайте новое задание синхронизации с схемой синхронизации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cac98-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="cac98-107">Задание создано в отключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="cac98-107">The job is created in a disabled state.</span></span> <span data-ttu-id="cac98-108">Запустите [Задание запуска](synchronization-synchronizationjob-start.md) , чтобы начать синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="cac98-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="cac98-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cac98-109">Permissions</span></span>
<span data-ttu-id="cac98-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cac98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac98-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cac98-112">Permission type</span></span>                        | <span data-ttu-id="cac98-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cac98-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cac98-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cac98-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="cac98-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac98-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cac98-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cac98-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cac98-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cac98-117">Not supported.</span></span>|
|<span data-ttu-id="cac98-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cac98-118">Application</span></span>                            |<span data-ttu-id="cac98-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cac98-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="cac98-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cac98-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="cac98-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cac98-121">Request headers</span></span>

| <span data-ttu-id="cac98-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cac98-122">Name</span></span>           | <span data-ttu-id="cac98-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cac98-123">Type</span></span>    | <span data-ttu-id="cac98-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cac98-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cac98-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cac98-125">Authorization</span></span>  | <span data-ttu-id="cac98-126">string</span><span class="sxs-lookup"><span data-stu-id="cac98-126">string</span></span>  | <span data-ttu-id="cac98-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cac98-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cac98-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cac98-129">Request body</span></span>

<span data-ttu-id="cac98-130">В тексте запроса добавьте представление объекта [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cac98-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="cac98-131">Единственное обязательное свойство — `templateId`.</span><span class="sxs-lookup"><span data-stu-id="cac98-131">The only required property is `templateId`.</span></span> <span data-ttu-id="cac98-132">`templateId` Свойство должно быть соответствующим одному из шаблонов, созданных для этого приложения или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cac98-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="cac98-133">Чтобы найти доступные шаблоны, используйте [шаблоны списков](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="cac98-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="cac98-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac98-134">Response</span></span>

<span data-ttu-id="cac98-135">В случае успеха возвращает код `201 Created` отклика и объект [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cac98-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac98-136">Пример</span><span class="sxs-lookup"><span data-stu-id="cac98-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cac98-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cac98-137">Request</span></span>
<span data-ttu-id="cac98-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cac98-138">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cac98-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cac98-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cac98-140">C#</span><span class="sxs-lookup"><span data-stu-id="cac98-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cac98-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cac98-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cac98-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cac98-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cac98-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac98-143">Response</span></span>
<span data-ttu-id="cac98-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cac98-144">The following is an example of a response.</span></span> 

><span data-ttu-id="cac98-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cac98-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
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
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
