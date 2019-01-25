---
title: Создание synchronizationJob
description: Создание нового задания синхронизации со схемой по умолчанию синхронизации. Задание будет создан в отключенном состоянии. Вызов запуска задания, чтобы запустить синхронизацию.
localization_priority: Normal
ms.openlocfilehash: f41ebe87d8ca935a355c37ea53d1c7bd62b1652e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507917"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="5273e-105">Создание synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5273e-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5273e-106">Создание нового задания синхронизации со схемой по умолчанию синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5273e-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="5273e-107">Задание будет создан в отключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="5273e-107">The job is created in a disabled state.</span></span> <span data-ttu-id="5273e-108">Вызов, [запуска заданий](synchronization-synchronizationjob-start.md) для запуска синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5273e-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="5273e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5273e-109">Permissions</span></span>
<span data-ttu-id="5273e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5273e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5273e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5273e-112">Permission type</span></span>                        | <span data-ttu-id="5273e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5273e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5273e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5273e-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="5273e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5273e-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5273e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5273e-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5273e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5273e-117">Not supported.</span></span>|
|<span data-ttu-id="5273e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5273e-118">Application</span></span>                            |<span data-ttu-id="5273e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5273e-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5273e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5273e-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="5273e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5273e-121">Request headers</span></span>

| <span data-ttu-id="5273e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5273e-122">Name</span></span>           | <span data-ttu-id="5273e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5273e-123">Type</span></span>    | <span data-ttu-id="5273e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5273e-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5273e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5273e-125">Authorization</span></span>  | <span data-ttu-id="5273e-126">string</span><span class="sxs-lookup"><span data-stu-id="5273e-126">string</span></span>  | <span data-ttu-id="5273e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5273e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5273e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5273e-129">Request body</span></span>

<span data-ttu-id="5273e-130">В тексте запроса укажите представление объекта [synchronizationJob](../resources/synchronization-synchronizationjob.md) будет создан с JSON.</span><span class="sxs-lookup"><span data-stu-id="5273e-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="5273e-131">Является единственным обязательным свойством `templateId`.</span><span class="sxs-lookup"><span data-stu-id="5273e-131">The only required property is `templateId`.</span></span> <span data-ttu-id="5273e-132">`templateId` Свойство должно соответствовать одному из шаблонов, которые созданы для участника-службы и приложения.</span><span class="sxs-lookup"><span data-stu-id="5273e-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="5273e-133">Чтобы найти доступные шаблоны, используйте [Шаблоны списков](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="5273e-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="5273e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5273e-134">Response</span></span>

<span data-ttu-id="5273e-135">В случае успеха возвращает `201 Created` код ответа и объект [synchronizationJob](../resources/synchronization-synchronizationjob.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5273e-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5273e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5273e-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5273e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5273e-137">Request</span></span>
<span data-ttu-id="5273e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5273e-138">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5273e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5273e-139">Response</span></span>
<span data-ttu-id="5273e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5273e-140">The following is an example of a response.</span></span> 

><span data-ttu-id="5273e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5273e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
