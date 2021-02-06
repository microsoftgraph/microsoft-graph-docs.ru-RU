---
title: Запуск synchronizationJob
description: Запустите существующее задание синхронизации. Если задание приостановлено, оно продолжит обработку изменений с момента приостановки. Если задание находится в карантине, состояние карантина будет очищено.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1fae704446d35c7a93d850f25f31355f50d332e0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132771"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="bcf39-105">Запуск synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="bcf39-105">Start synchronizationJob</span></span>

<span data-ttu-id="bcf39-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcf39-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf39-107">Запустите существующее задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bcf39-107">Start an existing synchronization job.</span></span> <span data-ttu-id="bcf39-108">Если задание приостановлено, оно продолжит обработку изменений с момента приостановки.</span><span class="sxs-lookup"><span data-stu-id="bcf39-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="bcf39-109">Если задание находится в карантине, состояние карантина будет очищено.</span><span class="sxs-lookup"><span data-stu-id="bcf39-109">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcf39-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf39-110">Permissions</span></span>
<span data-ttu-id="bcf39-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf39-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcf39-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf39-113">Permission type</span></span>                        | <span data-ttu-id="bcf39-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcf39-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcf39-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcf39-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="bcf39-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf39-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bcf39-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcf39-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bcf39-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf39-118">Not supported.</span></span> |
|<span data-ttu-id="bcf39-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcf39-119">Application</span></span>                            |<span data-ttu-id="bcf39-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf39-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bcf39-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcf39-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="bcf39-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bcf39-122">Request headers</span></span>

| <span data-ttu-id="bcf39-123">Имя</span><span class="sxs-lookup"><span data-stu-id="bcf39-123">Name</span></span>           | <span data-ttu-id="bcf39-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bcf39-124">Type</span></span>    | <span data-ttu-id="bcf39-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf39-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bcf39-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcf39-126">Authorization</span></span>  | <span data-ttu-id="bcf39-127">string</span><span class="sxs-lookup"><span data-stu-id="bcf39-127">string</span></span>  | <span data-ttu-id="bcf39-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcf39-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcf39-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcf39-130">Request body</span></span>

<span data-ttu-id="bcf39-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcf39-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="bcf39-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf39-132">Response</span></span>

<span data-ttu-id="bcf39-133">В случае успеха возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="bcf39-133">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="bcf39-134">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bcf39-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcf39-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bcf39-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bcf39-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcf39-136">Request</span></span>
<span data-ttu-id="bcf39-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcf39-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcf39-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcf39-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="bcf39-139">C#</span><span class="sxs-lookup"><span data-stu-id="bcf39-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcf39-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcf39-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcf39-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcf39-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcf39-142">Java</span><span class="sxs-lookup"><span data-stu-id="bcf39-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bcf39-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf39-143">Response</span></span>
<span data-ttu-id="bcf39-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bcf39-144">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


