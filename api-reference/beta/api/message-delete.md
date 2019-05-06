---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0c221b08d895bcc19ebbb87996b8ef3c5f3c029a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598639"
---
# <a name="delete-message"></a><span data-ttu-id="9f641-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="9f641-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f641-104">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="9f641-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="9f641-105">Например, вы можете удалить из сообщения указанного [](../resources/mention.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f641-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="9f641-106">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным [именем](../resources/mailfolder.md) `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="9f641-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="9f641-107">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="9f641-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f641-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f641-108">Permissions</span></span>
<span data-ttu-id="9f641-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f641-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f641-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f641-111">Permission type</span></span>      | <span data-ttu-id="9f641-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f641-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f641-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f641-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9f641-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f641-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f641-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f641-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f641-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f641-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f641-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f641-117">Application</span></span> | <span data-ttu-id="9f641-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f641-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f641-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f641-119">HTTP request</span></span>

<span data-ttu-id="9f641-120">Удаление указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="9f641-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="9f641-121">Чтобы удалить определенное [упоминание](../resources/mention.md) в сообщении, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="9f641-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f641-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f641-122">Request headers</span></span>
| <span data-ttu-id="9f641-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9f641-123">Name</span></span>       | <span data-ttu-id="9f641-124">Тип</span><span class="sxs-lookup"><span data-stu-id="9f641-124">Type</span></span> | <span data-ttu-id="9f641-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9f641-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f641-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f641-126">Authorization</span></span>  | <span data-ttu-id="9f641-127">string</span><span class="sxs-lookup"><span data-stu-id="9f641-127">string</span></span>  | <span data-ttu-id="9f641-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f641-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f641-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f641-130">Request body</span></span>
<span data-ttu-id="9f641-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f641-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f641-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f641-132">Response</span></span>

<span data-ttu-id="9f641-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9f641-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f641-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9f641-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9f641-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="9f641-136">Request 1</span></span>
<span data-ttu-id="9f641-137">В первом примере показано, как удалить указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="9f641-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="9f641-138">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="9f641-138">Response 1</span></span>
<span data-ttu-id="9f641-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f641-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9f641-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9f641-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9f641-141">Языках</span><span class="sxs-lookup"><span data-stu-id="9f641-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f641-142">Язык</span><span class="sxs-lookup"><span data-stu-id="9f641-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="9f641-143">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="9f641-143">Request 2</span></span>
<span data-ttu-id="9f641-144">В следующем примере показано, как \*\*\*\* удалить определенное упоминание из указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="9f641-144">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="9f641-145">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="9f641-145">Response 2</span></span>
<span data-ttu-id="9f641-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9f641-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9f641-147">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9f641-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9f641-148">Языках</span><span class="sxs-lookup"><span data-stu-id="9f641-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f641-149">Язык</span><span class="sxs-lookup"><span data-stu-id="9f641-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
