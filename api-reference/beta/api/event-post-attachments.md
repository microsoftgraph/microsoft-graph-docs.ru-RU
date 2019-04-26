---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к событию. Так как
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 583959b227afccaf52b5951aa4270523bccd1dc1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324340"
---
# <a name="add-attachment"></a><span data-ttu-id="1b874-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="1b874-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b874-p102">С помощью этого API можно добавить [вложение](../resources/attachment.md) к событию. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="1b874-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b874-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b874-107">Permissions</span></span>

<span data-ttu-id="1b874-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b874-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b874-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b874-110">Permission type</span></span>      | <span data-ttu-id="1b874-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b874-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b874-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b874-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b874-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b874-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1b874-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b874-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b874-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b874-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1b874-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b874-116">Application</span></span> | <span data-ttu-id="1b874-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b874-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b874-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b874-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="1b874-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b874-119">Request headers</span></span>

| <span data-ttu-id="1b874-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1b874-120">Name</span></span>       | <span data-ttu-id="1b874-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1b874-121">Type</span></span> | <span data-ttu-id="1b874-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1b874-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1b874-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b874-123">Authorization</span></span>  | <span data-ttu-id="1b874-124">string</span><span class="sxs-lookup"><span data-stu-id="1b874-124">string</span></span>  | <span data-ttu-id="1b874-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b874-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b874-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b874-127">Content-Type</span></span> | <span data-ttu-id="1b874-128">string</span><span class="sxs-lookup"><span data-stu-id="1b874-128">string</span></span>  | <span data-ttu-id="1b874-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b874-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b874-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b874-131">Request body</span></span>

<span data-ttu-id="1b874-132">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b874-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b874-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b874-133">Response</span></span>

<span data-ttu-id="1b874-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b874-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="1b874-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="1b874-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="1b874-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b874-136">Request</span></span>

<span data-ttu-id="1b874-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b874-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
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

<span data-ttu-id="1b874-138">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b874-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="1b874-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b874-139">Response</span></span>

<span data-ttu-id="1b874-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b874-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
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

## <a name="example-item-attachment"></a><span data-ttu-id="1b874-143">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="1b874-143">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="1b874-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b874-144">Request</span></span>

<span data-ttu-id="1b874-145">Ниже приведен пример, в котором присоединяется событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="1b874-145">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

### <a name="response"></a><span data-ttu-id="1b874-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b874-146">Response</span></span>

<span data-ttu-id="1b874-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b874-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
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

## <a name="example-reference-attachment"></a><span data-ttu-id="1b874-150">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="1b874-150">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="1b874-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b874-151">Request</span></span>

<span data-ttu-id="1b874-152">Ниже приведен пример запроса, добавляющего к существующему событию вложенное ссылку.</span><span class="sxs-lookup"><span data-stu-id="1b874-152">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="1b874-153">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1b874-153">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event",
  "@odata.type": "microsoft.graph.referenceAttachment"
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

### <a name="response"></a><span data-ttu-id="1b874-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b874-154">Response</span></span>

<span data-ttu-id="1b874-155">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="1b874-155">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
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
  "tocPath": "",
  "suppressions": [
    "Error: create_file_attachment_from_event/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk='"
  ]
}
-->
