---
title: Создание Синчронизатионжоб
description: Создайте новое задание синхронизации с схемой синхронизации по умолчанию. Задание создано в отключенном состоянии. Запустите задание запуска, чтобы начать синхронизацию.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7fac7eda83cb5caf4332110e38367acb876c8ef7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437551"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="c66c0-105">Создание Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="c66c0-105">Create synchronizationJob</span></span>

<span data-ttu-id="c66c0-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c66c0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c66c0-107">Создайте новое задание синхронизации с схемой синхронизации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c66c0-107">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="c66c0-108">Задание создано в отключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="c66c0-108">The job is created in a disabled state.</span></span> <span data-ttu-id="c66c0-109">Запустите [Задание запуска](synchronization-synchronizationjob-start.md) , чтобы начать синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="c66c0-109">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c66c0-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c66c0-110">Permissions</span></span>
<span data-ttu-id="c66c0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c66c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c66c0-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c66c0-113">Permission type</span></span>                        | <span data-ttu-id="c66c0-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c66c0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c66c0-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c66c0-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="c66c0-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c66c0-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c66c0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c66c0-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c66c0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c66c0-118">Not supported.</span></span>|
|<span data-ttu-id="c66c0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c66c0-119">Application</span></span>                            |<span data-ttu-id="c66c0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c66c0-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c66c0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c66c0-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="c66c0-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c66c0-122">Request headers</span></span>

| <span data-ttu-id="c66c0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c66c0-123">Name</span></span>           | <span data-ttu-id="c66c0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c66c0-124">Type</span></span>    | <span data-ttu-id="c66c0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c66c0-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c66c0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c66c0-126">Authorization</span></span>  | <span data-ttu-id="c66c0-127">string</span><span class="sxs-lookup"><span data-stu-id="c66c0-127">string</span></span>  | <span data-ttu-id="c66c0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c66c0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c66c0-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c66c0-130">Request body</span></span>

<span data-ttu-id="c66c0-131">В тексте запроса добавьте представление объекта [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c66c0-131">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="c66c0-132">Единственное обязательное свойство — `templateId`.</span><span class="sxs-lookup"><span data-stu-id="c66c0-132">The only required property is `templateId`.</span></span> <span data-ttu-id="c66c0-133">`templateId` Свойство должно быть соответствующим одному из шаблонов, созданных для этого приложения или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="c66c0-133">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="c66c0-134">Чтобы найти доступные шаблоны, используйте [шаблоны списков](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="c66c0-134">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="c66c0-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c66c0-135">Response</span></span>

<span data-ttu-id="c66c0-136">В случае успеха возвращает код `201 Created` отклика и объект [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c66c0-136">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c66c0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c66c0-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c66c0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c66c0-138">Request</span></span>
<span data-ttu-id="c66c0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c66c0-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c66c0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c66c0-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c66c0-141">C#</span><span class="sxs-lookup"><span data-stu-id="c66c0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c66c0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c66c0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c66c0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c66c0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c66c0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c66c0-144">Response</span></span>
<span data-ttu-id="c66c0-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c66c0-145">The following is an example of a response.</span></span> 

><span data-ttu-id="c66c0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c66c0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
