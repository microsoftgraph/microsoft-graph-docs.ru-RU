---
title: Добавление вложения
description: 'С помощью этого API можно добавить вложение к сообщению. '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0d282afb127dba1222f208d0660e6ff584c22834
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052238"
---
# <a name="add-attachment"></a><span data-ttu-id="19269-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="19269-103">Add attachment</span></span>

<span data-ttu-id="19269-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19269-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19269-105">С помощью этого API можно добавить [вложение](../resources/attachment.md) к сообщению.</span><span class="sxs-lookup"><span data-stu-id="19269-105">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="19269-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="19269-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="19269-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="19269-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="19269-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="19269-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="19269-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="19269-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="19269-110">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="19269-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="19269-111">Вы можете добавить вложение к существующему сообщению, добавив его в коллекцию вложений, или к сообщению, [создаваемому и отправляемому на ходу](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="19269-111">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="19269-112">Эта операция ограничивает размер вложения, который можно добавить до 3 МБ.</span><span class="sxs-lookup"><span data-stu-id="19269-112">This operation limits the size of the attachment you can add to under 3 MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="19269-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19269-113">Permissions</span></span>
<span data-ttu-id="19269-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19269-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19269-116">Permission type</span></span>      | <span data-ttu-id="19269-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19269-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19269-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19269-118">Delegated (work or school account)</span></span> | <span data-ttu-id="19269-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19269-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="19269-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19269-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19269-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19269-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="19269-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19269-122">Application</span></span> | <span data-ttu-id="19269-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19269-123">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="19269-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19269-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="19269-125">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="19269-125">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="19269-126">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="19269-126">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="19269-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="19269-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="19269-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19269-129">Request headers</span></span>
| <span data-ttu-id="19269-130">Имя</span><span class="sxs-lookup"><span data-stu-id="19269-130">Name</span></span>       | <span data-ttu-id="19269-131">Тип</span><span class="sxs-lookup"><span data-stu-id="19269-131">Type</span></span> | <span data-ttu-id="19269-132">Описание</span><span class="sxs-lookup"><span data-stu-id="19269-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19269-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="19269-133">Authorization</span></span>  | <span data-ttu-id="19269-134">string</span><span class="sxs-lookup"><span data-stu-id="19269-134">string</span></span>  | <span data-ttu-id="19269-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19269-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19269-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19269-137">Content-Type</span></span> | <span data-ttu-id="19269-138">string</span><span class="sxs-lookup"><span data-stu-id="19269-138">string</span></span>  | <span data-ttu-id="19269-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19269-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19269-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19269-141">Request body</span></span>
<span data-ttu-id="19269-142">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19269-142">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="19269-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="19269-143">Response</span></span>

<span data-ttu-id="19269-144">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="19269-144">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="19269-145">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="19269-145">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="19269-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="19269-146">Request</span></span>
<span data-ttu-id="19269-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19269-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19269-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="19269-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message_v1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```
# <a name="c"></a>[<span data-ttu-id="19269-149">C#</span><span class="sxs-lookup"><span data-stu-id="19269-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19269-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19269-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19269-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19269-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19269-152">Java</span><span class="sxs-lookup"><span data-stu-id="19269-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-message-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="19269-153">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19269-153">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="19269-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="19269-154">Response</span></span>
<span data-ttu-id="19269-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19269-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_message_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 202

{
    "id": "AAMkADNkN2R",
    "lastModifiedDateTime": "2017-01-26T08:48:28Z",
    "name": "smile",
    "contentType": "image/gif",
    "size": 1008,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="19269-156">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="19269-156">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="19269-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="19269-157">Request</span></span>
<span data-ttu-id="19269-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19269-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "create_item_attachment_from_message_v1"
}-->

```
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
    "@odata.type": "microsoft.graph.event",
    "subject": "Discuss gifts for children",
    "body": {
      "contentType": "HTML",
      "content": "Let's look for funding!"
    },
    "start": {
      "dateTime": "2016-12-02T18:00:00",
      "timeZone": "Pacific Standard Time"
    },
    "end": {
      "dateTime": "2016-12-02T19:00:00",
      "timeZone": "Pacific Standard Time"
    }
  }
}
```


##### <a name="response"></a><span data-ttu-id="19269-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="19269-159">Response</span></span>
<span data-ttu-id="19269-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19269-160">Here is an example of the response.</span></span> <span data-ttu-id="19269-161">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="19269-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_message_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "id":"AAMkADNkNJp5JVnQIe9r0=",
  "lastModifiedDateTime":"2016-12-01T22:27:13Z",
  "name":"Holiday event",
  "contentType":null,
  "size":2473,
  "isInline":false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

