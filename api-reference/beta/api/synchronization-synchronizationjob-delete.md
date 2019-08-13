---
title: Удаление Синчронизатионжоб
description: Остановите задание синхронизации и окончательно удалите все связанные с ним состояния. Синхронизированные учетные записи остаются недоступными.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39c6af0cf6acf69fc03641a3fb3722ac7b850702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363580"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="c98b8-104">Удаление Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="c98b8-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c98b8-105">Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.</span><span class="sxs-lookup"><span data-stu-id="c98b8-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="c98b8-106">Синхронизированные учетные записи остаются недоступными.</span><span class="sxs-lookup"><span data-stu-id="c98b8-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="c98b8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c98b8-107">Permissions</span></span>
<span data-ttu-id="c98b8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c98b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c98b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c98b8-110">Permission type</span></span>                        | <span data-ttu-id="c98b8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c98b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c98b8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c98b8-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="c98b8-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c98b8-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c98b8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c98b8-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c98b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c98b8-115">Not supported.</span></span>  |
|<span data-ttu-id="c98b8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c98b8-116">Application</span></span>                            |<span data-ttu-id="c98b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c98b8-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c98b8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c98b8-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="c98b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c98b8-119">Request headers</span></span>

| <span data-ttu-id="c98b8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c98b8-120">Name</span></span>           | <span data-ttu-id="c98b8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c98b8-121">Type</span></span>    | <span data-ttu-id="c98b8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c98b8-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c98b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c98b8-123">Authorization</span></span>  | <span data-ttu-id="c98b8-124">string</span><span class="sxs-lookup"><span data-stu-id="c98b8-124">string</span></span>  | <span data-ttu-id="c98b8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c98b8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c98b8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c98b8-127">Request body</span></span>

<span data-ttu-id="c98b8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c98b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c98b8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c98b8-129">Response</span></span>

<span data-ttu-id="c98b8-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="c98b8-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="c98b8-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c98b8-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c98b8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c98b8-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c98b8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c98b8-133">Request</span></span>
<span data-ttu-id="c98b8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c98b8-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c98b8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c98b8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c98b8-136">C#</span><span class="sxs-lookup"><span data-stu-id="c98b8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c98b8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c98b8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c98b8-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c98b8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c98b8-139">Java</span><span class="sxs-lookup"><span data-stu-id="c98b8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c98b8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c98b8-140">Response</span></span>
<span data-ttu-id="c98b8-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c98b8-141">The following is an example of the response.</span></span> 

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
