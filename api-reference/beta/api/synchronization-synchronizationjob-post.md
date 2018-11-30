---
title: Создание synchronizationJob
description: Создание нового задания синхронизации со схемой по умолчанию синхронизации. Задание будет создан в отключенном состоянии. Вызов запуска задания, чтобы запустить синхронизацию.
ms.openlocfilehash: 3c7e3c3a9c89f95b031cd45d38848e0f2f451de7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081938"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="cc730-105">Создание synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="cc730-105">Create synchronizationJob</span></span>

> <span data-ttu-id="cc730-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc730-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc730-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc730-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc730-108">Создание нового задания синхронизации со схемой по умолчанию синхронизации.</span><span class="sxs-lookup"><span data-stu-id="cc730-108">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="cc730-109">Задание будет создан в отключенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="cc730-109">The job is created in a disabled state.</span></span> <span data-ttu-id="cc730-110">Вызов, [запуска заданий](synchronization-synchronizationjob-start.md) для запуска синхронизации.</span><span class="sxs-lookup"><span data-stu-id="cc730-110">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc730-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc730-111">Permissions</span></span>
<span data-ttu-id="cc730-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc730-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc730-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc730-114">Permission type</span></span>                        | <span data-ttu-id="cc730-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc730-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc730-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc730-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="cc730-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc730-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cc730-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc730-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cc730-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc730-119">Not supported.</span></span>|
|<span data-ttu-id="cc730-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc730-120">Application</span></span>                            |<span data-ttu-id="cc730-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc730-121">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="cc730-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc730-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="cc730-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc730-123">Request headers</span></span>

| <span data-ttu-id="cc730-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cc730-124">Name</span></span>           | <span data-ttu-id="cc730-125">Тип</span><span class="sxs-lookup"><span data-stu-id="cc730-125">Type</span></span>    | <span data-ttu-id="cc730-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cc730-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cc730-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc730-127">Authorization</span></span>  | <span data-ttu-id="cc730-128">string</span><span class="sxs-lookup"><span data-stu-id="cc730-128">string</span></span>  | <span data-ttu-id="cc730-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc730-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc730-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc730-131">Request body</span></span>

<span data-ttu-id="cc730-132">В тексте запроса укажите представление объекта [synchronizationJob](../resources/synchronization-synchronizationjob.md) будет создан с JSON.</span><span class="sxs-lookup"><span data-stu-id="cc730-132">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="cc730-133">Является единственным обязательным свойством `templateId`.</span><span class="sxs-lookup"><span data-stu-id="cc730-133">The only required property is `templateId`.</span></span> <span data-ttu-id="cc730-134">`templateId` Свойство должно соответствовать одному из шаблонов, которые созданы для участника-службы и приложения.</span><span class="sxs-lookup"><span data-stu-id="cc730-134">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="cc730-135">Чтобы найти доступные шаблоны, используйте [Шаблоны списков](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="cc730-135">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="cc730-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc730-136">Response</span></span>

<span data-ttu-id="cc730-137">В случае успеха возвращает `201 Created` код ответа и объект [synchronizationJob](../resources/synchronization-synchronizationjob.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cc730-137">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc730-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cc730-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cc730-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc730-139">Request</span></span>
<span data-ttu-id="cc730-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc730-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cc730-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc730-141">Response</span></span>
<span data-ttu-id="cc730-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cc730-142">The following is an example of a response.</span></span> 

><span data-ttu-id="cc730-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc730-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->