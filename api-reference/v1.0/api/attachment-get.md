---
title: Получение вложения
description: 'Чтение свойств и связей объекта, представляющего вложение, которое было добавлено к данным о событии '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 09fac27ef28fe30a69c03a7bfb18e8c3d95575f8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264808"
---
# <a name="get-attachment"></a><span data-ttu-id="371f4-103">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="371f4-103">Get attachment</span></span>

<span data-ttu-id="371f4-104">Чтение свойств и связей объекта, представляющего вложение, которое было добавлено к [данным о событии](../resources/event.md), [сообщению](../resources/message.md) или [записи](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="371f4-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="371f4-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="371f4-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="371f4-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="371f4-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="371f4-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="371f4-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="371f4-108">Вы можете использовать `$expand` для получения других свойств этого элемента.</span><span class="sxs-lookup"><span data-stu-id="371f4-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="371f4-109">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="371f4-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="371f4-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="371f4-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="371f4-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="371f4-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 


## <a name="permissions"></a><span data-ttu-id="371f4-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="371f4-112">Permissions</span></span>
<span data-ttu-id="371f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="371f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="371f4-115">При доступе к вложениям в сообщениях: Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="371f4-115">If accessing attachments in messages: Mail.Read.</span></span>
* <span data-ttu-id="371f4-116">При доступе к вложениям в событиях: Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="371f4-116">If accessing attachments in events: Calendars.Read.</span></span>
* <span data-ttu-id="371f4-117">При доступе к вложениям в событиях или записях групп: Group.Read.All.</span><span class="sxs-lookup"><span data-stu-id="371f4-117">If accessing attachments in group posts: Group.Read.All.</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="371f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="371f4-118">HTTP request</span></span>
<span data-ttu-id="371f4-119">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f4-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}

GET /me/calendar/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="371f4-120">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f4-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="371f4-121">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f4-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="371f4-122">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f4-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="371f4-123">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="371f4-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="371f4-p103">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д. </span><span class="sxs-lookup"><span data-stu-id="371f4-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="371f4-126">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="371f4-126">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="371f4-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="371f4-127">Optional query parameters</span></span>
<span data-ttu-id="371f4-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="371f4-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="371f4-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="371f4-129">Request headers</span></span>
| <span data-ttu-id="371f4-130">Имя</span><span class="sxs-lookup"><span data-stu-id="371f4-130">Name</span></span>       | <span data-ttu-id="371f4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="371f4-131">Type</span></span> | <span data-ttu-id="371f4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="371f4-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="371f4-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="371f4-133">Authorization</span></span>  | <span data-ttu-id="371f4-134">string</span><span class="sxs-lookup"><span data-stu-id="371f4-134">string</span></span>  | <span data-ttu-id="371f4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="371f4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="371f4-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="371f4-137">Request body</span></span>
<span data-ttu-id="371f4-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="371f4-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="371f4-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="371f4-139">Response</span></span>

<span data-ttu-id="371f4-140">В случае успеха этот метод возвращает код ответа `200 OK` и объект **attachment** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="371f4-140">If successful, this method returns a `200 OK` response code and an **attachment** object in the response body.</span></span> <span data-ttu-id="371f4-141">Кроме того, возвращаются свойства этого типа вложения: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="371f4-141">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="371f4-142">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="371f4-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="371f4-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="371f4-143">Request</span></span>
<span data-ttu-id="371f4-144">Ниже приведен пример запроса на получение вложенного файла из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="371f4-144">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a><span data-ttu-id="371f4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="371f4-145">Response</span></span>
<span data-ttu-id="371f4-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="371f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "contentType": "contentType-value",
  "contentLocation": "contentLocation-value",
  "contentBytes": "binary",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="371f4-149">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="371f4-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="371f4-150">C#</span><span class="sxs-lookup"><span data-stu-id="371f4-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_file_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="371f4-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="371f4-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_file_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="371f4-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="371f4-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_file_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
## <a name="example-item-attachment"></a><span data-ttu-id="371f4-153">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="371f4-153">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="371f4-154">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="371f4-154">Request 1</span></span>
<span data-ttu-id="371f4-155">В первом примере показано, как получить вложенный элемент в сообщении.</span><span class="sxs-lookup"><span data-stu-id="371f4-155">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="371f4-156">Возвращаются свойства **itemAttachment**.</span><span class="sxs-lookup"><span data-stu-id="371f4-156">The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```

##### <a name="response-1"></a><span data-ttu-id="371f4-157">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="371f4-157">Response 1</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="371f4-158">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="371f4-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="371f4-159">C#</span><span class="sxs-lookup"><span data-stu-id="371f4-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_item_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="371f4-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="371f4-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_item_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="371f4-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="371f4-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_item_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="371f4-162">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="371f4-162">Request 2</span></span>
<span data-ttu-id="371f4-163">В следующем примере показано, как использовать `$expand` для получения свойств элемента, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="371f4-163">The next example shows how to use `$expand` to get the properties of the item that is attached to the message.</span></span> <span data-ttu-id="371f4-164">В этом примере вложением является сообщением. Свойства вложенного сообщения также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="371f4-164">In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```

##### <a name="response-2"></a><span data-ttu-id="371f4-165">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="371f4-165">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="371f4-166">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="371f4-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="371f4-167">C#</span><span class="sxs-lookup"><span data-stu-id="371f4-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_and_expand_item_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="371f4-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="371f4-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_and_expand_item_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="371f4-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="371f4-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_and_expand_item_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



## <a name="example-reference-attachment"></a><span data-ttu-id="371f4-170">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="371f4-170">Example (reference attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="371f4-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="371f4-171">Request</span></span>
<span data-ttu-id="371f4-172">Ниже приведен пример запроса на получение вложенной ссылки из сообщения.</span><span class="sxs-lookup"><span data-stu-id="371f4-172">Here is an example of the request to get a reference attachment on a message.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
##### <a name="response"></a><span data-ttu-id="371f4-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="371f4-173">Response</span></span>
<span data-ttu-id="371f4-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="371f4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKgAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=",
    "lastModifiedDateTime": "2019-04-02T02:58:11Z",
    "name": "Sales Invoice Template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 1060,
    "isInline": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="371f4-177">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="371f4-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="371f4-178">C#</span><span class="sxs-lookup"><span data-stu-id="371f4-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_reference_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="371f4-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="371f4-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_reference_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="371f4-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="371f4-180">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_reference_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
