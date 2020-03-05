---
title: Удаление Синчронизатионжоб
description: Остановите задание синхронизации и окончательно удалите все связанные с ним состояния. Синхронизированные учетные записи остаются недоступными.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2c346b1020250cb1e46aa9f3c2b57f9fd5b1f1ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453027"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="ad879-104">Удаление Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="ad879-104">Delete synchronizationJob</span></span>

<span data-ttu-id="ad879-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ad879-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad879-106">Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.</span><span class="sxs-lookup"><span data-stu-id="ad879-106">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="ad879-107">Синхронизированные учетные записи остаются недоступными.</span><span class="sxs-lookup"><span data-stu-id="ad879-107">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad879-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad879-108">Permissions</span></span>
<span data-ttu-id="ad879-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad879-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad879-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad879-111">Permission type</span></span>                        | <span data-ttu-id="ad879-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad879-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad879-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad879-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="ad879-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad879-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ad879-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad879-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ad879-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad879-116">Not supported.</span></span>  |
|<span data-ttu-id="ad879-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad879-117">Application</span></span>                            |<span data-ttu-id="ad879-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad879-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ad879-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad879-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="ad879-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad879-120">Request headers</span></span>

| <span data-ttu-id="ad879-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ad879-121">Name</span></span>           | <span data-ttu-id="ad879-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ad879-122">Type</span></span>    | <span data-ttu-id="ad879-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ad879-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ad879-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad879-124">Authorization</span></span>  | <span data-ttu-id="ad879-125">string</span><span class="sxs-lookup"><span data-stu-id="ad879-125">string</span></span>  | <span data-ttu-id="ad879-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad879-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad879-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad879-128">Request body</span></span>

<span data-ttu-id="ad879-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad879-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad879-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad879-130">Response</span></span>

<span data-ttu-id="ad879-131">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="ad879-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="ad879-132">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ad879-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad879-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ad879-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ad879-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad879-134">Request</span></span>
<span data-ttu-id="ad879-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad879-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad879-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad879-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="ad879-137">C#</span><span class="sxs-lookup"><span data-stu-id="ad879-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad879-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad879-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad879-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad879-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ad879-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad879-140">Response</span></span>
<span data-ttu-id="ad879-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad879-141">The following is an example of the response.</span></span> 

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
