---
title: Список вложений
description: Получение списка объектов attachment, вложенных в сообщение.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7a8e6c6a3586ecc030f725c96c385376daf2f4a2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054562"
---
# <a name="list-attachments"></a><span data-ttu-id="6b079-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="6b079-103">List attachments</span></span>

<span data-ttu-id="6b079-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b079-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b079-105">Получение списка объектов [attachment](../resources/attachment.md), вложенных в сообщение.</span><span class="sxs-lookup"><span data-stu-id="6b079-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b079-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b079-106">Permissions</span></span>
<span data-ttu-id="6b079-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b079-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b079-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b079-109">Permission type</span></span>      | <span data-ttu-id="6b079-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b079-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b079-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b079-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b079-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b079-112">Mail.Read</span></span>    |
|<span data-ttu-id="6b079-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b079-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b079-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b079-114">Mail.Read</span></span>    |
|<span data-ttu-id="6b079-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b079-115">Application</span></span> | <span data-ttu-id="6b079-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b079-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b079-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b079-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6b079-118">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b079-118">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="6b079-119">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b079-119">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="6b079-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="6b079-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b079-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6b079-122">Optional query parameters</span></span>
<span data-ttu-id="6b079-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6b079-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6b079-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b079-124">Request headers</span></span>
| <span data-ttu-id="6b079-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6b079-125">Name</span></span>       | <span data-ttu-id="6b079-126">Тип</span><span class="sxs-lookup"><span data-stu-id="6b079-126">Type</span></span> | <span data-ttu-id="6b079-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6b079-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b079-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b079-128">Authorization</span></span>  | <span data-ttu-id="6b079-129">string</span><span class="sxs-lookup"><span data-stu-id="6b079-129">string</span></span>  | <span data-ttu-id="6b079-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b079-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b079-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b079-132">Request body</span></span>
<span data-ttu-id="6b079-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b079-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b079-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b079-134">Response</span></span>

<span data-ttu-id="6b079-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b079-135">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b079-136">Пример</span><span class="sxs-lookup"><span data-stu-id="6b079-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b079-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b079-137">Request</span></span>
<span data-ttu-id="6b079-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b079-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b079-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b079-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="6b079-140">C#</span><span class="sxs-lookup"><span data-stu-id="6b079-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b079-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b079-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b079-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b079-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b079-143">Java</span><span class="sxs-lookup"><span data-stu-id="6b079-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b079-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b079-144">Response</span></span>
<span data-ttu-id="6b079-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b079-145">Here is an example of the response.</span></span> <span data-ttu-id="6b079-146">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b079-146">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "message_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
