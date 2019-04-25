---
title: Удаление сообщения
description: Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1237ba7e4aa5ab0439af9f07902705e7b4061374
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540551"
---
# <a name="delete-message"></a><span data-ttu-id="c6e01-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="c6e01-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6e01-104">Удаление сообщения из почтового ящика указанного пользователя или удаление связи сообщения.</span><span class="sxs-lookup"><span data-stu-id="c6e01-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="c6e01-105">Например, вы можете удалить из сообщения указанного [](../resources/mention.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6e01-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="c6e01-106">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным [именем](../resources/mailfolder.md) `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="c6e01-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="c6e01-107">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="c6e01-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6e01-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6e01-108">Permissions</span></span>
<span data-ttu-id="c6e01-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6e01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6e01-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6e01-111">Permission type</span></span>      | <span data-ttu-id="c6e01-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6e01-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6e01-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6e01-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6e01-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6e01-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6e01-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6e01-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6e01-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6e01-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c6e01-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6e01-117">Application</span></span> | <span data-ttu-id="c6e01-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6e01-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6e01-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6e01-119">HTTP request</span></span>

<span data-ttu-id="c6e01-120">Удаление указанного сообщения:</span><span class="sxs-lookup"><span data-stu-id="c6e01-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="c6e01-121">Чтобы удалить определенное [упоминание](../resources/mention.md) в сообщении, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="c6e01-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c6e01-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6e01-122">Request headers</span></span>
| <span data-ttu-id="c6e01-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c6e01-123">Name</span></span>       | <span data-ttu-id="c6e01-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c6e01-124">Type</span></span> | <span data-ttu-id="c6e01-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c6e01-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6e01-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6e01-126">Authorization</span></span>  | <span data-ttu-id="c6e01-127">string</span><span class="sxs-lookup"><span data-stu-id="c6e01-127">string</span></span>  | <span data-ttu-id="c6e01-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6e01-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6e01-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6e01-130">Request body</span></span>
<span data-ttu-id="c6e01-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6e01-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6e01-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6e01-132">Response</span></span>

<span data-ttu-id="c6e01-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c6e01-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6e01-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c6e01-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c6e01-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c6e01-136">Request 1</span></span>
<span data-ttu-id="c6e01-137">В первом примере показано, как удалить указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="c6e01-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="c6e01-138">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="c6e01-138">Response 1</span></span>
<span data-ttu-id="c6e01-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6e01-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="c6e01-140">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="c6e01-140">Request 2</span></span>
<span data-ttu-id="c6e01-141">В следующем примере показано, как \*\*\*\* удалить определенное упоминание из указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="c6e01-141">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="c6e01-142">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="c6e01-142">Response 2</span></span>
<span data-ttu-id="c6e01-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6e01-143">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/message-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
