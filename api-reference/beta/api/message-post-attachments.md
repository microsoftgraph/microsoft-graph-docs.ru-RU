---
title: Добавление вложения
description: 'С помощью этого API можно добавить вложение к сообщению. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6374677a1f93e655220b56de31f8f76cbc1d72e8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447979"
---
# <a name="add-attachment"></a><span data-ttu-id="75339-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="75339-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75339-104">С помощью этого API можно добавить [вложение](../resources/attachment.md) к сообщению.</span><span class="sxs-lookup"><span data-stu-id="75339-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="75339-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="75339-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="75339-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="75339-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="75339-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="75339-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="75339-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="75339-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="75339-109">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="75339-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="75339-110">Вложение можно добавить к существующему сообщению, добавив его в коллекцию вложений или в новое сообщение, которое будет [черновиком](../api/user-post-messages.md)или [создано и отправлено на ходу](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="75339-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="75339-111">Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="75339-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="75339-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75339-112">Permissions</span></span>
<span data-ttu-id="75339-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75339-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75339-115">Permission type</span></span>      | <span data-ttu-id="75339-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75339-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75339-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75339-117">Delegated (work or school account)</span></span> | <span data-ttu-id="75339-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75339-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="75339-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75339-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75339-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75339-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="75339-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75339-121">Application</span></span> | <span data-ttu-id="75339-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75339-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="75339-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75339-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="75339-124">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="75339-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="75339-125">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="75339-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="75339-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="75339-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="75339-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75339-128">Request headers</span></span>
| <span data-ttu-id="75339-129">Имя</span><span class="sxs-lookup"><span data-stu-id="75339-129">Name</span></span>       | <span data-ttu-id="75339-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75339-130">Type</span></span> | <span data-ttu-id="75339-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75339-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75339-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="75339-132">Authorization</span></span>  | <span data-ttu-id="75339-133">string</span><span class="sxs-lookup"><span data-stu-id="75339-133">string</span></span>  | <span data-ttu-id="75339-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75339-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75339-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75339-136">Content-Type</span></span> | <span data-ttu-id="75339-137">string</span><span class="sxs-lookup"><span data-stu-id="75339-137">string</span></span>  | <span data-ttu-id="75339-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75339-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75339-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75339-140">Request body</span></span>
<span data-ttu-id="75339-141">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75339-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="75339-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="75339-142">Response</span></span>

<span data-ttu-id="75339-143">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [вложения](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75339-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="75339-144">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="75339-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="75339-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="75339-145">Request</span></span>
<span data-ttu-id="75339-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75339-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75339-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="75339-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "a0b1c76de9f7="
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75339-148">C#</span><span class="sxs-lookup"><span data-stu-id="75339-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75339-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="75339-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75339-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="75339-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="75339-151">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75339-151">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="75339-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="75339-152">Response</span></span>
<span data-ttu-id="75339-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75339-153">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 201 Created
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
    "contentBytes": "a0b1c76de9f7="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="75339-154">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="75339-154">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="75339-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="75339-155">Request</span></span>
<span data-ttu-id="75339-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75339-156">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkpsDRVK/attachments
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


##### <a name="response"></a><span data-ttu-id="75339-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="75339-157">Response</span></span>
<span data-ttu-id="75339-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75339-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="example-reference-attachment"></a><span data-ttu-id="75339-161">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="75339-161">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="75339-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="75339-162">Request</span></span>
<span data-ttu-id="75339-163">Ниже приведен пример запроса, который добавляет к существующему сообщению ссылку с вложением.</span><span class="sxs-lookup"><span data-stu-id="75339-163">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="75339-164">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="75339-164">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75339-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="75339-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_message",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M88AADUv0uFAAA=/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75339-166">C#</span><span class="sxs-lookup"><span data-stu-id="75339-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75339-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="75339-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75339-168">Цель — C</span><span class="sxs-lookup"><span data-stu-id="75339-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="75339-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="75339-169">Response</span></span>
<span data-ttu-id="75339-170">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="75339-170">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/messages/AAMkAGE1M88AADUv0uFAAA%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_file_attachment_from_message/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'a0b1c76de9f7='"
  ]
}
-->
