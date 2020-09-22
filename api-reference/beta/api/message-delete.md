---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 040161d10daa2eda171525fb61a2edd0cc049035
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027617"
---
# <a name="delete-message"></a><span data-ttu-id="575ad-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="575ad-103">Delete message</span></span>

<span data-ttu-id="575ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="575ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="575ad-105">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="575ad-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="575ad-106">Например, вы можете [удалить из сообщения](../resources/mention.md) указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="575ad-106">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="575ad-107">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено [известным именем папки](../resources/mailfolder.md) `recoverableitemsdeletions` ).</span><span class="sxs-lookup"><span data-stu-id="575ad-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="575ad-108">Дополнительные сведения см. в статье [Хранение удаленных](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="575ad-108">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="575ad-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="575ad-109">Permissions</span></span>
<span data-ttu-id="575ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="575ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="575ad-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="575ad-112">Permission type</span></span>      | <span data-ttu-id="575ad-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="575ad-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="575ad-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="575ad-114">Delegated (work or school account)</span></span> | <span data-ttu-id="575ad-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="575ad-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="575ad-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="575ad-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="575ad-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="575ad-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="575ad-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="575ad-118">Application</span></span> | <span data-ttu-id="575ad-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="575ad-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="575ad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="575ad-120">HTTP request</span></span>

<span data-ttu-id="575ad-121">Удаление указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="575ad-121">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="575ad-122">Чтобы удалить определенное [упоминание](../resources/mention.md) в сообщении, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="575ad-122">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="575ad-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="575ad-123">Request headers</span></span>
| <span data-ttu-id="575ad-124">Имя</span><span class="sxs-lookup"><span data-stu-id="575ad-124">Name</span></span>       | <span data-ttu-id="575ad-125">Тип</span><span class="sxs-lookup"><span data-stu-id="575ad-125">Type</span></span> | <span data-ttu-id="575ad-126">Описание</span><span class="sxs-lookup"><span data-stu-id="575ad-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="575ad-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="575ad-127">Authorization</span></span>  | <span data-ttu-id="575ad-128">string</span><span class="sxs-lookup"><span data-stu-id="575ad-128">string</span></span>  | <span data-ttu-id="575ad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="575ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="575ad-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="575ad-131">Request body</span></span>
<span data-ttu-id="575ad-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="575ad-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="575ad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="575ad-133">Response</span></span>

<span data-ttu-id="575ad-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="575ad-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="575ad-136">Пример</span><span class="sxs-lookup"><span data-stu-id="575ad-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="575ad-137">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="575ad-137">Request 1</span></span>
<span data-ttu-id="575ad-138">В первом примере показано, как удалить указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="575ad-138">The first example deletes the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="575ad-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="575ad-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="575ad-140">C#</span><span class="sxs-lookup"><span data-stu-id="575ad-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="575ad-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="575ad-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="575ad-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="575ad-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="575ad-143">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="575ad-143">Response 1</span></span>
<span data-ttu-id="575ad-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="575ad-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="575ad-145">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="575ad-145">Request 2</span></span>
<span data-ttu-id="575ad-146">В следующем примере показано, как удалить определенное **упоминание** из указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="575ad-146">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="575ad-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="575ad-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="c"></a>[<span data-ttu-id="575ad-148">C#</span><span class="sxs-lookup"><span data-stu-id="575ad-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="575ad-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="575ad-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="575ad-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="575ad-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="575ad-151">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="575ad-151">Response 2</span></span>
<span data-ttu-id="575ad-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="575ad-152">Here is an example of the response.</span></span>
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


