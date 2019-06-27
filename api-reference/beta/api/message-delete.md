---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d1df6b9d9b1b01d2960c12ce7cee1a927843626f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266089"
---
# <a name="delete-message"></a><span data-ttu-id="c0d03-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="c0d03-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d03-104">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="c0d03-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="c0d03-105">Например, вы можете удалить из сообщения указанного [](../resources/mention.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="c0d03-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="c0d03-106">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным [именем](../resources/mailfolder.md) `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="c0d03-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="c0d03-107">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="c0d03-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0d03-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0d03-108">Permissions</span></span>
<span data-ttu-id="c0d03-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0d03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0d03-111">Permission type</span></span>      | <span data-ttu-id="c0d03-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0d03-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0d03-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0d03-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c0d03-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0d03-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c0d03-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0d03-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d03-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0d03-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c0d03-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0d03-117">Application</span></span> | <span data-ttu-id="c0d03-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0d03-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0d03-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0d03-119">HTTP request</span></span>

<span data-ttu-id="c0d03-120">Удаление указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="c0d03-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="c0d03-121">Чтобы удалить определенное [упоминание](../resources/mention.md) в сообщении, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="c0d03-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0d03-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0d03-122">Request headers</span></span>
| <span data-ttu-id="c0d03-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c0d03-123">Name</span></span>       | <span data-ttu-id="c0d03-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c0d03-124">Type</span></span> | <span data-ttu-id="c0d03-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c0d03-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0d03-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0d03-126">Authorization</span></span>  | <span data-ttu-id="c0d03-127">string</span><span class="sxs-lookup"><span data-stu-id="c0d03-127">string</span></span>  | <span data-ttu-id="c0d03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0d03-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0d03-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0d03-130">Request body</span></span>
<span data-ttu-id="c0d03-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0d03-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0d03-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0d03-132">Response</span></span>

<span data-ttu-id="c0d03-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c0d03-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0d03-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c0d03-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c0d03-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c0d03-136">Request 1</span></span>
<span data-ttu-id="c0d03-137">В первом примере показано, как удалить указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="c0d03-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="c0d03-138">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="c0d03-138">Response 1</span></span>
<span data-ttu-id="c0d03-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0d03-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c0d03-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c0d03-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c0d03-141">C#</span><span class="sxs-lookup"><span data-stu-id="c0d03-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0d03-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0d03-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c0d03-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c0d03-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="c0d03-144">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="c0d03-144">Request 2</span></span>
<span data-ttu-id="c0d03-145">В следующем примере показано, как \*\*\*\* удалить определенное упоминание из указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="c0d03-145">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="c0d03-146">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="c0d03-146">Response 2</span></span>
<span data-ttu-id="c0d03-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0d03-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c0d03-148">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c0d03-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c0d03-149">C#</span><span class="sxs-lookup"><span data-stu-id="c0d03-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0d03-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0d03-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c0d03-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c0d03-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
