---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e128dd174e7b99a1d10060a1e9cfd6d70f2fc780
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43361812"
---
# <a name="delete-message"></a><span data-ttu-id="51c8a-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="51c8a-103">Delete message</span></span>

<span data-ttu-id="51c8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51c8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51c8a-105">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="51c8a-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="51c8a-106">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено [известным именем папки](../resources/mailfolder.md) `recoverableitemsdeletions` ).</span><span class="sxs-lookup"><span data-stu-id="51c8a-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="51c8a-107">Дополнительные сведения см. в статье [Хранение удаленных](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="51c8a-107">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="51c8a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51c8a-108">Permissions</span></span>
<span data-ttu-id="51c8a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51c8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51c8a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51c8a-111">Permission type</span></span>      | <span data-ttu-id="51c8a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51c8a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51c8a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51c8a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="51c8a-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51c8a-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51c8a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51c8a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51c8a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51c8a-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51c8a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51c8a-117">Application</span></span> | <span data-ttu-id="51c8a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51c8a-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="51c8a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51c8a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="51c8a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51c8a-120">Request headers</span></span>
| <span data-ttu-id="51c8a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="51c8a-121">Name</span></span>       | <span data-ttu-id="51c8a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="51c8a-122">Type</span></span> | <span data-ttu-id="51c8a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="51c8a-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51c8a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="51c8a-124">Authorization</span></span>  | <span data-ttu-id="51c8a-125">string</span><span class="sxs-lookup"><span data-stu-id="51c8a-125">string</span></span>  | <span data-ttu-id="51c8a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51c8a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51c8a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51c8a-128">Request body</span></span>
<span data-ttu-id="51c8a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51c8a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51c8a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="51c8a-130">Response</span></span>

<span data-ttu-id="51c8a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="51c8a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51c8a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="51c8a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51c8a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="51c8a-134">Request</span></span>
<span data-ttu-id="51c8a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51c8a-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51c8a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="51c8a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="51c8a-137">C#</span><span class="sxs-lookup"><span data-stu-id="51c8a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51c8a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51c8a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51c8a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51c8a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51c8a-140">Java</span><span class="sxs-lookup"><span data-stu-id="51c8a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="51c8a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="51c8a-141">Response</span></span>
<span data-ttu-id="51c8a-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51c8a-142">Here is an example of the response.</span></span>
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
