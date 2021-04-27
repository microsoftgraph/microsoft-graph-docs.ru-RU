---
title: Создание синхронизацииJob
description: Создайте новое задание синхронизации с схемой синхронизации по умолчанию. Задание создается в состоянии отключения. Вызов Начните работу, чтобы начать синхронизацию.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6cab9a652d2902fce735b87b5cd249fd2a273786
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054821"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="a714b-105">Создание синхронизацииJob</span><span class="sxs-lookup"><span data-stu-id="a714b-105">Create synchronizationJob</span></span>

<span data-ttu-id="a714b-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a714b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a714b-107">Создайте новое задание синхронизации с схемой синхронизации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a714b-107">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="a714b-108">Задание создается в состоянии отключения.</span><span class="sxs-lookup"><span data-stu-id="a714b-108">The job is created in a disabled state.</span></span> <span data-ttu-id="a714b-109">Вызов [Начните работу,](synchronization-synchronizationjob-start.md) чтобы начать синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="a714b-109">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="a714b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a714b-110">Permissions</span></span>
<span data-ttu-id="a714b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a714b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a714b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a714b-113">Permission type</span></span>                        | <span data-ttu-id="a714b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a714b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a714b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a714b-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="a714b-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a714b-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a714b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a714b-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a714b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a714b-118">Not supported.</span></span>|
|<span data-ttu-id="a714b-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="a714b-119">Application</span></span>                            |<span data-ttu-id="a714b-120">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a714b-120">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="a714b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a714b-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="a714b-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a714b-122">Request headers</span></span>

| <span data-ttu-id="a714b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a714b-123">Name</span></span>           | <span data-ttu-id="a714b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a714b-124">Type</span></span>    | <span data-ttu-id="a714b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a714b-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a714b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a714b-126">Authorization</span></span>  | <span data-ttu-id="a714b-127">string</span><span class="sxs-lookup"><span data-stu-id="a714b-127">string</span></span>  | <span data-ttu-id="a714b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a714b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a714b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a714b-130">Request body</span></span>

<span data-ttu-id="a714b-131">В корпусе запроса создадим JSON-представление создаваемого объекта [синхронизацииJob.](../resources/synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="a714b-131">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="a714b-132">Единственное необходимое свойство `templateId` .</span><span class="sxs-lookup"><span data-stu-id="a714b-132">The only required property is `templateId`.</span></span> <span data-ttu-id="a714b-133">Свойство `templateId` должно соответствовать одному из шаблонов, созданных для этого основного приложения или службы.</span><span class="sxs-lookup"><span data-stu-id="a714b-133">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="a714b-134">Чтобы найти доступные шаблоны, используйте [шаблоны List.](synchronization-synchronizationtemplate-list.md)</span><span class="sxs-lookup"><span data-stu-id="a714b-134">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="a714b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a714b-135">Response</span></span>

<span data-ttu-id="a714b-136">В случае успешной работы возвращает код ответа и `201 Created` объект [синхронизацииJob](../resources/synchronization-synchronizationjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a714b-136">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a714b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a714b-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a714b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a714b-138">Request</span></span>
<span data-ttu-id="a714b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a714b-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a714b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a714b-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a714b-141">C#</span><span class="sxs-lookup"><span data-stu-id="a714b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a714b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a714b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a714b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a714b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a714b-144">Java</span><span class="sxs-lookup"><span data-stu-id="a714b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationjob-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a714b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a714b-145">Response</span></span>
<span data-ttu-id="a714b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a714b-146">The following is an example of a response.</span></span> 

><span data-ttu-id="a714b-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a714b-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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


