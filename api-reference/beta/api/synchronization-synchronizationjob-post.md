---
title: Создание Синчронизатионжоб
description: Создайте новое задание синхронизации с схемой синхронизации по умолчанию. Задание создано в отключенном состоянии. Запустите задание запуска, чтобы начать синхронизацию.
localization_priority: Normal
ms.openlocfilehash: fa0c3e539d73ff9496a0d4d0e3af8ebeda75e839
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638034"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="ba0d0-105">Создание Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="ba0d0-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba0d0-106">Создайте новое задание синхронизации с схемой синхронизации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="ba0d0-107">Задание создано в отключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-107">The job is created in a disabled state.</span></span> <span data-ttu-id="ba0d0-108">Запустите [Задание запуска](synchronization-synchronizationjob-start.md) , чтобы начать синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba0d0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba0d0-109">Permissions</span></span>
<span data-ttu-id="ba0d0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba0d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba0d0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba0d0-112">Permission type</span></span>                        | <span data-ttu-id="ba0d0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba0d0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba0d0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba0d0-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="ba0d0-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba0d0-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ba0d0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba0d0-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ba0d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-117">Not supported.</span></span>|
|<span data-ttu-id="ba0d0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba0d0-118">Application</span></span>                            |<span data-ttu-id="ba0d0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ba0d0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba0d0-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="ba0d0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba0d0-121">Request headers</span></span>

| <span data-ttu-id="ba0d0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ba0d0-122">Name</span></span>           | <span data-ttu-id="ba0d0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ba0d0-123">Type</span></span>    | <span data-ttu-id="ba0d0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ba0d0-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ba0d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba0d0-125">Authorization</span></span>  | <span data-ttu-id="ba0d0-126">string</span><span class="sxs-lookup"><span data-stu-id="ba0d0-126">string</span></span>  | <span data-ttu-id="ba0d0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba0d0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba0d0-129">Request body</span></span>

<span data-ttu-id="ba0d0-130">В тексте запроса добавьте представление объекта [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="ba0d0-131">Единственное обязательное свойство — `templateId`.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-131">The only required property is `templateId`.</span></span> <span data-ttu-id="ba0d0-132">`templateId` Свойство должно быть соответствующим одному из шаблонов, созданных для этого приложения или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="ba0d0-133">Чтобы найти доступные шаблоны, используйте [шаблоны списков](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="ba0d0-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="ba0d0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba0d0-134">Response</span></span>

<span data-ttu-id="ba0d0-135">В случае успеха возвращает код `201 Created` отклика и объект [синчронизатионжоб](../resources/synchronization-synchronizationjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba0d0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ba0d0-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ba0d0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba0d0-137">Request</span></span>
<span data-ttu-id="ba0d0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-138">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ba0d0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba0d0-139">Response</span></span>
<span data-ttu-id="ba0d0-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-140">The following is an example of a response.</span></span> 

><span data-ttu-id="ba0d0-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ba0d0-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba0d0-142">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ba0d0-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ba0d0-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ba0d0-144">Языках</span><span class="sxs-lookup"><span data-stu-id="ba0d0-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba0d0-145">Язык</span><span class="sxs-lookup"><span data-stu-id="ba0d0-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
