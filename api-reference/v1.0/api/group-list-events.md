---
title: Список событий
description: Получение списка, включающего объекты событий.
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a00227170c5d16a639553049c0b85af060fd51ef
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682567"
---
# <a name="list-events"></a><span data-ttu-id="88695-103">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="88695-103">List events</span></span>

<span data-ttu-id="88695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88695-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88695-105">Получение списка объектов [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="88695-105">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="88695-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88695-106">Permissions</span></span>
<span data-ttu-id="88695-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88695-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88695-109">Permission type</span></span>      | <span data-ttu-id="88695-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88695-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88695-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88695-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88695-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88695-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="88695-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88695-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88695-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88695-114">Not supported.</span></span>    |
|<span data-ttu-id="88695-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88695-115">Application</span></span> | <span data-ttu-id="88695-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88695-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88695-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88695-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88695-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88695-118">Optional query parameters</span></span>
<span data-ttu-id="88695-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="88695-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88695-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88695-120">Request headers</span></span>
| <span data-ttu-id="88695-121">Имя</span><span class="sxs-lookup"><span data-stu-id="88695-121">Name</span></span>       | <span data-ttu-id="88695-122">Тип</span><span class="sxs-lookup"><span data-stu-id="88695-122">Type</span></span> | <span data-ttu-id="88695-123">Описание</span><span class="sxs-lookup"><span data-stu-id="88695-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="88695-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88695-124">Authorization</span></span>  | <span data-ttu-id="88695-125">string</span><span class="sxs-lookup"><span data-stu-id="88695-125">string</span></span> | <span data-ttu-id="88695-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88695-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="88695-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="88695-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="88695-129">string</span><span class="sxs-lookup"><span data-stu-id="88695-129">string</span></span> | <span data-ttu-id="88695-p103">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в отклике. Если он не задан, эти значения времени возвращаются в формате UTC. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="88695-p103">Use this to specify the time zone for start and end times in the response. If not specified, those time values are returned in UTC. Optional.</span></span> |
| <span data-ttu-id="88695-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="88695-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="88695-134">string</span><span class="sxs-lookup"><span data-stu-id="88695-134">string</span></span> | <span data-ttu-id="88695-135">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="88695-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="88695-136">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="88695-136">Values can be "text" or "html".</span></span> <span data-ttu-id="88695-137">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="88695-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="88695-138">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="88695-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="88695-139">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="88695-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88695-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88695-140">Request body</span></span>
<span data-ttu-id="88695-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88695-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88695-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="88695-142">Response</span></span>
<span data-ttu-id="88695-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="88695-143">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88695-144">Пример</span><span class="sxs-lookup"><span data-stu-id="88695-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="88695-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="88695-145">Request</span></span>
<span data-ttu-id="88695-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88695-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88695-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="88695-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```
# <a name="c"></a>[<span data-ttu-id="88695-148">C#</span><span class="sxs-lookup"><span data-stu-id="88695-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88695-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88695-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88695-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88695-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88695-151">Java</span><span class="sxs-lookup"><span data-stu-id="88695-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="88695-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="88695-152">Response</span></span>
<span data-ttu-id="88695-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="88695-153">The following is an example of the response.</span></span>
><span data-ttu-id="88695-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="88695-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
              "endDate": "0001-01-01",
              "recurrenceTimeZone": "Eastern Standard Time",
              "numberOfOccurrences": 0
          }
      },
      "attendees": [
          {
              "type": "required",
              "status": {
                  "response": "accepted",
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "HR Taskforce",
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Megan Bowen",
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
          }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

