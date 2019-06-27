---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к событию. Так как
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8067b289fec2de2c07c70d1b1cfafcc2b5be6835
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259194"
---
# <a name="add-attachment"></a><span data-ttu-id="50c12-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="50c12-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50c12-p102">С помощью этого API можно добавить [вложение](../resources/attachment.md) к событию. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="50c12-p102">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="50c12-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50c12-107">Permissions</span></span>

<span data-ttu-id="50c12-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50c12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50c12-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50c12-110">Permission type</span></span>      | <span data-ttu-id="50c12-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50c12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50c12-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50c12-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50c12-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50c12-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="50c12-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50c12-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50c12-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50c12-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="50c12-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50c12-116">Application</span></span> | <span data-ttu-id="50c12-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50c12-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50c12-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50c12-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
```

<!--
POST /groups/{id}/events/{id}/attachments
-->

## <a name="request-headers"></a><span data-ttu-id="50c12-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50c12-119">Request headers</span></span>

| <span data-ttu-id="50c12-120">Имя</span><span class="sxs-lookup"><span data-stu-id="50c12-120">Name</span></span>       | <span data-ttu-id="50c12-121">Тип</span><span class="sxs-lookup"><span data-stu-id="50c12-121">Type</span></span> | <span data-ttu-id="50c12-122">Описание</span><span class="sxs-lookup"><span data-stu-id="50c12-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50c12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50c12-123">Authorization</span></span>  | <span data-ttu-id="50c12-124">string</span><span class="sxs-lookup"><span data-stu-id="50c12-124">string</span></span>  | <span data-ttu-id="50c12-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50c12-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50c12-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50c12-127">Content-Type</span></span> | <span data-ttu-id="50c12-128">string</span><span class="sxs-lookup"><span data-stu-id="50c12-128">string</span></span>  | <span data-ttu-id="50c12-p105">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50c12-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50c12-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50c12-131">Request body</span></span>

<span data-ttu-id="50c12-132">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50c12-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="50c12-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="50c12-133">Response</span></span>

<span data-ttu-id="50c12-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50c12-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="50c12-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="50c12-135">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="50c12-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="50c12-136">Request</span></span>

<span data-ttu-id="50c12-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50c12-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="50c12-138">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50c12-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="50c12-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="50c12-139">Response</span></span>

<span data-ttu-id="50c12-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50c12-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="50c12-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="50c12-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50c12-144">C#</span><span class="sxs-lookup"><span data-stu-id="50c12-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50c12-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="50c12-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_event-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="50c12-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="50c12-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_event-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="50c12-147">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="50c12-147">Example (item attachment)</span></span>

### <a name="request"></a><span data-ttu-id="50c12-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="50c12-148">Request</span></span>

<span data-ttu-id="50c12-149">Ниже приведен пример, в котором присоединяется событие с другим событием в качестве вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="50c12-149">Here is an example which attaches an event with another event as an item attachment.</span></span>

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

### <a name="response"></a><span data-ttu-id="50c12-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="50c12-150">Response</span></span>

<span data-ttu-id="50c12-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50c12-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="50c12-154">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="50c12-154">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="50c12-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="50c12-155">Request</span></span>

<span data-ttu-id="50c12-156">Ниже приведен пример запроса, добавляющего к существующему событию вложенное ссылку.</span><span class="sxs-lookup"><span data-stu-id="50c12-156">Here is an example of a request that adds a reference attachment to an existing event.</span></span>
<span data-ttu-id="50c12-157">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="50c12-157">The attachment points to a folder on OneDrive.</span></span>
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

### <a name="response"></a><span data-ttu-id="50c12-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="50c12-158">Response</span></span>

<span data-ttu-id="50c12-159">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="50c12-159">Here is an example of a full response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="50c12-160">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="50c12-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50c12-161">C#</span><span class="sxs-lookup"><span data-stu-id="50c12-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50c12-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="50c12-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_event-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="50c12-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="50c12-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_event-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: create_file_attachment_from_event/contentBytes:\r\n      Expected type Binary but actual was String. Property: contentBytes, actual value: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk='"
  ]
}
-->
