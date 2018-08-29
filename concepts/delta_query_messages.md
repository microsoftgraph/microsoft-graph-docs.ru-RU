# <a name="get-incremental-changes-to-messages-in-a-folder"></a><span data-ttu-id="acd82-101">Получение добавочных изменений для сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="acd82-101">Get incremental changes to messages in a folder</span></span>

<span data-ttu-id="acd82-p101">Запрос изменений позволяет запрашивать добавления, удаления или обновления сообщений в папке с помощью серии вызовов функции [delta](../api-reference/v1.0/api/message_delta.md). Разностные данные позволяют поддерживать и синхронизировать локальное хранилище сообщений пользователя. При этом вам не требуется каждый раз получать весь набор сообщений пользователя с сервера.</span><span class="sxs-lookup"><span data-stu-id="acd82-p101">Delta query lets you query for additions, deletions, or updates to messages in a folder, by way of a series of [delta](../api-reference/v1.0/api/message_delta.md) function calls. Delta data enables you to maintain and synchronize a local store of a user's messages, without having to fetch the entire set of the user's messages from the server every time.</span></span>

<span data-ttu-id="acd82-p102">Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в папке (например, в папке "Входящие" пользователя), так и добавочную синхронизацию с получением всех сообщений в этой папке, которые изменились с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация сообщений в папке, а затем в папку периодически добавляются изменения.</span><span class="sxs-lookup"><span data-stu-id="acd82-p102">Delta query supports both full synchronization that retrieves all of the messages in a folder (for example, the user's Inbox), and incremental synchronization that retrieves all of the messages that have changed in that folder since the last synchronization. Typically, you would do an initial full synchronization of all the messages in a folder, and subsequently, get incremental changes to that folder periodically.</span></span>

## <a name="track-message-changes-in-a-folder"></a><span data-ttu-id="acd82-106">Отслеживание изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="acd82-106">Track message changes in a folder</span></span>

<span data-ttu-id="acd82-p103">Запрос изменений выполняется отдельно для каждой папки. Чтобы отслеживать изменения сообщений в иерархии папок, необходимо наблюдать за каждой папкой отдельно.</span><span class="sxs-lookup"><span data-stu-id="acd82-p103">Delta query is a per-folder operation. To track the changes of the messages in a folder hierarchy, you need to track each folder individually.</span></span>

<span data-ttu-id="acd82-p104">Как правило, цикл отслеживания изменений сообщений в папке почты состоит из одного или нескольких запросов GET с функцией **delta**. Исходный запрос GET во многом аналогичен [получению сообщений](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), но он также содержит функцию **delta**:</span><span class="sxs-lookup"><span data-stu-id="acd82-p104">Tracking message changes in a mail folder typically is a round of one or more GET requests with the **delta** function. The initial GET request is very much like the way you [get messages](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), except that you include the **delta** function:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

<span data-ttu-id="acd82-111">Запрос GET с функцией **delta** возвращает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="acd82-111">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="acd82-112">ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _skipToken_);</span><span class="sxs-lookup"><span data-stu-id="acd82-112">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span>
- <span data-ttu-id="acd82-113">ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="acd82-113">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="acd82-p105">Это маркеры являются [маркерами состояния](delta_query_overview.md#state-tokens), полностью непрозрачными для клиента. Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес, полученный из последнего запроса GET, при следующем вызове функции **delta** для этой папки. Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен. Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.</span><span class="sxs-lookup"><span data-stu-id="acd82-p105">These tokens are [state tokens](delta_query_overview.md#state-tokens) that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next **delta** function call for the same folder. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="acd82-118">В приведенном ниже [примере](#example-to-synchronize-messages-in-a-folder) показано, как использовать URL-адреса `nextLink` и `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="acd82-118">See the [example](#example-to-synchronize-messages-in-a-folder) below to learn how to use the `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a><span data-ttu-id="acd82-119">Использование параметров запроса изменений для сообщений</span><span class="sxs-lookup"><span data-stu-id="acd82-119">Use query parameters in a delta query for messages</span></span>

- <span data-ttu-id="acd82-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство `id` возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="acd82-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The `id` property is always returned.</span></span>
- <span data-ttu-id="acd82-122">Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для сообщений.</span><span class="sxs-lookup"><span data-stu-id="acd82-122">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span>
- <span data-ttu-id="acd82-123">Имеется ограниченная поддержка параметров `$filter` и `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="acd82-123">There is limited support for `$filter` and `$orderby`:</span></span>
  - <span data-ttu-id="acd82-124">Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.</span><span class="sxs-lookup"><span data-stu-id="acd82-124">The only supported `$filter` expressions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  - <span data-ttu-id="acd82-p107">Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.</span><span class="sxs-lookup"><span data-stu-id="acd82-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span>
- <span data-ttu-id="acd82-127">Параметр `$search` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd82-127">There is no support for `$search`.</span></span>

### <a name="optional-request-header"></a><span data-ttu-id="acd82-128">Необязательный заголовок запроса</span><span class="sxs-lookup"><span data-stu-id="acd82-128">Optional request header</span></span>

<span data-ttu-id="acd82-129">Каждый разностный запрос GET возвращает в отклике коллекцию из одного или нескольких сообщений.</span><span class="sxs-lookup"><span data-stu-id="acd82-129">Each delta query GET request returns a collection of one or more messages in the response.</span></span> <span data-ttu-id="acd82-130">При необходимости вы можете указать заголовок запроса `Prefer: odata.maxpagesize={x}`, чтобы задать максимальное количество сообщений в отклике.</span><span class="sxs-lookup"><span data-stu-id="acd82-130">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of messages in a response.</span></span>

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

6. When you eventually receive a _deltaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This
round of change tracking is complete.

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated)
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a><span data-ttu-id="acd82-131">Пример синхронизации сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="acd82-131">Example to synchronize messages in a folder</span></span>

<span data-ttu-id="acd82-132">В приведенном ниже примере показаны 2 цикла синхронизации определенной папки, которая изначально содержала 5 сообщений.</span><span class="sxs-lookup"><span data-stu-id="acd82-132">The following example shows 2 rounds of synchronization of a specific folder which initially contains 5 messages.</span></span>

<span data-ttu-id="acd82-133">В первом цикле выполняется серия из 3 запросов на синхронизацию всех 5 сообщений в папке:</span><span class="sxs-lookup"><span data-stu-id="acd82-133">The first round involves a series of 3 requests to synchronize all 5 messages in the folder:</span></span>

- <span data-ttu-id="acd82-134">[Пример исходного запроса](#sample-initial-request) и [ответ](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="acd82-134">[Sample initial request](#sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="acd82-135">[Пример второго запроса](#sample-second-request) и [ответ](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="acd82-135">[Sample second request](#sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="acd82-136">[Пример третьего запроса](#sample-third-request) и [последний ответ](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="acd82-136">[Sample third request](#sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="acd82-137">После первого цикла одно из сообщений удаляется, а еще одно помечается как прочитанное.</span><span class="sxs-lookup"><span data-stu-id="acd82-137">After the first round, one of the messages is deleted, and another is marked as read.</span></span> <span data-ttu-id="acd82-138">Во [втором цикле](#synchronize-messages-in-the-same-folder-in-the-next-round) синхронизации возвращаются только удаленные и обновленные сообщения. При этом не возвращаются сообщения, оставшиеся без изменений.</span><span class="sxs-lookup"><span data-stu-id="acd82-138">The [second round](#synchronize-messages-in-the-same-folder-in-the-next-round) of synchronization returns only the delta (the deletion and update), without returning the other messages that have remained the same.</span></span>

### <a name="sample-initial-request"></a><span data-ttu-id="acd82-139">Пример исходного запроса</span><span class="sxs-lookup"><span data-stu-id="acd82-139">Sample initial request</span></span>

<span data-ttu-id="acd82-p110">В этом примере указанная папка синхронизируется впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния. В этом цикле будут возвращены все сообщения из этой папки.</span><span class="sxs-lookup"><span data-stu-id="acd82-p110">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the messages in that folder.</span></span>

<span data-ttu-id="acd82-142">Первый запрос задает следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="acd82-142">The first request specifies the following:</span></span>

- <span data-ttu-id="acd82-143">параметр `$select` для возврата свойств `subject`, `sender` и `isRead` для каждого сообщения в ответе;</span><span class="sxs-lookup"><span data-stu-id="acd82-143">A `$select` parameter to return the `subject`, `sender`, and `isRead` properties for each message in the response.</span></span>
- <span data-ttu-id="acd82-144">[необязательный заголовок запроса](#optional-request-header) _odata.maxpagesize_, возвращающий 2 сообщения одновременно.</span><span class="sxs-lookup"><span data-stu-id="acd82-144">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 messages at a time.</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_1"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$select=subject,sender,isRead HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-initial-response"></a><span data-ttu-id="acd82-145">Пример исходного ответа</span><span class="sxs-lookup"><span data-stu-id="acd82-145">Sample initial response</span></span>

<span data-ttu-id="acd82-p111">Ответ включает два сообщения и заголовок ответа `@odata.nextLink`. URL-адрес `nextLink` указывает, что в папке еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="acd82-p111">The response includes two messages and an `@odata.nextLink` response header. The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "false",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
      "subject": "Holiday promotion sale",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Samantha Booth",
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAVRMKAAAAA=="
    }
  ]
}
```

### <a name="sample-second-request"></a><span data-ttu-id="acd82-148">Пример второго запроса</span><span class="sxs-lookup"><span data-stu-id="acd82-148">Sample second request</span></span>

<span data-ttu-id="acd82-p112">Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа. Обратите внимание, что в нем больше не требуется указывать тот же параметр `$select`, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает его в закодированном виде.</span><span class="sxs-lookup"><span data-stu-id="acd82-p112">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same `$select` parameter as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes it.</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_2"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="acd82-151">Пример второго ответа</span><span class="sxs-lookup"><span data-stu-id="acd82-151">Sample second response</span></span>

<span data-ttu-id="acd82-152">Второй ответ содержит следующие 2 сообщения в папке и еще одну ссылку `nextLink`, указывающую, что в папке еще остались сообщения.</span><span class="sxs-lookup"><span data-stu-id="acd82-152">The second response returns the next 2 messages in the folder and another `nextLink`, indicating there are more messages to get from the folder.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlqfdAAAEfYB+\"",
      "subject": "Microsoft Virtual Academy at Contoso",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Elliot Hyde",
          "address": "elliot-hyde@tailspintoys.com"
        }
      },
      "id": "AQMkADNkNAAAgWkAAAA"
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "New or modified user account information",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Randi Welch",
          "address": "randiw@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAgWJAAAA"
    }
  ]
}
```

### <a name="sample-third-request"></a><span data-ttu-id="acd82-153">Пример третьего запроса</span><span class="sxs-lookup"><span data-stu-id="acd82-153">Sample third request</span></span>

<span data-ttu-id="acd82-154">Третий запрос продолжает использовать URL-адрес `nextLink`, полученный из последнего запроса на синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="acd82-154">The third request continues to use the latest `nextLink` URL returned from the last sync request.</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailFolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="acd82-155">Пример третьего и последнего ответа</span><span class="sxs-lookup"><span data-stu-id="acd82-155">Sample third and final response</span></span>

<span data-ttu-id="acd82-p113">Третий ответ содержит последнее оставшееся сообщение из папки и URL-адрес `deltaLink`, указывающий, что синхронизация для этой папки пока что завершена. Сохраните URL-адрес `deltaLink` и используйте его в [следующем цикле синхронизации этой папки](#synchronize-messages-in-the-same-folder-in-the-next-round).</span><span class="sxs-lookup"><span data-stu-id="acd82-p113">The third response returns the only remaining message in the folder, and a `deltaLink` URL which indicates synchronization is complete for the time being for this folder. Save and use the `deltaLink` URL to [synchronize the same folder in the next round](#synchronize-messages-in-the-same-folder-in-the-next-round).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzFPjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "Fabric CDN now available",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Jodie Sharp",
          "address": "Jodie.Sharp@contoso.com"
        }
      },
      "id": "AAMkADk0MGFkODE3LWEAAA="
    }
  ]
}
```

### <a name="synchronize-messages-in-the-same-folder-in-the-next-round"></a><span data-ttu-id="acd82-158">Синхронизация сообщений из одной папки в следующем цикле</span><span class="sxs-lookup"><span data-stu-id="acd82-158">Synchronize messages in the same folder in the next round</span></span>

<span data-ttu-id="acd82-p114">С помощью ссылки `deltaLink` из последнего цикла [прошлого запроса](#sample-third-request) вы сможете получить только те сообщения, которые изменились (путем добавления, удаления или обновления) в этой папке с момента последней синхронизации. При условии, что вы не хотите менять максимальный размер страницы ответа, первый запрос следующего цикла будет выглядеть следующим образом:</span><span class="sxs-lookup"><span data-stu-id="acd82-p114">Using the `deltaLink` from the [last request](#sample-third-request) in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_next"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```

<span data-ttu-id="acd82-161">Ответ содержит ссылку `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="acd82-161">The response contains a `deltaLink`.</span></span> <span data-ttu-id="acd82-162">Это означает, что теперь синхронизированы все изменения в удаленной почтовой папке.</span><span class="sxs-lookup"><span data-stu-id="acd82-162">This indicates that all changes in the remote mail folder are now synchronized.</span></span> <span data-ttu-id="acd82-163">Одно сообщение было удалено, а еще одно — изменено.</span><span class="sxs-lookup"><span data-stu-id="acd82-163">One message was deleted and the other message was changed.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS0Dh_6qB-pB2Sa2pUum19a6YAAKnLuxoAAA=",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="acd82-164">См. также</span><span class="sxs-lookup"><span data-stu-id="acd82-164">See also</span></span>

- [<span data-ttu-id="acd82-165">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="acd82-165">Microsoft Graph delta query</span></span>](delta_query_overview.md)
- [<span data-ttu-id="acd82-166">Получение добавочных изменений для событий в представлении календаря</span><span class="sxs-lookup"><span data-stu-id="acd82-166">Get incremental changes to events in a calendar view</span></span>](delta_query_events.md)
- [<span data-ttu-id="acd82-167">Получение добавочных изменений для групп</span><span class="sxs-lookup"><span data-stu-id="acd82-167">Get incremental changes to groups</span></span>](delta_query_groups.md)
- [<span data-ttu-id="acd82-168">Получение добавочных изменений пользователей</span><span class="sxs-lookup"><span data-stu-id="acd82-168">Get incremental changes to users</span></span>](delta_query_users.md)
