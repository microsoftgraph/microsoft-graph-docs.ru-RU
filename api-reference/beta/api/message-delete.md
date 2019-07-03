---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cd4141dbf6ab8f55990ff494fc61167f1ea8758c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448252"
---
# <a name="delete-message"></a><span data-ttu-id="1677c-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="1677c-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1677c-104">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="1677c-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="1677c-105">Например, вы можете удалить из сообщения указанного [](../resources/mention.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="1677c-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="1677c-106">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным [именем](../resources/mailfolder.md) `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="1677c-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="1677c-107">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="1677c-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="1677c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1677c-108">Permissions</span></span>
<span data-ttu-id="1677c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1677c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1677c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1677c-111">Permission type</span></span>      | <span data-ttu-id="1677c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1677c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1677c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1677c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1677c-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1677c-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1677c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1677c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1677c-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1677c-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1677c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1677c-117">Application</span></span> | <span data-ttu-id="1677c-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1677c-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1677c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1677c-119">HTTP request</span></span>

<span data-ttu-id="1677c-120">Удаление указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="1677c-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="1677c-121">Чтобы удалить определенное [упоминание](../resources/mention.md) в сообщении, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1677c-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1677c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1677c-122">Request headers</span></span>
| <span data-ttu-id="1677c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1677c-123">Name</span></span>       | <span data-ttu-id="1677c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1677c-124">Type</span></span> | <span data-ttu-id="1677c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1677c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1677c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1677c-126">Authorization</span></span>  | <span data-ttu-id="1677c-127">string</span><span class="sxs-lookup"><span data-stu-id="1677c-127">string</span></span>  | <span data-ttu-id="1677c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1677c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1677c-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1677c-130">Request body</span></span>
<span data-ttu-id="1677c-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1677c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1677c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1677c-132">Response</span></span>

<span data-ttu-id="1677c-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1677c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1677c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="1677c-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="1677c-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="1677c-136">Request 1</span></span>
<span data-ttu-id="1677c-137">В первом примере показано, как удалить указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="1677c-137">The first example deletes the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1677c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1677c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1677c-139">C#</span><span class="sxs-lookup"><span data-stu-id="1677c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1677c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="1677c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1677c-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1677c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="1677c-142">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="1677c-142">Response 1</span></span>
<span data-ttu-id="1677c-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1677c-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="1677c-144">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="1677c-144">Request 2</span></span>
<span data-ttu-id="1677c-145">В следующем примере показано, как \*\*\*\* удалить определенное упоминание из указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="1677c-145">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1677c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1677c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1677c-147">C#</span><span class="sxs-lookup"><span data-stu-id="1677c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1677c-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="1677c-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1677c-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1677c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="1677c-150">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="1677c-150">Response 2</span></span>
<span data-ttu-id="1677c-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1677c-151">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
