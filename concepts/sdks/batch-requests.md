---
title: Использование SDKs Graph Майкрософт для пакетных запросов
description: Содержит инструкции по созданию пакета запросов API с помощью SDKs Graph Microsoft.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: 222200851b3b6d5a1b85e49a1af741e5dbb1a809
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451957"
---
# <a name="use-the-microsoft-graph-sdks-to-batch-requests"></a>Использование SDKs Graph Майкрософт для пакетных запросов

[Пакетирование](../json-batching.md) — это способ объединения нескольких запросов в один http-запрос. Запросы объединяются в одну полезной нагрузки JSON, которая отправляется через POST в `\$batch` конечную точку. В Graph SDKs есть набор классов, упрощающий создание пакетных полезной нагрузки и разгрузку пакетных ответов.

> [!IMPORTANT]
> Текущие ограничения с пакетами JSON в Microsoft Graph см. в ссылке [Known Issues.](../known-issues.md#json-batching)

## <a name="create-a-batch-request"></a>Создание пакетного запроса

SDKs Graph Майкрософт предоставляют три класса для работы с пакетными запросами и ответами.

- **BatchRequestStep** — представляет один запрос `GET /me` (например) в пакете. Это позволяет назначить уникальный идентификатор запросу и указать зависимости между запросами.
- **BatchRequestContent** — упрощает создание полезной нагрузки пакетного запроса. Он содержит несколько **объектов BatchRequestStep.**
- **BatchResponseContent** — упрощает размыв ответа из пакетного запроса. Он обеспечивает возможность получения всех ответов, получения определенного ответа по ID и получения `@odata.nextLink` свойства, если оно присутствует.

## <a name="simple-batching-example"></a>Простой пример пакетной обработки

В этом примере показано, как отправлять несколько запросов в пакете, не зависящих друг от друга. Запросы могут быть запускаться службой в любом порядке. В этом примере пользователь получает представление календаря пользователя на текущий день.

### <a name="c"></a>[C#](#tab/csharp)

```csharp
// Use the request builder to generate a regular
// request to /me
var userRequest = graphClient.Me.Request();

var today = DateTime.Now.Date;
var start = today.ToString("yyyy-MM-ddTHH:mm:ssK");
var end = today.AddDays(1).ToString("yyyy-MM-ddTHH:mm:ssK");

var queryOptions = new List<QueryOption>
{
    new QueryOption("startDateTime", start),
    new QueryOption("endDateTime", end)
};

// Use the request builder to generate a regular
// request to /me/calendarview?startDateTime="start"&endDateTime="end"
var eventsRequest = graphClient.Me.CalendarView.Request(queryOptions);

// Build the batch
var batchRequestContent = new BatchRequestContent();

// Using AddBatchRequestStep adds each request as a step
// with no specified order of execution
var userRequestId = batchRequestContent.AddBatchRequestStep(userRequest);
var eventsRequestId = batchRequestContent.AddBatchRequestStep(eventsRequest);

var returnedResponse = await graphClient.Batch.Request().PostAsync(batchRequestContent);

// De-serialize response based on known return type
try
{
    var user = await returnedResponse
        .GetResponseByIdAsync<User>(userRequestId);
    Console.WriteLine($"Hello {user.DisplayName}!");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Get user failed: {ex.Error.Message}");
}

// For collections, must use the *CollectionResponse class to deserialize
// The .Value property will contain the *CollectionPage type that the Graph client
// returns from GetAsync().
try
{
    var events = await returnedResponse
        .GetResponseByIdAsync<UserCalendarViewCollectionResponse>(eventsRequestId);
    Console.WriteLine($"You have {events.Value.CurrentPage.Count} events on your calendar today.");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Get calendar view failed: {ex.Error.Message}");
}
```

### <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
// Create a batch request step to GET /me
let userRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "1",
  request: new Request("/me", {
    method: "GET"
  })
}

let today = moment({hour: 0, minute: 0, seconds: 0});
let start = today.format();
let end = today.add(1, "day").format();

// Create a batch request step to GET
// /me/calendarview?startDateTime="start"&endDateTime="end"
let calendarViewRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "2",
  request: new Request(`/me/calendarview?startDateTime=${start}&endDateTime=${end}`, {
    method: "GET"
  })
}

// Create the batch request content with the steps created
// above
let batchRequestContent = new MicrosoftGraph.BatchRequestContent([
  userRequestStep,
  calendarViewRequestStep
]);

let content = await batchRequestContent.getContent();

// POST the batch request content to the /$batch endpoint
let batchResponse = await client
  .api('/$batch')
  .post(content);

// Create a BatchResponseContent object to parse the response
let batchResponseContent = new MicrosoftGraph.BatchResponseContent(batchResponse);

// Get the user response using the id assigned to the request
let userResponse = batchResponseContent.getResponseById("1");

// For a single entity, the JSON payload can be deserialized
// into the expected type
// Types supplied by @microsoft/microsoft-graph-types
if (userResponse.ok) {
  let user: User = await userResponse.json();
  console.log(`Hello ${user.displayName}!`);
} else {
  console.log(`Get user failed with status ${userResponse.status}`);
}

// Get the calendar view response by id
let calendarResponse = batchResponseContent.getResponseById("2");

// For a collection of entities, the "value" property of
// the JSON payload can be deserialized into an array of
// the expected type
if (calendarResponse.ok) {
  let rawResponse = await calendarResponse.json();
  let events: [Event] = rawResponse.value;
  console.log(`You have ${events.length} events on your calendar today.`);
} else {
  console.log(`Get calendar view failed with status ${calendarResponse.status}`);
}
```

### <a name="java"></a>[Java](#tab/java)

```java
// Create the batch request content with the steps
final BatchRequestContent batchRequestContent = new BatchRequestContent();

// Use the Graph client to generate the request for GET /me
final String meGetId = batchRequestContent
                        .addBatchRequestStep(graphClient
                                              .me()
                                              .buildRequest());

final ZoneOffset localTimeZone = OffsetDateTime.now().getOffset();
final OffsetDateTime today = OffsetDateTime.of(LocalDate.now(), LocalTime.MIDNIGHT, localTimeZone);
final OffsetDateTime tomorrow = today.plusDays(1);

// Use the Graph client to generate the request URL for
// GET /me/calendarview?startDateTime="start"&endDateTime="end"
final List<Option> calendarViewOptions = Arrays.asList(new QueryOption("startDateTime", today.toString()),
                                                      new QueryOption("endDateTime", tomorrow.toString()));
final String calendarViewRequestStepId = batchRequestContent
                                        .addBatchRequestStep(graphClient
                                          .me()
                                          .calendarView()
                                          .buildRequest(calendarViewOptions));

// Send the batch request content to the /$batch endpoint
final BatchResponseContent batchResponseContent = graphClient.batch().buildRequest().post(batchRequestContent);
// Get the user response using the id assigned to the request
final User user = batchResponseContent.getResponseById(meGetId).getDeserializedBody(User.class);
System.out.println(String.format("Hello %s!", user.displayName));

// Get the calendar view response by id
final EventCollectionResponse events = batchResponseContent.getResponseById(calendarViewRequestStepId).getDeserializedBody(EventCollectionResponse.class);
System.out.println(String.format("You have %d events on your calendar today", events.value.size()));
```

---

## <a name="batches-with-dependent-requests"></a>Пакеты с зависимыми запросами

В этом примере показано, как отправлять несколько запросов в пакете, зависящих друг от друга. Запросы будут запускаться службой в порядке, указанном зависимостями. В этом примере событие со временем начала в течение текущего дня добавляется в календарь пользователя и получает представление календаря пользователя на текущий день. Чтобы убедиться, что возвращаемый обзор календаря включает созданное новое событие, запрос на просмотр календаря настроен в зависимости от запроса на добавление нового события. Это гарантирует, что сначала будет выполняться запрос на добавление события.

> [!NOTE]
> Если запрос добавить событие не удается, запрос на просмотр календаря будет сбой с `424 Failed Dependency` ошибкой.

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[C#](#tab/csharp)

```csharp
var today = DateTime.Now.Date;

var newEvent = new Event
{
    Subject = "File end-of-day report",
    Start = new DateTimeTimeZone
    {
        // 5:00 PM
        DateTime = today.AddHours(17).ToString("yyyy-MM-ddTHH:mm:ss"),
        TimeZone = TimeZoneInfo.Local.StandardName
    },
    End = new DateTimeTimeZone
    {
        // 5:30 PM
        DateTime = today.AddHours(17).AddMinutes(30).ToString("yyyy-MM-ddTHH:mm:ss"),
        TimeZone = TimeZoneInfo.Local.StandardName
    }
};

// POST requests are handled a bit differently
// The SDK request builders generate GET requests, so
// you must get the HttpRequestMessage and convert to a POST
var jsonEvent = graphClient.HttpProvider.Serializer.SerializeAsJsonContent(newEvent);

var addEventRequest = graphClient.Me.Events.Request().GetHttpRequestMessage();
addEventRequest.Method = HttpMethod.Post;
addEventRequest.Content = jsonEvent;

var start = today.ToString("yyyy-MM-ddTHH:mm:ssK");
var end = today.AddDays(1).ToString("yyyy-MM-ddTHH:mm:ssK");

var queryOptions = new List<QueryOption>
{
    new QueryOption("startDateTime", start),
    new QueryOption("endDateTime", end)
};

// Use the request builder to generate a regular
// request to /me/calendarview?startDateTime="start"&endDateTime="end"
var calendarViewRequest = graphClient.Me.CalendarView.Request(queryOptions);

// Build the batch
var batchRequestContent = new BatchRequestContent();

// Force the requests to execute in order, so that the request for
// today's events will include the new event created.

// First request, no dependency
var addEventRequestId = batchRequestContent.AddBatchRequestStep(addEventRequest);

// Second request, depends on addEventRequestId
var eventsRequestId = Guid.NewGuid().ToString();
batchRequestContent.AddBatchRequestStep(new BatchRequestStep(
    eventsRequestId,
    calendarViewRequest.GetHttpRequestMessage(),
    new List<string> { addEventRequestId }
));

var returnedResponse = await graphClient.Batch.Request().PostAsync(batchRequestContent);

// De-serialize response based on known return type
try
{
    var createdEvent = await returnedResponse
        .GetResponseByIdAsync<Event>(addEventRequestId);
    Console.WriteLine($"New event created with ID: {createdEvent.Id}");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Add event failed: {ex.Error.Message}");
}

// For collections, must use the *CollectionResponse class to deserialize
// The .Value property will contain the *CollectionPage type that the Graph client
// returns from GetAsync().
try
{
    var events = await returnedResponse
        .GetResponseByIdAsync<UserCalendarViewCollectionResponse>(eventsRequestId);
    Console.WriteLine($"You have {events.Value.CurrentPage.Count} events on your calendar today.");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Get calendar view failed: {ex.Error.Message}");
}
```

### <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
// 5:00 PM
let eventStart = moment({hour: 17, minute: 0, seconds: 0});

// Create a batch request step to add an event
let newEvent: Event = {
  subject: "File end-of-day report",
  start: {
    dateTime: eventStart
      .format("YYYY-MM-DDTHH:mm:ss"),
    timeZone: moment.tz.guess()
  },
  end: {
    // 5:30 PM
    dateTime: eventStart.add(30, "minutes")
      .format("YYYY-MM-DDTHH:mm:ss"),
    timeZone: moment.tz.guess()
  }
}
console.log(JSON.stringify(newEvent));

let addEventRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "1",
  request: new Request("/me/events", {
    method: "POST",
    body: JSON.stringify(newEvent),
    headers: {
      "Content-Type": "application/json"
    }
  })
}

let today = moment({hour: 0, minute: 0, seconds: 0});
let start = today.format();
let end = today.add(1, "day").format();
console.log(`/me/calendarview?startDateTime=${start}&endDateTime=${end}`);

// Create a batch request step to GET
// /me/calendarview?startDateTime="start"&endDateTime="end"
let calendarViewRequestStep: MicrosoftGraph.BatchRequestStep = {
  id: "2",
  // This step will happen after step 1
  dependsOn: [ "1" ],
  request: new Request(`/me/calendarview?startDateTime=${start}&endDateTime=${end}`, {
    method: "GET"
  })
}

// Create the batch request content with the steps created
// above
let batchRequestContent = new MicrosoftGraph.BatchRequestContent([
  addEventRequestStep,
  calendarViewRequestStep
]);

let content = await batchRequestContent.getContent();

// POST the batch request content to the /$batch endpoint
let batchResponse = await client
  .api('/$batch')
  .post(content);

// Create a BatchResponseContent object to parse the response
let batchResponseContent = new MicrosoftGraph.BatchResponseContent(batchResponse);

// Get the create event response by id
let newEventResponse = batchResponseContent.getResponseById("1");
if (newEventResponse.ok) {
  let event: Event = await newEventResponse.json();
  console.log(`New event created with ID: ${event.id}`);
} else {
  console.log(`Create event failed with status ${newEventResponse.status}`);
}

// Get the calendar view response by id
let calendarResponse = batchResponseContent.getResponseById("2");

if (calendarResponse.ok)
{
  // For a collection of entities, the "value" property of
  // the JSON payload can be deserialized into an array of
  // the expected type
  let rawResponse = await calendarResponse.json();
  let events: [Event] = rawResponse.value;
  console.log(`You have ${events.length} events on your calendar today.`);
} else {
  console.log(`Get calendar view failed with status ${calendarResponse.status}`);
}
```

### <a name="java"></a>[Java](#tab/java)

```java
// Create the batch request content with the steps
final BatchRequestContent batchRequestContent = new BatchRequestContent(batchSteps);

final ZoneOffset localTimeZone = OffsetDateTime.now().getOffset();
final OffsetDateTime today = OffsetDateTime.of(LocalDate.now(), LocalTime.MIDNIGHT, localTimeZone);
final OffsetDateTime tomorrow = today.plusDays(1);

// Use the Graph client to generate the request URL for POST /me/events
final Event newEvent = new Event();
newEvent.subject = "File end-of-day report";
newEvent.start = new DateTimeTimeZone();
// 5:00 PM
newEvent.start.dateTime = today.plusHours(17)
    .format(DateTimeFormatter.ISO_LOCAL_DATE_TIME);
newEvent.start.timeZone = ZoneOffset.systemDefault().getId();
newEvent.end = new DateTimeTimeZone();
// 5:30 PM
newEvent.end.dateTime = today.plusHours(17).plusMinutes(30)
    .format(DateTimeFormatter.ISO_LOCAL_DATE_TIME);
newEvent.end.timeZone = ZoneOffset.systemDefault().getId();

final String addEventRequestId = batchRequestContent
                                .addBatchRequestStep(graphClient
                                                .me()
                                                .events()
                                                .buildRequest(), HttpMethod.POST, newEvent);

// Use the Graph client to generate the request URL for
// GET /me/calendarview?startDateTime="start"&endDateTime="end"
final List<Option> calendarViewOptions = Arrays.asList(new QueryOption("startDateTime", today.toString()),
                                                      new QueryOption("endDateTime", tomorrow.toString()));
final String calendarViewRequestStepId = batchRequestContent
                                        .addBatchRequestStep(graphClient
                                          .me()
                                          .calendarView()
                                          .buildRequest(calendarViewOptions),
                                          HttpMethod.GET,
                                          null,
                                          addEventRequestId);

// Send the batch request content to the /$batch endpoint
final BatchResponseContent batchResponseContent = client.batch().buildRequest().post(batchRequestContent);
// Get the user response using the id assigned to the request
final Event event = batchResponseContent.getResponseById(addEventRequestId).getDeserializedBody(Event.class);
System.out.println(String.format("New event created with ID: %s", event.id));

// Get the calendar view response by id
final EventCollectionResponse events = batchResponseContent.getResponseById(calendarViewRequestStepId).getDeserializedBody(EventCollectionResponse.class);
System.out.println(String.format("You have %d events on your calendar today", events.value.size()));
```

---

## <a name="implementing-batching-using-batchrequestcontent-batchrequeststep-and-httprequestmessage"></a>Реализация пакета с помощью BatchRequestContent, BatchRequestStep и HttpRequestMessage

В следующем примере показано, как использовать , и отправлять несколько запросов в пакете и как обрабатывать ограничение в 20 с запросами API microsoft `BatchRequestContent` `BatchRequestStep` Graph `HttpRequestMessage` API. В этом примере создаются ссылки на собрания с использованием конечной `onlineMeetings/createOrGet` точки для указанного пользовательского ИД. Этот пример можно использовать и с Graph конечными точками Майкрософт.

```csharp
using System;
using System.Collections.Generic;
using System.Net.Http;
using System.Net.Http.Headers;
using System.Text;
using System.Threading.Tasks;
using Microsoft.Graph;
using Newtonsoft.Json;
using Newtonsoft.Json.Linq;

public async void GenerateBatchedMeetingLink(List<ItemCollections> meetingLinksToBeGenerated)
        {            
            List<string> _joinWebUrls = new List<string>();
            //Total number of items per batch supported is 20
            int maxNoBatchItems = 20;
            try
            {
                //valid GraphAccessToken is required to execute the call
                var graphClient = GetAuthenticatedClient(GraphAccessToken);
                var events = new List<OnlineMeetingCreateOrGetRequestBody>();
                foreach (var item in meetingLinksToBeGenerated)
                {
                    var externalId = Guid.NewGuid().ToString();
                    var @event = new OnlineMeetingCreateOrGetRequestBody
                    {
                        StartDateTime = item.StartTime,
                        EndDateTime = item.EndTime,
                        Subject = "Test Meeting",
                        ExternalId = externalId,
                        
                    };
                    events.Add(@event);
                }
                // if the requests are more than 20 limit, we need to create multiple batches of the BatchRequestContent
                List<BatchRequestContent> batches = new List<BatchRequestContent>();
                var batchRequestContent = new BatchRequestContent();
                foreach (OnlineMeetingCreateOrGetRequestBody e in events)
                { 
                    //create online meeting for particular user or we can use /me as well
                    var httpRequestMessage = new HttpRequestMessage(HttpMethod.Post, $"https://graph.microsoft.com/v1.0/users/{userID}/onlineMeetings/createOrGet")
                    {
                        Content = new StringContent(JsonConvert.SerializeObject(e), Encoding.UTF8, "application/json")
                    };
                    BatchRequestStep requestStep = new BatchRequestStep(events.IndexOf(e).ToString(), httpRequestMessage, null);
                    batchRequestContent.AddBatchRequestStep(requestStep);
                    if (events.IndexOf(e) > 0 && ((events.IndexOf(e) + 1) % maxNoBatchItems == 0))
                    {
                        batches.Add(batchRequestContent);
                        batchRequestContent = new BatchRequestContent();
                    }
                }
                if (batchRequestContent.BatchRequestSteps.Count < maxNoBatchItems)
                {
                    batches.Add(batchRequestContent);
                }

                if (batches.Count == 0 && batchRequestContent != null)
                {
                    batches.Add(batchRequestContent);
                }

                foreach (BatchRequestContent batch in batches)
                {
                    BatchResponseContent response = null;
                    response = await graphClient.Batch.Request().PostAsync(batch);
                    Dictionary<string, HttpResponseMessage> responses = await response.GetResponsesAsync();
                    foreach (string key in responses.Keys)
                    {
                        HttpResponseMessage httpResponse = await response.GetResponseByIdAsync(key);
                        var responseContent = await httpResponse.Content.ReadAsStringAsync();
                        JObject eventResponse = JObject.Parse(responseContent);
                        //do something below
                        Console.writeline(eventResponse["joinWebUrl"].ToString());                      
                    }                 
                }
            }
            catch (Exception ex)
            {
                Console.Writeline(ex.Message + ex.StackTrace);               
            }
        }    

```
---
<!-- markdownlint-enable MD024 -->
