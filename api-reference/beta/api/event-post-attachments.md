---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к событию. Так как
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e1fb6c9bf074228c7cb30de2fa1f5ecd611f7f86
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43365063"
---
# <a name="add-attachment"></a><span data-ttu-id="c7ce1-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="c7ce1-104">Add attachment</span></span>

<span data-ttu-id="c7ce1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7ce1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7ce1-106">Используйте этот API, чтобы добавить [вложение](../resources/attachment.md) к существующему [событию](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c7ce1-106">Use this API to add an [attachment](../resources/attachment.md) to an existing [event](../resources/event.md).</span></span> <span data-ttu-id="c7ce1-107">Эта операция ограничит размер вложения, которое можно добавить в раздел 3 МБ.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-107">This operation limits the size of the attachment you can add to under 3 MB.</span></span>

<span data-ttu-id="c7ce1-108">Если организатор добавляет вложение в событие собрания, организатор может впоследствии [Обновить](event-update.md) событие, чтобы отправить вложение и обновить событие для каждого участника.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-108">If an organizer adds an attachment to a meeting event, the organizer can subsequently [update](event-update.md) the event to send the attachment and update the event for each attendee as well.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7ce1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ce1-109">Permissions</span></span>

<span data-ttu-id="c7ce1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7ce1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ce1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ce1-112">Permission type</span></span>      | <span data-ttu-id="c7ce1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7ce1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7ce1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7ce1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c7ce1-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ce1-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7ce1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7ce1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7ce1-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ce1-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c7ce1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7ce1-118">Application</span></span> | <span data-ttu-id="c7ce1-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ce1-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7ce1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7ce1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="c7ce1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7ce1-121">Request headers</span></span>

| <span data-ttu-id="c7ce1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c7ce1-122">Name</span></span>       | <span data-ttu-id="c7ce1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ce1-123">Type</span></span> | <span data-ttu-id="c7ce1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ce1-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7ce1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7ce1-125">Authorization</span></span>  | <span data-ttu-id="c7ce1-126">string</span><span class="sxs-lookup"><span data-stu-id="c7ce1-126">string</span></span>  | <span data-ttu-id="c7ce1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7ce1-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7ce1-129">Content-Type</span></span> | <span data-ttu-id="c7ce1-130">string</span><span class="sxs-lookup"><span data-stu-id="c7ce1-130">string</span></span>  | <span data-ttu-id="c7ce1-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7ce1-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7ce1-133">Request body</span></span>

<span data-ttu-id="c7ce1-134">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c7ce1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ce1-135">Response</span></span>

<span data-ttu-id="c7ce1-136">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-136">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="c7ce1-137">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="c7ce1-137">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="c7ce1-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ce1-138">Request</span></span>

<span data-ttu-id="c7ce1-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7ce1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7ce1-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```
# <a name="c"></a>[<span data-ttu-id="c7ce1-141">C#</span><span class="sxs-lookup"><span data-stu-id="c7ce1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-event-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7ce1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7ce1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-event-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7ce1-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7ce1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-event-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c7ce1-144">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-144">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="c7ce1-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ce1-145">Response</span></span>

<span data-ttu-id="c7ce1-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_file_attachment_from_event_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
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

## <a name="example-item-attachment"></a><span data-ttu-id="c7ce1-149">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="c7ce1-149">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="c7ce1-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ce1-150">Request</span></span>

<span data-ttu-id="c7ce1-151">Ниже приведен пример, в котором присоединяется событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-151">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
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


### <a name="response"></a><span data-ttu-id="c7ce1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ce1-152">Response</span></span>

<span data-ttu-id="c7ce1-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_item_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/beta/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="c7ce1-156">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="c7ce1-156">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="c7ce1-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ce1-157">Request</span></span>

<span data-ttu-id="c7ce1-158">Ниже приведен пример запроса, добавляющего к существующему событию вложенное ссылку.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-158">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="c7ce1-159">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-159">The attachment points to a folder on OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7ce1-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7ce1-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments
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
# <a name="c"></a>[<span data-ttu-id="c7ce1-161">C#</span><span class="sxs-lookup"><span data-stu-id="c7ce1-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7ce1-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7ce1-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7ce1-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7ce1-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7ce1-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ce1-164">Response</span></span>

<span data-ttu-id="c7ce1-165">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="c7ce1-165">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_reference_attachment_from_event",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
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
