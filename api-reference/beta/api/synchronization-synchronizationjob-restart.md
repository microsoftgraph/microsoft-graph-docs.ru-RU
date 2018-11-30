---
title: Перезапустите synchronizationJob
description: Перезапустите задание синхронизации, заставить его повторно обработать все объекты в каталоге. При необходимости удаляет существующие состояние синхронизации и предыдущих ошибок.
ms.openlocfilehash: 0b7ebfcd7b13400225d9ea149442207ecd994a8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081052"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="e454c-104">Перезапустите synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="e454c-104">Restart synchronizationJob</span></span>

> <span data-ttu-id="e454c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e454c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e454c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e454c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e454c-107">Перезапустите задание синхронизации, заставить его повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="e454c-107">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="e454c-108">При необходимости удаляет существующие состояние синхронизации и предыдущих ошибок.</span><span class="sxs-lookup"><span data-stu-id="e454c-108">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="e454c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e454c-109">Permissions</span></span>
<span data-ttu-id="e454c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e454c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e454c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e454c-112">Permission type</span></span>                        | <span data-ttu-id="e454c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e454c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e454c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e454c-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="e454c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e454c-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e454c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e454c-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e454c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e454c-117">Not supported.</span></span> |
|<span data-ttu-id="e454c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e454c-118">Application</span></span>                            |<span data-ttu-id="e454c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e454c-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e454c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e454c-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="e454c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e454c-121">Request headers</span></span>

| <span data-ttu-id="e454c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e454c-122">Name</span></span>           | <span data-ttu-id="e454c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e454c-123">Type</span></span>    | <span data-ttu-id="e454c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e454c-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e454c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e454c-125">Authorization</span></span>  | <span data-ttu-id="e454c-126">string</span><span class="sxs-lookup"><span data-stu-id="e454c-126">string</span></span>  | <span data-ttu-id="e454c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e454c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e454c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e454c-129">Request body</span></span>

<span data-ttu-id="e454c-130">Предоставить объект JSON в тексте запроса следующий параметр.</span><span class="sxs-lookup"><span data-stu-id="e454c-130">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="e454c-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="e454c-131">Parameter</span></span>     | <span data-ttu-id="e454c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e454c-132">Type</span></span>      | <span data-ttu-id="e454c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e454c-133">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="e454c-134">criteria</span><span class="sxs-lookup"><span data-stu-id="e454c-134">criteria</span></span>       |[<span data-ttu-id="e454c-135">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="e454c-135">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="e454c-136">Перезапустите критериев</span><span class="sxs-lookup"><span data-stu-id="e454c-136">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="e454c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e454c-137">Response</span></span>

<span data-ttu-id="e454c-138">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="e454c-138">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="e454c-139">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e454c-139">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e454c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e454c-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e454c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e454c-141">Request</span></span>
<span data-ttu-id="e454c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e454c-142">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```

##### <a name="response"></a><span data-ttu-id="e454c-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="e454c-143">Response</span></span>
<span data-ttu-id="e454c-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e454c-144">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
