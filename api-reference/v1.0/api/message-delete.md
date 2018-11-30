---
title: Удаление сообщения
description: Удалить сообщение в почтовый ящик указанного пользователя или отношения сообщения.
ms.openlocfilehash: 5bfcb57f3f9c82f79147c30c982f59172e48b51f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027495"
---
# <a name="delete-message"></a><span data-ttu-id="3a367-103">Удаление сообщения</span><span class="sxs-lookup"><span data-stu-id="3a367-103">Delete message</span></span>

<span data-ttu-id="3a367-104">Удалить сообщение в почтовый ящик указанного пользователя или отношения сообщения.</span><span class="sxs-lookup"><span data-stu-id="3a367-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="3a367-105">**Примечание** Можно не удалять элементы в папке восстанавливаемый удалений (представленное [имя папки известных](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="3a367-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="3a367-106">Для получения дополнительных сведений см [хранения удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="3a367-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a367-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a367-107">Permissions</span></span>
<span data-ttu-id="3a367-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a367-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a367-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a367-110">Permission type</span></span>      | <span data-ttu-id="3a367-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a367-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a367-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a367-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a367-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a367-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a367-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a367-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a367-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a367-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a367-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a367-116">Application</span></span> | <span data-ttu-id="3a367-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a367-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a367-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a367-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3a367-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a367-119">Request headers</span></span>
| <span data-ttu-id="3a367-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3a367-120">Name</span></span>       | <span data-ttu-id="3a367-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3a367-121">Type</span></span> | <span data-ttu-id="3a367-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3a367-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a367-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a367-123">Authorization</span></span>  | <span data-ttu-id="3a367-124">string</span><span class="sxs-lookup"><span data-stu-id="3a367-124">string</span></span>  | <span data-ttu-id="3a367-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a367-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a367-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a367-127">Request body</span></span>
<span data-ttu-id="3a367-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a367-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a367-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a367-129">Response</span></span>

<span data-ttu-id="3a367-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3a367-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a367-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3a367-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a367-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a367-133">Request</span></span>
<span data-ttu-id="3a367-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a367-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="3a367-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a367-135">Response</span></span>
<span data-ttu-id="3a367-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a367-136">Here is an example of the response.</span></span> 
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