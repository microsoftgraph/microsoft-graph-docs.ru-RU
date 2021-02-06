---
title: Список вложений
description: Получение списка объектов attachment, вложенных в сообщение.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 681c845f25e8bfa92749f5ec2e976b1404490b11
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131210"
---
# <a name="list-attachments"></a><span data-ttu-id="2301c-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="2301c-103">List attachments</span></span>

<span data-ttu-id="2301c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2301c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2301c-105">Получение списка объектов [attachment](../resources/attachment.md), вложенных в сообщение.</span><span class="sxs-lookup"><span data-stu-id="2301c-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="2301c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2301c-106">Permissions</span></span>
<span data-ttu-id="2301c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2301c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2301c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2301c-109">Permission type</span></span>      | <span data-ttu-id="2301c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2301c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2301c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2301c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2301c-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2301c-112">Mail.Read</span></span>    |
|<span data-ttu-id="2301c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2301c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2301c-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2301c-114">Mail.Read</span></span>    |
|<span data-ttu-id="2301c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2301c-115">Application</span></span> | <span data-ttu-id="2301c-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2301c-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="2301c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2301c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2301c-118">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2301c-118">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="2301c-119">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2301c-119">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="2301c-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="2301c-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2301c-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2301c-122">Optional query parameters</span></span>
<span data-ttu-id="2301c-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2301c-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="2301c-124">В частности, можно использовать параметр $expand, чтобы включить все вложения в сообщения вместе с остальными свойствами сообщения.</span><span class="sxs-lookup"><span data-stu-id="2301c-124">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="2301c-125">Например:</span><span class="sxs-lookup"><span data-stu-id="2301c-125">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="2301c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2301c-126">Request headers</span></span>
| <span data-ttu-id="2301c-127">Имя</span><span class="sxs-lookup"><span data-stu-id="2301c-127">Name</span></span>       | <span data-ttu-id="2301c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="2301c-128">Type</span></span> | <span data-ttu-id="2301c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2301c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2301c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2301c-130">Authorization</span></span>  | <span data-ttu-id="2301c-131">string</span><span class="sxs-lookup"><span data-stu-id="2301c-131">string</span></span>  | <span data-ttu-id="2301c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2301c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2301c-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2301c-134">Request body</span></span>
<span data-ttu-id="2301c-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2301c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2301c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2301c-136">Response</span></span>

<span data-ttu-id="2301c-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2301c-137">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2301c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2301c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2301c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2301c-139">Request</span></span>
<span data-ttu-id="2301c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2301c-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2301c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2301c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments_beta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="2301c-142">C#</span><span class="sxs-lookup"><span data-stu-id="2301c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2301c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2301c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2301c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2301c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2301c-145">Java</span><span class="sxs-lookup"><span data-stu-id="2301c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-attachments-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2301c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2301c-146">Response</span></span>
<span data-ttu-id="2301c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2301c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "message_get_attachments_beta",
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
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
