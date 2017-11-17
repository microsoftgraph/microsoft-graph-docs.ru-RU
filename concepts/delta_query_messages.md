# <a name="get-incremental-changes-to-messages-in-a-folder"></a><span data-ttu-id="76bee-101">Получение добавочных изменений для сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="76bee-101">Get incremental changes to messages in a folder</span></span> 

<span data-ttu-id="76bee-p101">Запрос изменений позволяет запрашивать добавления, удаления или обновления сообщений в папке с помощью серии вызовов функции [delta](../api-reference/v1.0/api/message_delta.md). Разностные данные позволяют поддерживать и синхронизировать локальное хранилище сообщений пользователя. При этом вам не требуется каждый раз получать весь набор сообщений пользователя с сервера.</span><span class="sxs-lookup"><span data-stu-id="76bee-p101">Delta query lets you query for additions, deletions, or updates to messages in a folder, by way of a series of [delta](../api-reference/v1.0/api/message_delta.md) function calls. Delta data enables you to maintain and synchronize a local store of a user's messages, without having to fetch the entire set of the user's messages from the server every time.</span></span>

<span data-ttu-id="76bee-p102">Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в папке (например, в папке "Входящие" пользователя), так и добавочную синхронизацию с получением всех сообщений в этой папке, которые изменились с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация сообщений в папке, а затем в папку периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="76bee-p102">Delta query supports both full synchronization that retrieves all of the messages in a folder (for example, the user's Inbox), and incremental synchronization that retrieves all of the messages that have changed in that folder since the last synchronization. Typically, you would do an initial full synchronization of all the messages in a folder, and subsequently, get incremental changes to that folder periodically.</span></span> 

## <a name="track-message-changes-in-a-folder"></a><span data-ttu-id="76bee-106">Отслеживание изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="76bee-106">Track message changes in a folder</span></span>

<span data-ttu-id="76bee-p103">Запрос изменений выполняется отдельно для каждой папки. Чтобы отслеживать изменения сообщений в иерархии папок, необходимо наблюдать за каждой папкой отдельно.</span><span class="sxs-lookup"><span data-stu-id="76bee-p103">Delta query is a per-folder operation. To track the changes of the messages in a folder hierarchy, you need to track each folder individually.</span></span> 

<span data-ttu-id="76bee-p104">Как правило, цикл отслеживания изменений сообщений в папке почты состоит из одного или нескольких запросов GET с функцией **delta**. Исходный запрос GET во многом аналогичен [получению сообщений](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), но он также содержит функцию **delta**:</span><span class="sxs-lookup"><span data-stu-id="76bee-p104">Tracking message changes in a mail folder typically is a round of one or more GET requests with the **delta** function. The initial GET request is very much like the way you [get messages](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), except that you include the **delta** function:</span></span>

```
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

<span data-ttu-id="76bee-111">Запрос GET с функцией **delta** возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="76bee-111">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="76bee-112">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _skipToken_);</span><span class="sxs-lookup"><span data-stu-id="76bee-112">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="76bee-113">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="76bee-113">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="76bee-p105">Это маркеры являются [маркерами состояния](delta_query_overview.md#state-tokens), полностью непрозрачными для клиента. Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес, полученный из последнего запроса GET, при следующем вызове функции **delta** для этой папки. Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен. Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="76bee-p105">These tokens are [state tokens](delta_query_overview.md#state-tokens) that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next **delta** function call for the same folder. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="76bee-118">В приведенном ниже [примере](#example-to-synchronize-messages-in-a-folder) показано, как использовать URL-адреса `nextLink` и `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="76bee-118">See the [example](#example-to-synchronize-messages-in-a-folder) below to learn how to use the `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a><span data-ttu-id="76bee-119">Использование параметров запроса изменений для сообщений</span><span class="sxs-lookup"><span data-stu-id="76bee-119">Use query parameters in a delta query for messages</span></span>

- <span data-ttu-id="76bee-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="76bee-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="76bee-122">Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для сообщений.</span><span class="sxs-lookup"><span data-stu-id="76bee-122">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="76bee-123">Имеется ограниченная поддержка параметров `$filter` и `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="76bee-123">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="76bee-124">Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="76bee-124">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="76bee-p107">Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.</span><span class="sxs-lookup"><span data-stu-id="76bee-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="76bee-127">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76bee-127">There is no support for `$search`.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="76bee-128">Необязательный заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="76bee-128">Optional request header</span></span>

<span data-ttu-id="76bee-129">Каждый разностный запрос GET возвращает в отклике коллекцию из одного или нескольких сообщений.</span><span class="sxs-lookup"><span data-stu-id="76bee-129">Each delta query GET request returns a collection of one or more messages in the response. You can optionally specify the request header, Prefer: odata.maxpagesize={x}, to set the maximum number of messages in a response.</span></span> <span data-ttu-id="76bee-130">При необходимости вы можете указать заголовок запроса `Prefer: odata.maxpagesize={x}`, чтобы задать максимальное количество сообщений в отклике.</span><span class="sxs-lookup"><span data-stu-id="76bee-130">Each delta query GET request returns a collection of one or more messages in the response. You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of messages in a response.</span></span>

<!--
### Iterative process 

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query 
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative 
process (steps 2-6) described below will return the entire set of messages in that folder. 

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header, 
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned 
   in _@odata.nextLink_, which includes a _skipToken_. 

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages, 
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3. 

6. When you eventually receive a _detlaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This 
round of change tracking is complete. 

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request 
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated) 
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a><span data-ttu-id="76bee-131">Пример синхронизации сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="76bee-131">Example to synchronize messages in a folder</span></span>

<span data-ttu-id="76bee-132">В следующем примере показана серия из 3 запросов, синхронизирующих определенную папку, которая содержит 5 сообщений:</span><span class="sxs-lookup"><span data-stu-id="76bee-132">The following example shows a series of 3 requests to synchronize a specific folder which contains 5 messages:</span></span>

- <span data-ttu-id="76bee-133">[Пример исходного запроса](#sample-initial-request) и [ответ](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="76bee-133">[Sample initial request](#sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="76bee-134">[Пример второго запроса](#sample-second-request) и [ответ](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="76bee-134">[Sample second request](#sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="76bee-135">[Пример третьего запроса](#sample-third-request) и [последний ответ](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="76bee-135">[Sample third request](#sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="76bee-136">См. также, что можно сделать в [следующем цикле](#the-next-round).</span><span class="sxs-lookup"><span data-stu-id="76bee-136">See also what you'll do in the [next round](#the-next-round).</span></span>


### <a name="sample-initial-request"></a><span data-ttu-id="76bee-137">Пример исходного запроса</span><span class="sxs-lookup"><span data-stu-id="76bee-137">Sample initial request</span></span>

<span data-ttu-id="76bee-p109">В этом примере указанная папка синхронизируется впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния. В этом цикле будут возвращены все сообщения из этой папки.</span><span class="sxs-lookup"><span data-stu-id="76bee-p109">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the messages in that folder.</span></span>

<span data-ttu-id="76bee-140">Первый запрос задает следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="76bee-140">The first request specifies the following:</span></span>

- <span data-ttu-id="76bee-141">Параметр `$select` для возврата свойств **Subject** и **Sender** каждого сообщения в ответе.</span><span class="sxs-lookup"><span data-stu-id="76bee-141">A `$select` parameter to return the **Subject** and **Sender** properties for each message in the response.</span></span>
- <span data-ttu-id="76bee-142">[необязательный заголовок запроса](#optional-request-header) _odata.maxpagesize_, возвращающий 2 сообщения одновременно.</span><span class="sxs-lookup"><span data-stu-id="76bee-142">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 messages at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_1"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$select=Subject,Sender HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="76bee-143">Пример исходного ответа</span><span class="sxs-lookup"><span data-stu-id="76bee-143">Sample initial response</span></span>

<span data-ttu-id="76bee-p110">Ответ включает два сообщения и заголовок ответа `@odata.nextLink`. URL-адрес `nextLink` указывает, что в папке еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="76bee-p110">The response includes two messages and an `@odata.nextLink` response header. The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
            "subject":"Holiday hours update",
            "sender":{
                "emailAddress":{
                    "name":"Dana Swope",
                    "address":"danas@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADNkNAAASq35xAAA="
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
            "subject":"Holiday promotion sale",
            "sender":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAVRMKAAAAA=="
        }
    ]
}
```

### <a name="sample-second-request"></a><span data-ttu-id="76bee-146">Пример второго запроса</span><span class="sxs-lookup"><span data-stu-id="76bee-146">Sample second request</span></span>

<span data-ttu-id="76bee-p111">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа. Обратите внимание, что в нем больше не требуется указывать тот же параметр `$select`, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает его в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="76bee-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same `$select` parameter as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_2"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="76bee-149">Пример второго ответа</span><span class="sxs-lookup"><span data-stu-id="76bee-149">Sample second response</span></span> 

<span data-ttu-id="76bee-150">Второй ответ содержит следующие 2 сообщения в папке и еще одну ссылку `nextLink`, указывающую, что в папке еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="76bee-150">The second response returns the next 2 messages in the folder and another `nextLink`, indicating there are more messages to get from the folder.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWJAAAA"
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB9\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWHAAAA"
        }
    ]
}
```


### <a name="sample-third-request"></a><span data-ttu-id="76bee-151">Пример третьего запроса</span><span class="sxs-lookup"><span data-stu-id="76bee-151">Sample third request</span></span>

<span data-ttu-id="76bee-152">Третий запрос продолжает использовать URL-адрес `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="76bee-152">The third request continues to use the latest `nextLink` URL returned from the last sync request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="76bee-153">Пример третьего и последнего ответа</span><span class="sxs-lookup"><span data-stu-id="76bee-153">Sample third and final response</span></span>

<span data-ttu-id="76bee-p112">Третий ответ содержит последнее оставшееся сообщение из папки и URL-адрес `deltaLink`, указывающий, что синхронизация для этой папки пока что завершена. Сохраните URL-адрес `deltaLink` и используйте его в [следующем цикле синхронизации этой папки](#the-next-round).</span><span class="sxs-lookup"><span data-stu-id="76bee-p112">The third response returns the only remaining message in the folder, and a `deltaLink` URL which indicates synchronization is complete for the time being for this folder. Save and use the `deltaLink` URL to [synchronize the same folder in the next round](#the-next-round).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB8\"",
            "subject":"You've joined the Customer Manager group",
            "sender":{
                "emailAddress":{
                    "name":"Customer Managers team",
                    "address":"customer_managers@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWFAAAA"
        }
    ]
}
```


### <a name="the-next-round"></a><span data-ttu-id="76bee-156">Следующий цикл</span><span class="sxs-lookup"><span data-stu-id="76bee-156">The next round</span></span>

<span data-ttu-id="76bee-p113">С помощью ссылки `deltaLink` из последнего цикла [прошлого запроса](#sample-third-request) вы сможете получить только те сообщения, которые изменились (путем добавления, удаления или обновления) в этой папке с момента последней синхронизации. При условии, что вы не хотите менять максимальный размер страницы ответа, первый запрос следующего цикла будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="76bee-p113">Using the `deltaLink` from the [last request](#sample-third-request) in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_next"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```



## <a name="see-also"></a><span data-ttu-id="76bee-159">См. также</span><span class="sxs-lookup"><span data-stu-id="76bee-159">See also</span></span>

- [<span data-ttu-id="76bee-160">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="76bee-160">Microsoft Graph delta query</span></span>](../Concepts/delta_query_overview.md)
- [<span data-ttu-id="76bee-161">Получение добавочных изменений для событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="76bee-161">Get incremental changes to events in a calendar view</span></span>](../Concepts/delta_query_events.md)
- [<span data-ttu-id="76bee-162">Получение добавочных изменений для групп</span><span class="sxs-lookup"><span data-stu-id="76bee-162">Get incremental changes to groups</span></span>](../Concepts/delta_query_groups.md)
- [<span data-ttu-id="76bee-163">Получение добавочных изменений для пользователей</span><span class="sxs-lookup"><span data-stu-id="76bee-163">Get incremental changes to users</span></span>](../Concepts/delta_query_users.md)
