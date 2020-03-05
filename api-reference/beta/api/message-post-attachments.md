---
title: Добавление вложения
description: 'С помощью этого API можно добавить вложение к сообщению. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7fb569124683ac20a442c75cdb002be6ae2615c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456938"
---
# <a name="add-attachment"></a><span data-ttu-id="a91d3-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="a91d3-103">Add attachment</span></span>

<span data-ttu-id="a91d3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a91d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a91d3-105">С помощью этого API можно добавить [вложение](../resources/attachment.md) к сообщению.</span><span class="sxs-lookup"><span data-stu-id="a91d3-105">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="a91d3-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="a91d3-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="a91d3-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a91d3-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="a91d3-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a91d3-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="a91d3-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="a91d3-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="a91d3-110">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="a91d3-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="a91d3-111">Вложение можно добавить к существующему [сообщению](../resources/message.md) , добавив его в коллекцию вложений или в новое сообщение, которое будет [черновиком](../api/user-post-messages.md)или [создано и отправлено на ходу](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="a91d3-111">You can add an attachment to an existing [message](../resources/message.md) by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

><span data-ttu-id="a91d3-112">**Примечание**. Эта операция ограничит размер вложения, которое можно добавить в разделе 3 МБ.</span><span class="sxs-lookup"><span data-stu-id="a91d3-112">**Note**: This operation limits the size of the attachment you can add to under 3 MB.</span></span>
>
> <span data-ttu-id="a91d3-113">Однако при присоединении к сообщению файла, который находится в диапазоне от 3 МБ и 150MB, вы можете [создать сеанс отправки](attachment-createuploadsession.md) и итеративно отправлять диапазоны файлов, чтобы присоединить их.</span><span class="sxs-lookup"><span data-stu-id="a91d3-113">However, if you're attaching to a message a file that is between 3MB and 150MB, you can [create an upload session](attachment-createuploadsession.md) and iteratively upload ranges of the file to attach it.</span></span> <span data-ttu-id="a91d3-114">В этом примере показано, как [прикрепить большие файлы к сообщениям Outlook](/graph/outlook-large-attachments) .</span><span class="sxs-lookup"><span data-stu-id="a91d3-114">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>
## <a name="permissions"></a><span data-ttu-id="a91d3-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a91d3-115">Permissions</span></span>
<span data-ttu-id="a91d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a91d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a91d3-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a91d3-118">Permission type</span></span>      | <span data-ttu-id="a91d3-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a91d3-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a91d3-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a91d3-120">Delegated (work or school account)</span></span> | <span data-ttu-id="a91d3-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a91d3-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a91d3-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a91d3-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a91d3-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a91d3-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a91d3-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a91d3-124">Application</span></span> | <span data-ttu-id="a91d3-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a91d3-125">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a91d3-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a91d3-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a91d3-127">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a91d3-127">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="a91d3-128">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a91d3-128">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="a91d3-p103">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="a91d3-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a91d3-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a91d3-131">Request headers</span></span>
| <span data-ttu-id="a91d3-132">Имя</span><span class="sxs-lookup"><span data-stu-id="a91d3-132">Name</span></span>       | <span data-ttu-id="a91d3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a91d3-133">Type</span></span> | <span data-ttu-id="a91d3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a91d3-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a91d3-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="a91d3-135">Authorization</span></span>  | <span data-ttu-id="a91d3-136">string</span><span class="sxs-lookup"><span data-stu-id="a91d3-136">string</span></span>  | <span data-ttu-id="a91d3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a91d3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a91d3-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a91d3-139">Content-Type</span></span> | <span data-ttu-id="a91d3-140">string</span><span class="sxs-lookup"><span data-stu-id="a91d3-140">string</span></span>  | <span data-ttu-id="a91d3-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a91d3-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a91d3-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a91d3-143">Request body</span></span>
<span data-ttu-id="a91d3-144">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a91d3-144">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a91d3-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91d3-145">Response</span></span>

<span data-ttu-id="a91d3-146">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [вложения](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a91d3-146">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a91d3-147">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="a91d3-147">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a91d3-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a91d3-148">Request</span></span>
<span data-ttu-id="a91d3-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a91d3-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a91d3-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a91d3-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a91d3-151">C#</span><span class="sxs-lookup"><span data-stu-id="a91d3-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-message-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a91d3-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a91d3-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-message-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a91d3-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a91d3-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-message-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a91d3-154">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a91d3-154">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a91d3-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="a91d3-155">Response</span></span>
<span data-ttu-id="a91d3-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a91d3-156">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="a91d3-157">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="a91d3-157">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a91d3-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a91d3-158">Request</span></span>
<span data-ttu-id="a91d3-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a91d3-159">Here is an example of the request.</span></span>

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


##### <a name="response"></a><span data-ttu-id="a91d3-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91d3-160">Response</span></span>
<span data-ttu-id="a91d3-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a91d3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="a91d3-164">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="a91d3-164">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a91d3-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="a91d3-165">Request</span></span>
<span data-ttu-id="a91d3-166">Ниже приведен пример запроса, который добавляет к существующему сообщению ссылку с вложением.</span><span class="sxs-lookup"><span data-stu-id="a91d3-166">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="a91d3-167">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a91d3-167">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="a91d3-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="a91d3-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a91d3-169">C#</span><span class="sxs-lookup"><span data-stu-id="a91d3-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a91d3-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a91d3-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a91d3-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a91d3-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a91d3-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91d3-172">Response</span></span>
<span data-ttu-id="a91d3-173">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="a91d3-173">Here is an example of a full response.</span></span>
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
