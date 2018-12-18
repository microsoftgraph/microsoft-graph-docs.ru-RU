---
title: Добавление вложения
description: 'С помощью этого API можно добавить вложение к сообщению. '
author: angelgolfer-ms
ms.openlocfilehash: 6f6a25f940429637e4b04f200e9a0fcee067c011
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318909"
---
# <a name="add-attachment"></a><span data-ttu-id="218b7-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="218b7-103">Add attachment</span></span>

> <span data-ttu-id="218b7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="218b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="218b7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="218b7-106">С помощью этого API можно добавить [вложение](../resources/attachment.md) к сообщению.</span><span class="sxs-lookup"><span data-stu-id="218b7-106">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="218b7-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="218b7-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="218b7-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="218b7-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="218b7-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="218b7-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="218b7-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="218b7-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="218b7-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="218b7-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="218b7-112">Можно добавить вложения в существующее сообщение, отправку сообщений в коллекцию вложения или в новое сообщение, который [черновик](../api/user-post-messages.md)или [создан и отправлен во время выполнения](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="218b7-112">You can add an attachment to an existing message by posting to its attachments collection, or to a new message that is being [drafted](../api/user-post-messages.md), or [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="218b7-113">Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="218b7-113">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="218b7-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="218b7-114">Permissions</span></span>
<span data-ttu-id="218b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="218b7-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="218b7-117">Permission type</span></span>      | <span data-ttu-id="218b7-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="218b7-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="218b7-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="218b7-119">Delegated (work or school account)</span></span> | <span data-ttu-id="218b7-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="218b7-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="218b7-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="218b7-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="218b7-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="218b7-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="218b7-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="218b7-123">Application</span></span> | <span data-ttu-id="218b7-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="218b7-124">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="218b7-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="218b7-125">HTTP request</span></span>
<span data-ttu-id="218b7-126"><!-- { "blockType": "ignored" } -->Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="218b7-126"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="218b7-127">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="218b7-127">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="218b7-p103">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="218b7-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="218b7-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="218b7-130">Request headers</span></span>
| <span data-ttu-id="218b7-131">Имя</span><span class="sxs-lookup"><span data-stu-id="218b7-131">Name</span></span>       | <span data-ttu-id="218b7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="218b7-132">Type</span></span> | <span data-ttu-id="218b7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="218b7-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="218b7-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="218b7-134">Authorization</span></span>  | <span data-ttu-id="218b7-135">string</span><span class="sxs-lookup"><span data-stu-id="218b7-135">string</span></span>  | <span data-ttu-id="218b7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218b7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="218b7-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="218b7-138">Content-Type</span></span> | <span data-ttu-id="218b7-139">string</span><span class="sxs-lookup"><span data-stu-id="218b7-139">string</span></span>  | <span data-ttu-id="218b7-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218b7-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="218b7-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="218b7-142">Request body</span></span>
<span data-ttu-id="218b7-143">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="218b7-143">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="218b7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="218b7-144">Response</span></span>

<span data-ttu-id="218b7-145">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [вложения](../resources/attachment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="218b7-145">If successful, this method returns `201 Created` response code and the [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="218b7-146">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="218b7-146">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="218b7-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="218b7-147">Request</span></span>
<span data-ttu-id="218b7-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="218b7-148">Here is an example of the request.</span></span>
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

<span data-ttu-id="218b7-149">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="218b7-149">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="218b7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="218b7-150">Response</span></span>
<span data-ttu-id="218b7-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="218b7-151">Here is an example of the response.</span></span> 
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

## <a name="example-item-attachment"></a><span data-ttu-id="218b7-152">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="218b7-152">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="218b7-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="218b7-153">Request</span></span>
<span data-ttu-id="218b7-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="218b7-154">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="218b7-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="218b7-155">Response</span></span>
<span data-ttu-id="218b7-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="218b7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="218b7-159">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="218b7-159">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="218b7-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="218b7-160">Request</span></span>
<span data-ttu-id="218b7-161">Ниже приведен пример запроса, добавляет подключение к ссылку существующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="218b7-161">Here is an example of a request that adds a reference attachment to an existing message.</span></span>
<span data-ttu-id="218b7-162">Вложение указывает на папку на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="218b7-162">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="218b7-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="218b7-163">Response</span></span>
<span data-ttu-id="218b7-164">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="218b7-164">Here is an example of a full response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
