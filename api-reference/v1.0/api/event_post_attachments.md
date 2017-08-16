# <a name="add-attachment"></a><span data-ttu-id="a2055-101">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="a2055-101">Add attachment</span></span>

<span data-ttu-id="a2055-p101">С помощью этого API можно добавить [вложение](../resources/attachment.md) к событию. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="a2055-p101">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2055-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a2055-104">Prerequisites</span></span>
<span data-ttu-id="a2055-105">Для применения этого API требуется одна из указанных **областей**: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="a2055-105">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="a2055-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2055-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a2055-107">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="a2055-107">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
POST /groups/{id}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
```
<span data-ttu-id="a2055-108">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2055-108">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="a2055-109">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2055-109">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="a2055-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2055-110">Request headers</span></span>
| <span data-ttu-id="a2055-111">Имя</span><span class="sxs-lookup"><span data-stu-id="a2055-111">Name</span></span>       | <span data-ttu-id="a2055-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a2055-112">Type</span></span> | <span data-ttu-id="a2055-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a2055-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2055-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2055-114">Authorization</span></span>  | <span data-ttu-id="a2055-115">string</span><span class="sxs-lookup"><span data-stu-id="a2055-115">string</span></span>  | <span data-ttu-id="a2055-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2055-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2055-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2055-118">Content-Type</span></span> | <span data-ttu-id="a2055-119">string</span><span class="sxs-lookup"><span data-stu-id="a2055-119">string</span></span>  | <span data-ttu-id="a2055-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2055-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2055-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2055-122">Request body</span></span>
<span data-ttu-id="a2055-123">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2055-123">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a2055-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2055-124">Response</span></span>

<span data-ttu-id="a2055-125">В случае успеха этот метод возвращает код отклика `201, Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2055-125">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a2055-126">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="a2055-126">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a2055-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2055-127">Request</span></span>
<span data-ttu-id="a2055-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2055-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments 
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```

<span data-ttu-id="a2055-129">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2055-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a2055-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2055-130">Response</span></span>
<span data-ttu-id="a2055-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2055-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-Length: 735

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

## <a name="example-item-attachment"></a><span data-ttu-id="a2055-132">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="a2055-132">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a2055-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2055-133">Request</span></span>

<span data-ttu-id="a2055-134">В этом примере к одному событию прикрепляется другое в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="a2055-134">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
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

##### <a name="response"></a><span data-ttu-id="a2055-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2055-135">Response</span></span>
<span data-ttu-id="a2055-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a2055-136">Here is an example of the response.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/api/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/api/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
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
  "tocPath": ""
}-->
