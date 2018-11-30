---
title: Добавление вложения
description: Используйте этот интерфейс API для добавления вложения в событии. Начиная с него
ms.openlocfilehash: 6a5d07c8cbbeab6895a38d915c2fcdfa9e2e5c50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076995"
---
# <a name="add-attachment"></a><span data-ttu-id="16c8e-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="16c8e-104">Add attachment</span></span>

> <span data-ttu-id="16c8e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16c8e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16c8e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16c8e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16c8e-p103">С помощью этого API можно добавить [вложение](../resources/attachment.md) к событию. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="16c8e-p103">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="16c8e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16c8e-109">Permissions</span></span>
<span data-ttu-id="16c8e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16c8e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16c8e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16c8e-112">Permission type</span></span>      | <span data-ttu-id="16c8e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16c8e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16c8e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16c8e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16c8e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16c8e-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="16c8e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16c8e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16c8e-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16c8e-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="16c8e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16c8e-118">Application</span></span> | <span data-ttu-id="16c8e-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16c8e-119">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="16c8e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16c8e-120">HTTP request</span></span>
<span data-ttu-id="16c8e-121">Вложения для [событий](../resources/event.md) в списке пользователя по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="16c8e-121">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="16c8e-122">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="16c8e-122">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="16c8e-123">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="16c8e-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="16c8e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16c8e-124">Request headers</span></span>
| <span data-ttu-id="16c8e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="16c8e-125">Name</span></span>       | <span data-ttu-id="16c8e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="16c8e-126">Type</span></span> | <span data-ttu-id="16c8e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="16c8e-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16c8e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="16c8e-128">Authorization</span></span>  | <span data-ttu-id="16c8e-129">string</span><span class="sxs-lookup"><span data-stu-id="16c8e-129">string</span></span>  | <span data-ttu-id="16c8e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16c8e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16c8e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16c8e-132">Content-Type</span></span> | <span data-ttu-id="16c8e-133">string</span><span class="sxs-lookup"><span data-stu-id="16c8e-133">string</span></span>  | <span data-ttu-id="16c8e-p106">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16c8e-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16c8e-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16c8e-136">Request body</span></span>
<span data-ttu-id="16c8e-137">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16c8e-137">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="16c8e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="16c8e-138">Response</span></span>

<span data-ttu-id="16c8e-139">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16c8e-139">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="16c8e-140">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="16c8e-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="16c8e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="16c8e-141">Request</span></span>
<span data-ttu-id="16c8e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16c8e-142">Here is an example of the request.</span></span>
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

<span data-ttu-id="16c8e-143">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16c8e-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="16c8e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="16c8e-144">Response</span></span>
<span data-ttu-id="16c8e-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16c8e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="16c8e-148">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="16c8e-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="16c8e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="16c8e-149">Request</span></span>

<span data-ttu-id="16c8e-150">В этом примере к одному событию прикрепляется другое в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="16c8e-150">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

##### <a name="response"></a><span data-ttu-id="16c8e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="16c8e-151">Response</span></span>
<span data-ttu-id="16c8e-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="16c8e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="16c8e-155">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="16c8e-155">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="16c8e-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="16c8e-156">Request</span></span>
<span data-ttu-id="16c8e-157">Ниже приведен пример запроса, добавляет подключение к ссылку на существующий событие.</span><span class="sxs-lookup"><span data-stu-id="16c8e-157">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="16c8e-158">Вложение указывает на папку на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="16c8e-158">The attachment points to a folder on OneDrive.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_event",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
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

##### <a name="response"></a><span data-ttu-id="16c8e-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="16c8e-159">Response</span></span>
<span data-ttu-id="16c8e-160">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="16c8e-160">Here is an example of a full response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
