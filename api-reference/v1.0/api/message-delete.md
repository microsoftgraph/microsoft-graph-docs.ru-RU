---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b944cb586b7da4580cf8242b25275e7e70e518e7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275672"
---
# <a name="delete-message"></a><span data-ttu-id="25ef7-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="25ef7-103">Delete message</span></span>

<span data-ttu-id="25ef7-104">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="25ef7-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="25ef7-105">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным [именем](../resources/mailfolder.md) `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="25ef7-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="25ef7-106">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="25ef7-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="25ef7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25ef7-107">Permissions</span></span>
<span data-ttu-id="25ef7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25ef7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25ef7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25ef7-110">Permission type</span></span>      | <span data-ttu-id="25ef7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25ef7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25ef7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25ef7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="25ef7-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25ef7-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="25ef7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25ef7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25ef7-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25ef7-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="25ef7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25ef7-116">Application</span></span> | <span data-ttu-id="25ef7-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25ef7-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="25ef7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25ef7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="25ef7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25ef7-119">Request headers</span></span>
| <span data-ttu-id="25ef7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="25ef7-120">Name</span></span>       | <span data-ttu-id="25ef7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="25ef7-121">Type</span></span> | <span data-ttu-id="25ef7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="25ef7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25ef7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="25ef7-123">Authorization</span></span>  | <span data-ttu-id="25ef7-124">string</span><span class="sxs-lookup"><span data-stu-id="25ef7-124">string</span></span>  | <span data-ttu-id="25ef7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25ef7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25ef7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25ef7-127">Request body</span></span>
<span data-ttu-id="25ef7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25ef7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25ef7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="25ef7-129">Response</span></span>

<span data-ttu-id="25ef7-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="25ef7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25ef7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="25ef7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25ef7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="25ef7-133">Request</span></span>
<span data-ttu-id="25ef7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25ef7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="25ef7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ef7-135">Response</span></span>
<span data-ttu-id="25ef7-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25ef7-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="25ef7-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="25ef7-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="25ef7-138">C#</span><span class="sxs-lookup"><span data-stu-id="25ef7-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25ef7-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="25ef7-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="25ef7-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="25ef7-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
