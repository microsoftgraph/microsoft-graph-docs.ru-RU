---
title: Создание Синчронизатионжоб
description: Создайте новое задание синхронизации с схемой синхронизации по умолчанию. Задание создано в отключенном состоянии. Запустите задание запуска, чтобы начать синхронизацию.
localization_priority: Normal
ms.openlocfilehash: 342364d9b3a2213c2ffdb686c9349700471a84da
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271353"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="6ef04-105">Создание Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="6ef04-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ef04-106">Создайте новое задание синхронизации с схемой синхронизации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6ef04-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="6ef04-107">Задание создано в отключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="6ef04-107">The job is created in a disabled state.</span></span> <span data-ttu-id="6ef04-108">Запустите [Задание запуска](synchronization-synchronizationjob-start.md) , чтобы начать синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="6ef04-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ef04-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef04-109">Permissions</span></span>
<span data-ttu-id="6ef04-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ef04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ef04-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef04-112">Permission type</span></span>                        | <span data-ttu-id="6ef04-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ef04-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ef04-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ef04-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="6ef04-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ef04-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6ef04-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ef04-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6ef04-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef04-117">Not supported.</span></span>|
|<span data-ttu-id="6ef04-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ef04-118">Application</span></span>                            |<span data-ttu-id="6ef04-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef04-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="6ef04-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ef04-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="6ef04-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ef04-121">Request headers</span></span>

| <span data-ttu-id="6ef04-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6ef04-122">Name</span></span>           | <span data-ttu-id="6ef04-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6ef04-123">Type</span></span>    | <span data-ttu-id="6ef04-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef04-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6ef04-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ef04-125">Authorization</span></span>  | <span data-ttu-id="6ef04-126">string</span><span class="sxs-lookup"><span data-stu-id="6ef04-126">string</span></span>  | <span data-ttu-id="6ef04-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ef04-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ef04-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ef04-129">Request body</span></span>

<span data-ttu-id="6ef04-130">В тексте запроса добавьте представление объекта [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ef04-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="6ef04-131">Единственное обязательное свойство — `templateId`.</span><span class="sxs-lookup"><span data-stu-id="6ef04-131">The only required property is `templateId`.</span></span> <span data-ttu-id="6ef04-132">`templateId` Свойство должно быть соответствующим одному из шаблонов, созданных для этого приложения или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="6ef04-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="6ef04-133">Чтобы найти доступные шаблоны, используйте [шаблоны списков](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="6ef04-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="6ef04-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ef04-134">Response</span></span>

<span data-ttu-id="6ef04-135">В случае успеха возвращает код `201 Created` отклика и объект [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ef04-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ef04-136">Пример</span><span class="sxs-lookup"><span data-stu-id="6ef04-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6ef04-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ef04-137">Request</span></span>
<span data-ttu-id="6ef04-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ef04-138">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6ef04-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ef04-139">Response</span></span>
<span data-ttu-id="6ef04-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ef04-140">The following is an example of a response.</span></span> 

><span data-ttu-id="6ef04-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ef04-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ef04-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6ef04-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6ef04-144">C#</span><span class="sxs-lookup"><span data-stu-id="6ef04-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ef04-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ef04-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6ef04-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6ef04-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
