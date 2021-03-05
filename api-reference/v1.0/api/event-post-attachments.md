---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к событию. Так как
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 14d62182f4d21618dae5d8009c4376404fff66eb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473828"
---
# <a name="add-attachment"></a><span data-ttu-id="8e98c-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="8e98c-104">Add attachment</span></span>

<span data-ttu-id="8e98c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e98c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e98c-106">Используйте этот API, чтобы добавить [вложение](../resources/attachment.md) к существующему [событию.](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="8e98c-106">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="8e98c-107">Эта операция ограничивает размер вложения, который можно добавить до 3 МБ.</span><span class="sxs-lookup"><span data-stu-id="8e98c-107">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="8e98c-108">Если организатор добавляет вложение в событие собрания, [](event-update.md) организатор может впоследствии обновить событие, чтобы отправить вложение и обновить событие для каждого участника.</span><span class="sxs-lookup"><span data-stu-id="8e98c-108">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e98c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e98c-109">Permissions</span></span>
<span data-ttu-id="8e98c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e98c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e98c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e98c-112">Permission type</span></span>      | <span data-ttu-id="8e98c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e98c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e98c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e98c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8e98c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e98c-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8e98c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e98c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e98c-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e98c-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8e98c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e98c-118">Application</span></span> | <span data-ttu-id="8e98c-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e98c-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e98c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e98c-120">HTTP request</span></span>
<span data-ttu-id="8e98c-121">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e98c-121">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
-->

<span data-ttu-id="8e98c-122">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e98c-122">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="8e98c-123">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e98c-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="8e98c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e98c-124">Request headers</span></span>
| <span data-ttu-id="8e98c-125">Имя</span><span class="sxs-lookup"><span data-stu-id="8e98c-125">Name</span></span>       | <span data-ttu-id="8e98c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="8e98c-126">Type</span></span> | <span data-ttu-id="8e98c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8e98c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e98c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e98c-128">Authorization</span></span>  | <span data-ttu-id="8e98c-129">string</span><span class="sxs-lookup"><span data-stu-id="8e98c-129">string</span></span>  | <span data-ttu-id="8e98c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e98c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e98c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e98c-132">Content-Type</span></span> | <span data-ttu-id="8e98c-133">string</span><span class="sxs-lookup"><span data-stu-id="8e98c-133">string</span></span>  | <span data-ttu-id="8e98c-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e98c-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e98c-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e98c-136">Request body</span></span>
<span data-ttu-id="8e98c-137">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e98c-137">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8e98c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e98c-138">Response</span></span>

<span data-ttu-id="8e98c-139">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e98c-139">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="8e98c-140">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="8e98c-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8e98c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e98c-141">Request</span></span>
<span data-ttu-id="8e98c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e98c-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e98c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e98c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_file_attachment_from_event_v1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```
# <a name="c"></a>[<span data-ttu-id="8e98c-144">C#</span><span class="sxs-lookup"><span data-stu-id="8e98c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e98c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e98c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e98c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e98c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e98c-147">Java</span><span class="sxs-lookup"><span data-stu-id="8e98c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-event-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8e98c-148">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e98c-148">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="8e98c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e98c-149">Response</span></span>
<span data-ttu-id="8e98c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e98c-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_event_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="8e98c-151">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="8e98c-151">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8e98c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e98c-152">Request</span></span>

<span data-ttu-id="8e98c-153">Вот пример, который прикрепит событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="8e98c-153">Here is an example which attaches an event with another event as an item attachment.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e98c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e98c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkAGI1AAAt9AHjAAA=/attachments
Content-type: application/json
Content-length: 600

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
# <a name="c"></a>[<span data-ttu-id="8e98c-155">C#</span><span class="sxs-lookup"><span data-stu-id="8e98c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e98c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e98c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e98c-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e98c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e98c-158">Java</span><span class="sxs-lookup"><span data-stu-id="8e98c-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="8e98c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e98c-159">Response</span></span>
<span data-ttu-id="8e98c-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e98c-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
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

