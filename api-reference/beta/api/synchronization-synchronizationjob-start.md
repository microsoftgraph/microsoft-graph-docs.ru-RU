---
title: Запустите synchronizationJob
description: Запустите существующее задание синхронизации. Если задание находится в приостановленном состоянии, он будет предоставляться обработки изменений из точки, где он был приостановлен. Если задание находится в карантине, будут очищены состояние карантина.
ms.openlocfilehash: c9f326a2c00564f25fb0ff982ede7e8454e14c8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081702"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="d185e-105">Запустите synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="d185e-105">Start synchronizationJob</span></span>

> <span data-ttu-id="d185e-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d185e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d185e-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d185e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d185e-108">Запустите существующее задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d185e-108">Start an existing synchronization job.</span></span> <span data-ttu-id="d185e-109">Если задание находится в приостановленном состоянии, он будет предоставляться обработки изменений из точки, где он был приостановлен.</span><span class="sxs-lookup"><span data-stu-id="d185e-109">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="d185e-110">Если задание находится в карантине, будут очищены состояние карантина.</span><span class="sxs-lookup"><span data-stu-id="d185e-110">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="d185e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d185e-111">Permissions</span></span>
<span data-ttu-id="d185e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d185e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d185e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d185e-114">Permission type</span></span>                        | <span data-ttu-id="d185e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d185e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d185e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d185e-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="d185e-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d185e-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d185e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d185e-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d185e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d185e-119">Not supported.</span></span> |
|<span data-ttu-id="d185e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d185e-120">Application</span></span>                            |<span data-ttu-id="d185e-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d185e-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d185e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d185e-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="d185e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d185e-123">Request headers</span></span>

| <span data-ttu-id="d185e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d185e-124">Name</span></span>           | <span data-ttu-id="d185e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d185e-125">Type</span></span>    | <span data-ttu-id="d185e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d185e-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d185e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d185e-127">Authorization</span></span>  | <span data-ttu-id="d185e-128">string</span><span class="sxs-lookup"><span data-stu-id="d185e-128">string</span></span>  | <span data-ttu-id="d185e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d185e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d185e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d185e-131">Request body</span></span>

<span data-ttu-id="d185e-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d185e-132">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="d185e-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="d185e-133">Response</span></span>

<span data-ttu-id="d185e-134">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="d185e-134">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="d185e-135">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d185e-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d185e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d185e-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d185e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d185e-137">Request</span></span>
<span data-ttu-id="d185e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d185e-138">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="d185e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d185e-139">Response</span></span>
<span data-ttu-id="d185e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d185e-140">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
