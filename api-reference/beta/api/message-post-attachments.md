---
title: Добавление вложения
description: 'С помощью этого API можно добавить вложение к сообщению. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 56693a04d6f0579d043b4d745fe53ae61536b82e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510094"
---
# <a name="add-attachment"></a><span data-ttu-id="4884c-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="4884c-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4884c-104">С помощью этого API можно добавить [вложение](../resources/attachment.md) к сообщению.</span><span class="sxs-lookup"><span data-stu-id="4884c-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="4884c-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="4884c-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="4884c-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4884c-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="4884c-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="4884c-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="4884c-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="4884c-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="4884c-109">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4884c-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="4884c-110">Можно добавить вложения в существующее сообщение, отправку сообщений в коллекцию вложения или в новое сообщение, который [черновик](../api/user-post-messages.md)или [создан и отправлен во время выполнения](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="4884c-110">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="4884c-111">Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="4884c-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="4884c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4884c-112">Permissions</span></span>
<span data-ttu-id="4884c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4884c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4884c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4884c-115">Permission type</span></span>      | <span data-ttu-id="4884c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4884c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4884c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4884c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4884c-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4884c-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4884c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4884c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4884c-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4884c-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4884c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4884c-121">Application</span></span> | <span data-ttu-id="4884c-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4884c-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4884c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4884c-123">HTTP request</span></span>
<span data-ttu-id="4884c-124"><!-- { "blockType": "ignored" } -->Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4884c-124"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="4884c-125">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4884c-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="4884c-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="4884c-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4884c-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4884c-128">Request headers</span></span>
| <span data-ttu-id="4884c-129">Имя</span><span class="sxs-lookup"><span data-stu-id="4884c-129">Name</span></span>       | <span data-ttu-id="4884c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4884c-130">Type</span></span> | <span data-ttu-id="4884c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4884c-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4884c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4884c-132">Authorization</span></span>  | <span data-ttu-id="4884c-133">string</span><span class="sxs-lookup"><span data-stu-id="4884c-133">string</span></span>  | <span data-ttu-id="4884c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4884c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4884c-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4884c-136">Content-Type</span></span> | <span data-ttu-id="4884c-137">string</span><span class="sxs-lookup"><span data-stu-id="4884c-137">string</span></span>  | <span data-ttu-id="4884c-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4884c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4884c-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4884c-140">Request body</span></span>
<span data-ttu-id="4884c-141">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4884c-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4884c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="4884c-142">Response</span></span>

<span data-ttu-id="4884c-143">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [вложения](../resources/attachment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4884c-143">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="4884c-144">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="4884c-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="4884c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4884c-145">Request</span></span>
<span data-ttu-id="4884c-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4884c-146">Here is an example of the request.</span></span>
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
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="4884c-147">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4884c-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4884c-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="4884c-148">Response</span></span>
<span data-ttu-id="4884c-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4884c-149">Here is an example of the response.</span></span> 
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
    "contentBytes": "R0lGODdhEAYEAA7"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="4884c-150">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="4884c-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="4884c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4884c-151">Request</span></span>
<span data-ttu-id="4884c-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4884c-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message"
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

##### <a name="response"></a><span data-ttu-id="4884c-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="4884c-153">Response</span></span>
<span data-ttu-id="4884c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4884c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="4884c-157">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="4884c-157">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="4884c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="4884c-158">Request</span></span>
<span data-ttu-id="4884c-159">Ниже приведен пример запроса, добавляет подключение к ссылку существующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="4884c-159">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="4884c-160">Вложение указывает на папку на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4884c-160">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4884c-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="4884c-161">Response</span></span>
<span data-ttu-id="4884c-162">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="4884c-162">Here is an example of a full response.</span></span>
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
    "Error: /api-reference/beta/api/message-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
