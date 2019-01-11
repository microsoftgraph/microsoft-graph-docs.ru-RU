---
title: Удаление сообщения
description: Удалить сообщение в почтовый ящик указанного пользователя или отношения сообщения.
localization_priority: Normal
ms.openlocfilehash: 3a76c936f72ebd238ee6d7a898dfd6a3e0356036
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864528"
---
# <a name="delete-message"></a><span data-ttu-id="7e63a-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="7e63a-103">Delete message</span></span>

> <span data-ttu-id="7e63a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7e63a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e63a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e63a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e63a-106">Удалить сообщение в почтовый ящик указанного пользователя или отношения сообщения.</span><span class="sxs-lookup"><span data-stu-id="7e63a-106">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="7e63a-107">Например можно удалить определенных [@ упоминание](../resources/mention.md) пользователя, указанный в сообщении.</span><span class="sxs-lookup"><span data-stu-id="7e63a-107">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="7e63a-108">**Примечание** Можно не удалять элементы в папке восстанавливаемый удалений (представленное [имя папки известных](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="7e63a-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="7e63a-109">Для получения дополнительных сведений см [хранения удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="7e63a-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e63a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e63a-110">Permissions</span></span>
<span data-ttu-id="7e63a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e63a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e63a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e63a-113">Permission type</span></span>      | <span data-ttu-id="7e63a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e63a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e63a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e63a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7e63a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e63a-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7e63a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e63a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e63a-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e63a-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7e63a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e63a-119">Application</span></span> | <span data-ttu-id="7e63a-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e63a-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e63a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e63a-121">HTTP request</span></span>

<span data-ttu-id="7e63a-122">Удаление указанного сообщения:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="7e63a-122">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="7e63a-123">Удаление конкретных [упомянуть](../resources/mention.md) в сообщении:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="7e63a-123">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e63a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e63a-124">Request headers</span></span>
| <span data-ttu-id="7e63a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="7e63a-125">Name</span></span>       | <span data-ttu-id="7e63a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="7e63a-126">Type</span></span> | <span data-ttu-id="7e63a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7e63a-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7e63a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e63a-128">Authorization</span></span>  | <span data-ttu-id="7e63a-129">string</span><span class="sxs-lookup"><span data-stu-id="7e63a-129">string</span></span>  | <span data-ttu-id="7e63a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e63a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e63a-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e63a-132">Request body</span></span>
<span data-ttu-id="7e63a-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e63a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e63a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e63a-134">Response</span></span>

<span data-ttu-id="7e63a-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7e63a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e63a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7e63a-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="7e63a-138">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="7e63a-138">Request 1</span></span>
<span data-ttu-id="7e63a-139">Первый пример удаляет указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="7e63a-139">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="7e63a-140">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="7e63a-140">Response 1</span></span>
<span data-ttu-id="7e63a-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e63a-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="7e63a-142">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="7e63a-142">Request 2</span></span>
<span data-ttu-id="7e63a-143">Следующий пример удаляет определенные **упомянуть** в указанное сообщение.</span><span class="sxs-lookup"><span data-stu-id="7e63a-143">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="7e63a-144">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="7e63a-144">Response 2</span></span>
<span data-ttu-id="7e63a-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e63a-145">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
