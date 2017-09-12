# <a name="get-incremental-changes-to-messages-in-a-folder"></a>Получение добавочных изменений для сообщений в папке 

Запрос изменений позволяет запрашивать добавления, удаления или обновления сообщений в папке с помощью серии вызовов функции [delta](../api-reference/v1.0/api/message_delta.md). Разностные данные позволяют поддерживать и синхронизировать локальное хранилище сообщений пользователя. При этом вам не требуется каждый раз получать весь набор сообщений пользователя с сервера.

Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в папке (например, в папке "Входящие" пользователя), так и добавочную синхронизацию с получением всех сообщений в этой папке, которые изменились с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация сообщений в папке, а затем в папку периодически добавляются изменения. 

## <a name="track-message-changes-in-a-folder"></a>Отслеживание изменений сообщений в папке

Запрос изменений выполняется отдельно для каждой папки. Чтобы отслеживать изменения сообщений в иерархии папок, необходимо наблюдать за каждой папкой отдельно. 

Как правило, цикл отслеживания изменений сообщений в папке почты состоит из одного или нескольких запросов GET с функцией **delta**. Исходный запрос GET во многом аналогичен [получению сообщений](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), но он также содержит функцию **delta**:

```
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

Запрос GET с функцией **delta** возвращает одно из следующих значений:

- ссылку `nextLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _skipToken_); 
- ссылку `deltaLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _deltaToken_).

Это маркеры являются [маркерами состояния](delta_query_overview.md#state-tokens), полностью непрозрачными для клиента. Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес, полученный из последнего запроса GET, при следующем вызове функции **delta** для этой папки. Ссылка `deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен. Вы можете сохранить и использовать URL-адрес `deltaLink` в начале следующего цикла.

В приведенном ниже [примере](#example-to-synchronize-messages-in-a-folder) показано, как использовать URL-адреса `nextLink` и `deltaLink`.

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a>Использование параметров запроса изменений для сообщений

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда. 
- Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для сообщений. 
- Имеется ограниченная поддержка параметров `$filter` и `$orderby`:
  * Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.
  * Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке. 
- Параметр `$search` не поддерживается.


### <a name="optional-request-header"></a>Необязательный заголовок запроса

Каждый запрос изменений GET возвращает коллекцию из одного или нескольких сообщений в ответе. При необходимости вы можете указать заголовок запроса _Prefer: odata.maxpagesize={x}_, чтобы задать максимальное количество сообщений в ответе.

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

## <a name="example-to-synchronize-messages-in-a-folder"></a>Пример синхронизации сообщений в папке

В следующем примере показана серия из 3 запросов, синхронизирующих определенную папку, которая содержит 5 сообщений:

- [Пример исходного запроса](#sample-initial-request) и [ответ](#sample-initial-response)
- [Пример второго запроса](#sample-second-request) и [ответ](#sample-second-response)
- [Пример третьего запроса](#sample-third-request) и [последний ответ](#sample-third-and-final-response)

См. также, что можно сделать в [следующем цикле](#the-next-round).


### <a name="sample-initial-request"></a>Пример исходного запроса

В этом примере указанная папка синхронизируется впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния. В этом цикле будут возвращены все сообщения из этой папки.

Первый запрос задает следующие параметры:

- Параметр `$select` для возврата свойств **Subject** и **Sender** каждого сообщения в ответе.
- [необязательный заголовок запроса](#optional-request-header) _odata.maxpagesize_, возвращающий 2 сообщения одновременно.

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_1"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$select=Subject,Sender HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a>Пример исходного ответа

Ответ включает два сообщения и заголовок ответа `@odata.nextLink`. URL-адрес `nextLink` указывает, что в папке еще остались сообщения.

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

### <a name="sample-second-request"></a>Пример второго запроса

Второй запрос указывает URL-адрес `nextLink`, полученный из предыдущего ответа. Обратите внимание, что в нем больше не требуется указывать тот же параметр `$select`, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `nextLink` включает его в закодированном виде.

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_2"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a>Пример второго ответа 

Второй ответ содержит следующие 2 сообщения в папке и еще одну ссылку `nextLink`, указывающую, что в папке еще остались сообщения.

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


### <a name="sample-third-request"></a>Пример третьего запроса

Третий запрос продолжает использовать URL-адрес `nextLink`, полученный из последнего запроса на синхронизацию. 

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a>Пример третьего и последнего ответа

Третий ответ содержит последнее оставшееся сообщение из папки и URL-адрес `deltaLink`, указывающий, что синхронизация для этой папки пока что завершена. Сохраните URL-адрес `deltaLink` и используйте его в [следующем цикле синхронизации этой папки](#the-next-round).

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


### <a name="the-next-round"></a>Следующий цикл

С помощью ссылки `deltaLink` из последнего цикла [прошлого запроса](#sample-third-request) вы сможете получить только те сообщения, которые изменились (путем добавления, удаления или обновления) в этой папке с момента последней синхронизации. При условии, что вы не хотите менять максимальный размер страницы ответа, первый запрос следующего цикла будет выглядеть следующим образом:

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_next"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```



## <a name="see-also"></a>См. также

- [Запрос изменений Microsoft Graph](../Concepts/delta_query_overview.md)
- [Получение добавочных изменений для событий в представлении календаря](../Concepts/delta_query_events.md)
- [Получение добавочных изменений для групп](../Concepts/delta_query_groups.md)
- [Получение добавочных изменений для пользователей](../Concepts/delta_query_users.md)
