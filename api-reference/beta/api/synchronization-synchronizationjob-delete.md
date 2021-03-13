---
title: Удаление синхронизацииJob
description: Остановите задание синхронизации и удалите навсегда все связанное с ним состояние.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d4b154cca11b46c53d6929ea9522a7ff36c3b908
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50773580"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="bb88d-103">Удаление синхронизацииJob</span><span class="sxs-lookup"><span data-stu-id="bb88d-103">Delete synchronizationJob</span></span>

<span data-ttu-id="bb88d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb88d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb88d-105">Остановите задание синхронизации и удалите навсегда все связанное с ним состояние.</span><span class="sxs-lookup"><span data-stu-id="bb88d-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="bb88d-106">Синхронизированные учетные записи оставлены как есть.</span><span class="sxs-lookup"><span data-stu-id="bb88d-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb88d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb88d-107">Permissions</span></span>
<span data-ttu-id="bb88d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb88d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb88d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb88d-110">Permission type</span></span>                        | <span data-ttu-id="bb88d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb88d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb88d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb88d-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="bb88d-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb88d-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bb88d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb88d-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bb88d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb88d-115">Not supported.</span></span>  |
|<span data-ttu-id="bb88d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb88d-116">Application</span></span>                            |<span data-ttu-id="bb88d-117">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb88d-117">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bb88d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb88d-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="bb88d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb88d-119">Request headers</span></span>

| <span data-ttu-id="bb88d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bb88d-120">Name</span></span>           | <span data-ttu-id="bb88d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bb88d-121">Type</span></span>    | <span data-ttu-id="bb88d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bb88d-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bb88d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb88d-123">Authorization</span></span>  | <span data-ttu-id="bb88d-124">string</span><span class="sxs-lookup"><span data-stu-id="bb88d-124">string</span></span>  | <span data-ttu-id="bb88d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb88d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb88d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb88d-127">Request body</span></span>

<span data-ttu-id="bb88d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb88d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb88d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb88d-129">Response</span></span>

<span data-ttu-id="bb88d-130">В случае успешного ответа `204 No Content` возвращается ответ.</span><span class="sxs-lookup"><span data-stu-id="bb88d-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="bb88d-131">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bb88d-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb88d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bb88d-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bb88d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb88d-133">Request</span></span>
<span data-ttu-id="bb88d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb88d-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb88d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb88d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="bb88d-136">C#</span><span class="sxs-lookup"><span data-stu-id="bb88d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb88d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb88d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb88d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb88d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb88d-139">Java</span><span class="sxs-lookup"><span data-stu-id="bb88d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb88d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb88d-140">Response</span></span>
<span data-ttu-id="bb88d-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bb88d-141">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


