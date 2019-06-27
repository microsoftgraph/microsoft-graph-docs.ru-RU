---
title: Добавление вложения
description: 'С помощью этого API можно добавить вложение к сообщению. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1b68777b98a3f956b0032318070531db2bf9c627
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276792"
---
# <a name="add-attachment"></a><span data-ttu-id="14dd8-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="14dd8-103">Add attachment</span></span>

<span data-ttu-id="14dd8-104">С помощью этого API можно добавить [вложение](../resources/attachment.md) к сообщению.</span><span class="sxs-lookup"><span data-stu-id="14dd8-104">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="14dd8-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="14dd8-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="14dd8-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="14dd8-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="14dd8-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="14dd8-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="14dd8-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="14dd8-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="14dd8-109">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="14dd8-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="14dd8-110">Вы можете добавить вложение к существующему сообщению, добавив его в коллекцию вложений, или к сообщению, [создаваемому и отправляемому на ходу](../api/user-sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="14dd8-110">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user-sendmail.md).</span></span>

<span data-ttu-id="14dd8-111">Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="14dd8-111">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="14dd8-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14dd8-112">Permissions</span></span>
<span data-ttu-id="14dd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14dd8-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14dd8-115">Permission type</span></span>      | <span data-ttu-id="14dd8-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14dd8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14dd8-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14dd8-117">Delegated (work or school account)</span></span> | <span data-ttu-id="14dd8-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14dd8-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="14dd8-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14dd8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14dd8-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14dd8-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="14dd8-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14dd8-121">Application</span></span> | <span data-ttu-id="14dd8-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14dd8-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="14dd8-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14dd8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="14dd8-124">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="14dd8-124">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="14dd8-125">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="14dd8-125">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="14dd8-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="14dd8-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="14dd8-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14dd8-128">Request headers</span></span>
| <span data-ttu-id="14dd8-129">Имя</span><span class="sxs-lookup"><span data-stu-id="14dd8-129">Name</span></span>       | <span data-ttu-id="14dd8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14dd8-130">Type</span></span> | <span data-ttu-id="14dd8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14dd8-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14dd8-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="14dd8-132">Authorization</span></span>  | <span data-ttu-id="14dd8-133">string</span><span class="sxs-lookup"><span data-stu-id="14dd8-133">string</span></span>  | <span data-ttu-id="14dd8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14dd8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14dd8-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14dd8-136">Content-Type</span></span> | <span data-ttu-id="14dd8-137">string</span><span class="sxs-lookup"><span data-stu-id="14dd8-137">string</span></span>  | <span data-ttu-id="14dd8-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14dd8-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14dd8-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14dd8-140">Request body</span></span>
<span data-ttu-id="14dd8-141">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14dd8-141">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="14dd8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="14dd8-142">Response</span></span>

<span data-ttu-id="14dd8-143">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14dd8-143">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="14dd8-144">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="14dd8-144">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="14dd8-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="14dd8-145">Request</span></span>
<span data-ttu-id="14dd8-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14dd8-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "base64R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="14dd8-147">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14dd8-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="14dd8-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="14dd8-148">Response</span></span>
<span data-ttu-id="14dd8-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14dd8-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
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
    "contentBytes": "base64R0lGODdhEAYEAA7"
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="14dd8-150">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="14dd8-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="14dd8-151">C#</span><span class="sxs-lookup"><span data-stu-id="14dd8-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14dd8-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="14dd8-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="14dd8-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="14dd8-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_message-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="14dd8-154">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="14dd8-154">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="14dd8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="14dd8-155">Request</span></span>
<span data-ttu-id="14dd8-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14dd8-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkpsDRVK"],
  "name": "create_item_attachment_from_message"
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

##### <a name="response"></a><span data-ttu-id="14dd8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="14dd8-157">Response</span></span>
<span data-ttu-id="14dd8-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14dd8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/message-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
