# <a name="add-attachment"></a><span data-ttu-id="00280-101">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="00280-101">Add attachment</span></span>

<span data-ttu-id="00280-p101">С помощью этого API можно добавить [вложение](../resources/attachment.md) к событию. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="00280-p101">Use this API to add an [attachment](../resources/attachment.md) to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="00280-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00280-104">Permissions</span></span>
<span data-ttu-id="00280-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00280-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00280-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00280-107">Permission type</span></span>      | <span data-ttu-id="00280-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00280-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00280-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00280-109">Delegated (work or school account)</span></span> | <span data-ttu-id="00280-110">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00280-110">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="00280-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00280-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00280-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00280-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="00280-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00280-113">Application</span></span> | <span data-ttu-id="00280-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00280-114">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00280-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00280-115">HTTP request</span></span>
<span data-ttu-id="00280-116">Вложения в событие ([event](../resources/event.md)) в пользовательском календаре ([calendar](../resources/calendar.md)), установленном по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="00280-116">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="00280-117">Вложения в событие ([event](../resources/event.md)) в календаре ([calendar](../resources/calendar.md)), который принадлежит установленной по умолчанию группе календарей ([calendarGroup](../resources/calendargroup.md)) пользователя.</span><span class="sxs-lookup"><span data-stu-id="00280-117">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
<span data-ttu-id="00280-118">Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="00280-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="00280-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00280-119">Request headers</span></span>
| <span data-ttu-id="00280-120">Имя</span><span class="sxs-lookup"><span data-stu-id="00280-120">Name</span></span>       | <span data-ttu-id="00280-121">Тип</span><span class="sxs-lookup"><span data-stu-id="00280-121">Type</span></span> | <span data-ttu-id="00280-122">Описание</span><span class="sxs-lookup"><span data-stu-id="00280-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="00280-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00280-123">Authorization</span></span>  | <span data-ttu-id="00280-124">строка</span><span class="sxs-lookup"><span data-stu-id="00280-124">string</span></span>  | <span data-ttu-id="00280-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00280-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00280-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00280-127">Content-Type</span></span> | <span data-ttu-id="00280-128">string</span><span class="sxs-lookup"><span data-stu-id="00280-128">string</span></span>  | <span data-ttu-id="00280-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00280-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00280-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00280-131">Request body</span></span>
<span data-ttu-id="00280-132">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00280-132">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00280-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="00280-133">Response</span></span>

<span data-ttu-id="00280-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00280-134">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="00280-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="00280-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="00280-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="00280-136">Request</span></span>
<span data-ttu-id="00280-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00280-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
  "name": "create_file_attachment_from_event"
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

<span data-ttu-id="00280-138">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00280-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="00280-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="00280-139">Response</span></span>
<span data-ttu-id="00280-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00280-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
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
    "contentBytes":"base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="00280-141">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="00280-141">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="00280-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="00280-142">Request</span></span>

<span data-ttu-id="00280-143">В этом примере к одному событию прикрепляется другое в качестве вложения.</span><span class="sxs-lookup"><span data-stu-id="00280-143">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAt9AHjAAA="],
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

##### <a name="response"></a><span data-ttu-id="00280-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="00280-144">Response</span></span>
<span data-ttu-id="00280-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00280-145">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
