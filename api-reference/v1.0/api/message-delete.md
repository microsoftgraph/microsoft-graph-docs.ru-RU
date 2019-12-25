---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b0e1d62dfe82c79f154a39a18d7878636687d1af
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864672"
---
# <a name="delete-message"></a><span data-ttu-id="220cf-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="220cf-103">Delete message</span></span>

<span data-ttu-id="220cf-104">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="220cf-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="220cf-105">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено [известным именем](../resources/mailfolder.md) `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="220cf-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="220cf-106">Дополнительные сведения см. в статье [Хранение удаленных](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="220cf-106">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="220cf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="220cf-107">Permissions</span></span>
<span data-ttu-id="220cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="220cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="220cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="220cf-110">Permission type</span></span>      | <span data-ttu-id="220cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="220cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="220cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="220cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="220cf-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="220cf-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="220cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="220cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="220cf-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="220cf-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="220cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="220cf-116">Application</span></span> | <span data-ttu-id="220cf-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="220cf-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="220cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="220cf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="220cf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="220cf-119">Request headers</span></span>
| <span data-ttu-id="220cf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="220cf-120">Name</span></span>       | <span data-ttu-id="220cf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="220cf-121">Type</span></span> | <span data-ttu-id="220cf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="220cf-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="220cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="220cf-123">Authorization</span></span>  | <span data-ttu-id="220cf-124">string</span><span class="sxs-lookup"><span data-stu-id="220cf-124">string</span></span>  | <span data-ttu-id="220cf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="220cf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="220cf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="220cf-127">Request body</span></span>
<span data-ttu-id="220cf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="220cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="220cf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="220cf-129">Response</span></span>

<span data-ttu-id="220cf-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="220cf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="220cf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="220cf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="220cf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="220cf-133">Request</span></span>
<span data-ttu-id="220cf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="220cf-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="220cf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="220cf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="220cf-136">C#</span><span class="sxs-lookup"><span data-stu-id="220cf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="220cf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="220cf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="220cf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="220cf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="220cf-139">Java</span><span class="sxs-lookup"><span data-stu-id="220cf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="220cf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="220cf-140">Response</span></span>
<span data-ttu-id="220cf-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="220cf-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
