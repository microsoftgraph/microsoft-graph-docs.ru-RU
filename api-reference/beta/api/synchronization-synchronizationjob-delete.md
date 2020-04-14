---
title: Удаление Синчронизатионжоб
description: Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd732200b8ab02be3bffc443272a45f2da8a9a77
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466436"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="5d4f0-103">Удаление Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="5d4f0-103">Delete synchronizationJob</span></span>

<span data-ttu-id="5d4f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d4f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d4f0-105">Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="5d4f0-106">Синхронизированные учетные записи остаются недоступными.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d4f0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d4f0-107">Permissions</span></span>
<span data-ttu-id="5d4f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d4f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d4f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d4f0-110">Permission type</span></span>                        | <span data-ttu-id="5d4f0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d4f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d4f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d4f0-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="5d4f0-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d4f0-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5d4f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d4f0-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5d4f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-115">Not supported.</span></span>  |
|<span data-ttu-id="5d4f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d4f0-116">Application</span></span>                            |<span data-ttu-id="5d4f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5d4f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d4f0-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="5d4f0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5d4f0-119">Request headers</span></span>

| <span data-ttu-id="5d4f0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5d4f0-120">Name</span></span>           | <span data-ttu-id="5d4f0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5d4f0-121">Type</span></span>    | <span data-ttu-id="5d4f0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5d4f0-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5d4f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d4f0-123">Authorization</span></span>  | <span data-ttu-id="5d4f0-124">string</span><span class="sxs-lookup"><span data-stu-id="5d4f0-124">string</span></span>  | <span data-ttu-id="5d4f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d4f0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d4f0-127">Request body</span></span>

<span data-ttu-id="5d4f0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d4f0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d4f0-129">Response</span></span>

<span data-ttu-id="5d4f0-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="5d4f0-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d4f0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5d4f0-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5d4f0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d4f0-133">Request</span></span>
<span data-ttu-id="5d4f0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d4f0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d4f0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="5d4f0-136">C#</span><span class="sxs-lookup"><span data-stu-id="5d4f0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d4f0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d4f0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d4f0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d4f0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d4f0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d4f0-139">Response</span></span>
<span data-ttu-id="5d4f0-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5d4f0-140">The following is an example of the response.</span></span> 

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
