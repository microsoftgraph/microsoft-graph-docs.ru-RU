---
title: Удаление Синчронизатионжоб
description: Остановите задание синхронизации и окончательно удалите все связанные с ним состояния. Синхронизированные учетные записи остаются недоступными.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a179e8b61d6cafb63b143a392c5543b566644325
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991130"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="75153-104">Удаление Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="75153-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75153-105">Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.</span><span class="sxs-lookup"><span data-stu-id="75153-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="75153-106">Синхронизированные учетные записи остаются недоступными.</span><span class="sxs-lookup"><span data-stu-id="75153-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="75153-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75153-107">Permissions</span></span>
<span data-ttu-id="75153-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75153-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75153-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75153-110">Permission type</span></span>                        | <span data-ttu-id="75153-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75153-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="75153-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75153-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="75153-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75153-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="75153-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75153-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="75153-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75153-115">Not supported.</span></span>  |
|<span data-ttu-id="75153-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75153-116">Application</span></span>                            |<span data-ttu-id="75153-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75153-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="75153-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75153-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="75153-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75153-119">Request headers</span></span>

| <span data-ttu-id="75153-120">Имя</span><span class="sxs-lookup"><span data-stu-id="75153-120">Name</span></span>           | <span data-ttu-id="75153-121">Тип</span><span class="sxs-lookup"><span data-stu-id="75153-121">Type</span></span>    | <span data-ttu-id="75153-122">Описание</span><span class="sxs-lookup"><span data-stu-id="75153-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="75153-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75153-123">Authorization</span></span>  | <span data-ttu-id="75153-124">string</span><span class="sxs-lookup"><span data-stu-id="75153-124">string</span></span>  | <span data-ttu-id="75153-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75153-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75153-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75153-127">Request body</span></span>

<span data-ttu-id="75153-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75153-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75153-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="75153-129">Response</span></span>

<span data-ttu-id="75153-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="75153-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="75153-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="75153-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75153-132">Пример</span><span class="sxs-lookup"><span data-stu-id="75153-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="75153-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="75153-133">Request</span></span>
<span data-ttu-id="75153-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75153-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75153-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="75153-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75153-136">C#</span><span class="sxs-lookup"><span data-stu-id="75153-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75153-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="75153-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75153-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="75153-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="75153-139">Java</span><span class="sxs-lookup"><span data-stu-id="75153-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="75153-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="75153-140">Response</span></span>
<span data-ttu-id="75153-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75153-141">The following is an example of the response.</span></span> 

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
