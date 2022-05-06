---
title: Получение добавочных изменений для сообщений в папке
description: Разностный запрос позволяет запрашивать добавления, удаления или обновления для сообщений в папке с помощью ряда
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 1ad9bdefc50f4b3d2acd14643cb0a24ed74fca2d
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246386"
---
# <a name="get-incremental-changes-to-messages-in-a-folder"></a>Получение добавочных изменений для сообщений в папке

Запрос изменений позволяет запрашивать добавления, удаления или обновления сообщений в папке с помощью серии вызовов функции [delta](/graph/api/message-delta). Разностные данные позволяют поддерживать и синхронизировать локальное хранилище сообщений пользователя. При этом вам не требуется каждый раз получать весь набор сообщений пользователя с сервера.

Запрос изменений поддерживает как полную синхронизацию с получением всех сообщений в папке (например, в папке "Входящие" пользователя), так и добавочную синхронизацию с получением всех сообщений в этой папке, которые изменились с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация сообщений в папке, а затем в папку периодически добавляются изменения.

## <a name="track-message-changes-in-a-folder"></a>Отслеживание изменений сообщений в папке

Запрос изменений выполняется отдельно для каждой папки. Чтобы отслеживать изменения сообщений в иерархии папок, необходимо наблюдать за каждой папкой отдельно.

Как правило, цикл отслеживания изменений сообщений в папке почты состоит из одного или нескольких запросов GET с функцией **delta**. Исходный запрос GET во многом аналогичен [получению сообщений](/graph/api/user-list-messages), но он также содержит функцию **delta**:

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

Запрос GET с функцией **delta** возвращает одно из следующих значений:

- ссылку `@odata.nextLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _skipToken_);
- ссылку `@odata.deltaLink` (содержащую URL-адрес с вызовом функции **delta** и маркером _deltaToken_).

Это маркеры являются [маркерами состояния](delta-query-overview.md#state-tokens), полностью непрозрачными для клиента. Чтобы продолжить цикл отслеживания изменений, просто скопируйте и примените URL-адрес, полученный из последнего запроса GET, при следующем вызове функции **delta** для этой папки. Ссылка `@odata.deltaLink` в ответе означает, что текущий цикл отслеживания изменений завершен. Вы можете сохранить и использовать URL-адрес `@odata.deltaLink` в начале следующего цикла.

В приведенном ниже [примере](#example-to-synchronize-messages-in-a-folder) показано, как использовать URL-адреса `@odata.nextLink` и `@odata.deltaLink`.

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a>Использование параметров запроса изменений для сообщений

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство `id` возвращается всегда.
- Запросы изменений поддерживают параметры `$select`, `$top` и `$expand` для сообщений.
- Имеется ограниченная поддержка параметров `$filter` и `$orderby`:
  - Для параметра `$filter` поддерживаются только выражения `$filter=receivedDateTime+ge+{value}` и `$filter=receivedDateTime+gt+{value}`.
  - При применении `$filter` в разностном запросе возвращается только до 5 000 сообщений.
  - Для параметра `$orderby` поддерживается только выражение `$orderby=receivedDateTime+desc`. Если выражение `$orderby` не указано, результаты будут возвращаться в непредсказуемом порядке.
- Параметр `$search` не поддерживается.

### <a name="optional-request-header"></a>Необязательный заголовок запроса

Каждый запрос изменений GET возвращает коллекцию из одного или нескольких сообщений в ответе. При необходимости вы можете указать заголовок запроса `Prefer: odata.maxpagesize={x}`, чтобы задать максимальное количество сообщений в ответе.

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

## <a name="example-to-synchronize-messages-in-a-folder"></a>Пример синхронизации сообщений в папке

В приведенном ниже примере показаны 2 цикла синхронизации определенной папки, которая изначально содержала 5 сообщений.

В первом цикле выполняется серия из 3 запросов на синхронизацию всех 5 сообщений в папке:

- [Пример исходного запроса](#sample-initial-request) и [ответ](#sample-initial-response)
- [Пример второго запроса](#sample-second-request) и [ответ](#sample-second-response)
- [Пример третьего запроса](#sample-third-request) и [последний ответ](#sample-third-and-final-response)

После первого цикла одно из сообщений удаляется, а еще одно помечается как прочитанное. Во [втором цикле](#synchronize-messages-in-the-same-folder-in-the-next-round) синхронизации возвращаются только удаленные и обновленные сообщения. При этом не возвращаются сообщения, оставшиеся без изменений.

### <a name="sample-initial-request"></a>Пример исходного запроса

В этом примере указанная папка синхронизируется впервые, поэтому исходный запрос на синхронизацию не содержит маркер состояния. В этом цикле будут возвращены все сообщения из этой папки.

Первый запрос задает следующие параметры:

- параметр `$select` для возврата свойств `subject`, `sender` и `isRead` для каждого сообщения в ответе;
- [необязательный заголовок запроса](#optional-request-header) _odata.maxpagesize_, возвращающий 2 сообщения одновременно.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_1"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$select=subject,sender,isRead HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-initial-response"></a>Пример исходного ответа

Ответ включает два сообщения и заголовок ответа `@odata.nextLink`. URL-адрес `@odata.nextLink` указывает, что в папке еще остались сообщения.

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
      "isRead": false,
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
      "isRead": true,
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

### <a name="sample-second-request"></a>Пример второго запроса

Второй запрос указывает URL-адрес `@odata.nextLink`, полученный из предыдущего ответа. Обратите внимание, что в нем больше не требуется указывать тот же параметр `$select`, что и в исходном запросе, так как маркер `skipToken` в URL-адресе `@odata.nextLink` включает его в закодированном виде.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_2"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a>Пример второго ответа

Второй ответ содержит следующие 2 сообщения в папке и еще одну ссылку `@odata.nextLink`, указывающую, что в папке еще остались сообщения.

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

### <a name="sample-third-request"></a>Пример третьего запроса

Третий запрос продолжает использовать URL-адрес `@odata.nextLink`, полученный из последнего запроса на синхронизацию.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailFolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a>Пример третьего и последнего ответа

Третий ответ содержит последнее оставшееся сообщение из папки и URL-адрес `@odata.deltaLink`, указывающий, что синхронизация для этой папки пока что завершена. Сохраните URL-адрес `@odata.deltaLink` и используйте его в [следующем цикле синхронизации этой папки](#synchronize-messages-in-the-same-folder-in-the-next-round).

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

### <a name="synchronize-messages-in-the-same-folder-in-the-next-round"></a>Синхронизация сообщений из одной папки в следующем цикле

С помощью ссылки `@odata.deltaLink` из последнего цикла [прошлого запроса](#sample-third-request) вы сможете получить только те сообщения, которые изменились (путем добавления, удаления или обновления) в этой папке с момента последней синхронизации. При условии, что вы не хотите менять максимальный размер страницы ответа, первый запрос следующего цикла будет выглядеть следующим образом:

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_next"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```

Ответ содержит ссылку `@odata.deltaLink`. Это означает, что теперь синхронизированы все изменения в удаленной почтовой папке. Одно сообщение было удалено, а еще одно — изменено.

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

## <a name="see-also"></a>См. также

- [Запрос изменений Microsoft Graph](delta-query-overview.md)
- [Получение добавочных изменений для событий в представлении календаря](delta-query-events.md)
- [Получение добавочных изменений для групп](delta-query-groups.md)
- [Получение добавочных изменений пользователей](delta-query-users.md)
