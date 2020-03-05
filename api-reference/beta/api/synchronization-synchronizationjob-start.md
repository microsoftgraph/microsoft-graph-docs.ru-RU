---
title: Запуск Синчронизатионжоб
description: Запуск существующего задания синхронизации. Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено. Если задание находится в карантине, состояние карантина будет очищено.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 65587fe7675f905685dfb4c2044a670222899df9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452976"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="f5d4d-105">Запуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="f5d4d-105">Start synchronizationJob</span></span>

<span data-ttu-id="f5d4d-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5d4d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5d4d-107">Запуск существующего задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-107">Start an existing synchronization job.</span></span> <span data-ttu-id="f5d4d-108">Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="f5d4d-109">Если задание находится в карантине, состояние карантина будет очищено.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-109">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5d4d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d4d-110">Permissions</span></span>
<span data-ttu-id="f5d4d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5d4d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5d4d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d4d-113">Permission type</span></span>                        | <span data-ttu-id="f5d4d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5d4d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5d4d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5d4d-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="f5d4d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5d4d-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f5d4d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5d4d-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f5d4d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-118">Not supported.</span></span> |
|<span data-ttu-id="f5d4d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5d4d-119">Application</span></span>                            |<span data-ttu-id="f5d4d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f5d4d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5d4d-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="f5d4d-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5d4d-122">Request headers</span></span>

| <span data-ttu-id="f5d4d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f5d4d-123">Name</span></span>           | <span data-ttu-id="f5d4d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f5d4d-124">Type</span></span>    | <span data-ttu-id="f5d4d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f5d4d-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f5d4d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5d4d-126">Authorization</span></span>  | <span data-ttu-id="f5d4d-127">string</span><span class="sxs-lookup"><span data-stu-id="f5d4d-127">string</span></span>  | <span data-ttu-id="f5d4d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5d4d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5d4d-130">Request body</span></span>

<span data-ttu-id="f5d4d-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="f5d4d-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5d4d-132">Response</span></span>

<span data-ttu-id="f5d4d-133">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-133">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="f5d4d-134">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5d4d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f5d4d-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f5d4d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5d4d-136">Request</span></span>
<span data-ttu-id="f5d4d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5d4d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5d4d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="f5d4d-139">C#</span><span class="sxs-lookup"><span data-stu-id="f5d4d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5d4d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5d4d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5d4d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5d4d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f5d4d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5d4d-142">Response</span></span>
<span data-ttu-id="f5d4d-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5d4d-143">The following is an example of a response.</span></span>
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
