---
title: Добавление вложения
description: 'С помощью этого API можно добавить вложение к сообщению. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 05cdbdbc5cc044f30a3dd2f8ea63dcf6fac50222
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637569"
---
# <a name="add-attachment"></a><span data-ttu-id="a13a5-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="a13a5-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a13a5-104">С помощью этого API можно добавить [вложение](../resources/attachment.md) к сообщению.</span><span class="sxs-lookup"><span data-stu-id="a13a5-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="a13a5-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="a13a5-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="a13a5-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a13a5-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="a13a5-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a13a5-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="a13a5-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="a13a5-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="a13a5-109">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="a13a5-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="a13a5-110">Вложение можно добавить к существующему [сообщению](../resources/message.md) , добавив его в коллекцию вложений или в новое сообщение, которое будет [черновиком](../api/user-post-messages.md)или [создано и отправлено на ходу](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="a13a5-110">You can add an attachment to an existing [message](../resources/message.md) by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

><span data-ttu-id="a13a5-111">**Примечание**: Эта операция ограничит размер вложения, которое можно добавить в течение 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="a13a5-111">**Note**: This operation limits the size of the attachment you can add to under 4 MB.</span></span>
>
> <span data-ttu-id="a13a5-112">Однако при присоединении к сообщению файла, который находится в диапазоне от 3 МБ и 150MB, вы можете [создать сеанс отправки](attachment-createuploadsession.md) и итеративно отправлять диапазоны файлов, чтобы присоединить их.</span><span class="sxs-lookup"><span data-stu-id="a13a5-112">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="a13a5-113">В этом примере показано, как [прикрепить большие файлы к сообщениям Outlook](/graph/outlook-large-attachments) .</span><span class="sxs-lookup"><span data-stu-id="a13a5-113">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>
## <a name="permissions"></a><span data-ttu-id="a13a5-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a13a5-114">Permissions</span></span>
<span data-ttu-id="a13a5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a13a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a13a5-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a13a5-117">Permission type</span></span>      | <span data-ttu-id="a13a5-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a13a5-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a13a5-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a13a5-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a13a5-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a13a5-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a13a5-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a13a5-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a13a5-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a13a5-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a13a5-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a13a5-123">Application</span></span> | <span data-ttu-id="a13a5-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a13a5-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a13a5-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a13a5-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a13a5-126">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a13a5-126">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="a13a5-127">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a13a5-127">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="a13a5-p103">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="a13a5-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a13a5-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a13a5-130">Request headers</span></span>
| <span data-ttu-id="a13a5-131">Имя</span><span class="sxs-lookup"><span data-stu-id="a13a5-131">Name</span></span>       | <span data-ttu-id="a13a5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a13a5-132">Type</span></span> | <span data-ttu-id="a13a5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a13a5-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a13a5-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="a13a5-134">Authorization</span></span>  | <span data-ttu-id="a13a5-135">string</span><span class="sxs-lookup"><span data-stu-id="a13a5-135">string</span></span>  | <span data-ttu-id="a13a5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a13a5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a13a5-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a13a5-138">Content-Type</span></span> | <span data-ttu-id="a13a5-139">string</span><span class="sxs-lookup"><span data-stu-id="a13a5-139">string</span></span>  | <span data-ttu-id="a13a5-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a13a5-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a13a5-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a13a5-142">Request body</span></span>
<span data-ttu-id="a13a5-143">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a13a5-143">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a13a5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a13a5-144">Response</span></span>

<span data-ttu-id="a13a5-145">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [вложения](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a13a5-145">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a13a5-146">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="a13a5-146">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a13a5-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a13a5-147">Request</span></span>
<span data-ttu-id="a13a5-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a13a5-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a13a5-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="a13a5-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message_beta"
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a13a5-150">C#</span><span class="sxs-lookup"><span data-stu-id="a13a5-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a13a5-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a13a5-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a13a5-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a13a5-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a13a5-153">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a13a5-153">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a13a5-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="a13a5-154">Response</span></span>
<span data-ttu-id="a13a5-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a13a5-155">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_message_beta",
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

## <a name="example-item-attachment"></a><span data-ttu-id="a13a5-156">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="a13a5-156">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a13a5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="a13a5-157">Request</span></span>
<span data-ttu-id="a13a5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a13a5-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message_beta"
}-->

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


##### <a name="response"></a><span data-ttu-id="a13a5-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="a13a5-159">Response</span></span>
<span data-ttu-id="a13a5-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a13a5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_message_beta",
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

## <a name="example-reference-attachment"></a><span data-ttu-id="a13a5-163">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="a13a5-163">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a13a5-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="a13a5-164">Request</span></span>
<span data-ttu-id="a13a5-165">Ниже приведен пример запроса, который добавляет к существующему сообщению ссылку с вложением.</span><span class="sxs-lookup"><span data-stu-id="a13a5-165">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="a13a5-166">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a13a5-166">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a13a5-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="a13a5-167">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a13a5-168">C#</span><span class="sxs-lookup"><span data-stu-id="a13a5-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a13a5-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a13a5-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a13a5-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a13a5-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a13a5-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="a13a5-171">Response</span></span>
<span data-ttu-id="a13a5-172">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="a13a5-172">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_from_message",
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
  "tocPath": ""
}
-->
