---
title: Запуск Синчронизатионжоб
description: Запуск существующего задания синхронизации. Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено. Если задание находится в карантине, состояние карантина будет очищено.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d85a371db7b86010bf3aaf81b3b91837b8546d0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978858"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="e3a72-105">Запуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="e3a72-105">Start synchronizationJob</span></span>

<span data-ttu-id="e3a72-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3a72-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3a72-107">Запуск существующего задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e3a72-107">Start an existing synchronization job.</span></span> <span data-ttu-id="e3a72-108">Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено.</span><span class="sxs-lookup"><span data-stu-id="e3a72-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="e3a72-109">Если задание находится в карантине, состояние карантина будет очищено.</span><span class="sxs-lookup"><span data-stu-id="e3a72-109">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3a72-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3a72-110">Permissions</span></span>
<span data-ttu-id="e3a72-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3a72-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3a72-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3a72-113">Permission type</span></span>                        | <span data-ttu-id="e3a72-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3a72-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3a72-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3a72-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="e3a72-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a72-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e3a72-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3a72-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e3a72-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a72-118">Not supported.</span></span> |
|<span data-ttu-id="e3a72-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3a72-119">Application</span></span>                            |<span data-ttu-id="e3a72-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a72-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e3a72-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3a72-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="e3a72-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e3a72-122">Request headers</span></span>

| <span data-ttu-id="e3a72-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e3a72-123">Name</span></span>           | <span data-ttu-id="e3a72-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e3a72-124">Type</span></span>    | <span data-ttu-id="e3a72-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e3a72-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e3a72-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3a72-126">Authorization</span></span>  | <span data-ttu-id="e3a72-127">string</span><span class="sxs-lookup"><span data-stu-id="e3a72-127">string</span></span>  | <span data-ttu-id="e3a72-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3a72-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3a72-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3a72-130">Request body</span></span>

<span data-ttu-id="e3a72-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3a72-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="e3a72-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3a72-132">Response</span></span>

<span data-ttu-id="e3a72-133">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="e3a72-133">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="e3a72-134">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3a72-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3a72-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e3a72-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e3a72-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3a72-136">Request</span></span>
<span data-ttu-id="e3a72-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3a72-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3a72-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3a72-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="e3a72-139">C#</span><span class="sxs-lookup"><span data-stu-id="e3a72-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3a72-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3a72-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3a72-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3a72-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3a72-142">Java</span><span class="sxs-lookup"><span data-stu-id="e3a72-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3a72-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3a72-143">Response</span></span>
<span data-ttu-id="e3a72-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3a72-144">The following is an example of a response.</span></span>
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


