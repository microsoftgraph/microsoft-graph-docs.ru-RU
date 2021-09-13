---
title: Получение добавочных изменений для групп
description: Разностный запрос позволяет запрашивать добавления, удаления или обновления групп с помощью вызовов разностных функций. Разностный запрос позволяет обнаруживать изменения в группах
author: davidmu1
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: cea4e335a02c2ebdf107cdfbca72072b0b18d2f3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142391"
---
# <a name="get-incremental-changes-for-groups"></a>Получение добавочных изменений для групп

[Запрос изменений](./delta-query-overview.md) позволяет запрашивать добавления, удаления или обновления групп с помощью серии вызовов функции [delta](/graph/api/group-delta?view=graph-rest-1.0). Запрос изменений позволяет находить изменения в группах. При этом не требуется получать полный набор групп из Microsoft Graph и сравнивать изменения.

Клиенты, выполняющие синхронизацию групп с локальным хранилищем профилей, в ближайшем будущем смогут использовать запрос изменений как для первичной полной синхронизации, так и для добавочной синхронизации. Как правило, сначала выполняется полная синхронизация групп в клиенте, а затем в группы периодически добавляются изменения.

## <a name="tracking-group-changes"></a>Отслеживание изменений в группах

Как правило, цикл отслеживания изменений в группах состоит из одного или нескольких запросов GET с функцией **delta**. Запрос GET совершается практически так же, как и при [получении списка групп](/graph/api/group-list?view=graph-rest-1.0), но в него нужно включить:

- функцию **delta**;
- [маркер состояния](./delta-query-overview.md) (*deltaToken* или *skipToken*) из данных предыдущего вызова функции **delta** в запросе GET.

## <a name="example"></a>Пример

В следующем примере показана серия запросов для отслеживания изменений в группах:

1. [Исходный запрос](#initial-request) и [ответ](#initial-response)
2. [Запрос nextLink](#nextlink-request) и [ответ](#nextlink-response)
3. [Последний запрос nextLink](#final-nextlink-request) и [ответ](#final-nextlink-response)
4. [Запрос deltaLink ](#deltalink-request) и [ответ deltaLink](#deltalink-response)

## <a name="initial-request"></a>Исходный запрос

Чтобы начать отслеживать изменения в ресурсе группы, необходимо совершить к нему запрос, включающий функцию delta.

Обратите внимание на следующее:

- Необязательный параметр `$select` включен в запрос, чтобы продемонстрировать, как параметры запроса автоматически включаются в последующие запросы.
- Необязательный параметр запроса `$select` также используется, чтобы показать, как участников групп можно получать вместе с объектами групп. Это позволяет отслеживать изменения членства, например добавление или удаление пользователей из групп.
- Исходный запрос не включает маркер состояния. Маркеры состояния будут использоваться в последующих запросах.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

## <a name="initial-response"></a>Исходный отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](/graph/api/resources/group?view=graph-rest-1.0) в тексте отклика. Если весь набор групп не помещается в один отклик, также будет включена ссылка `nextLink`, содержащая маркер состояния.

В этом примере в запрос включена ссылка `nextLink`. Исходный параметр запроса `$select` закодирован в маркере состояния.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

>**Примечание.** Свойство `members@delta` включено в первый объект группы — TestGroup1 — и содержит двух текущих членов группы. В объекте TestGroup2 отсутствует это свойство, так как в группе нет участников.

## <a name="nextlink-request"></a>Запрос nextLink

Во втором запросе используется ссылка `nextLink` из предыдущего запроса, содержащая маркер `skipToken`. Обратите внимание, что параметр `$select` не указан в явном виде, так как он закодирован в маркере.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>Ответ nextLink

Ответ содержит ссылку `nextLink` с новым значением `skipToken`, означающим, что доступны дополнительные группы. Вы должны продолжать выполнение запросов с использованием URL-адреса `nextLink`, пока в окончательном ответе не будет возвращен URL-адрес `deltaLink`, даже если значением является пустой массив (это может происходить при некоторых обстоятельствах).

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "3c8ac7c4-d365-4df9-abfa-356a9dd7763c"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="final-nextlink-request"></a>Последний запрос nextLink

В третьем запросе снова используется последняя ссылка `nextLink`.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Последний отклик nextLink

Наконец, возвращается URL-адрес `deltaLink`. Это означает, что больше нет данных о текущем состоянии групп. Для последующих запросов приложение использует ссылку `deltaLink` и содержащееся в ней значение `deltaToken`, чтобы узнавать о новых изменениях групп.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a>Запрос deltaLink

С помощью ссылки `deltaLink` из [последнего отклика](#final-nextlink-response) вы сможете получить новые изменения групп с момента последнего запроса. К таким изменениям относятся:
- создание объектов групп;
- удаление объектов групп;
- изменение свойств объектов групп (например, свойства **displayName**);
- добавление или удаление объектов членов в объектах групп.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>Отклик deltaLink

Если изменений не произошло, возвращается ссылка `deltaLink` без результатов (свойство `value` остается пустым). Обязательно замените предыдущую ссылку в приложении для использования в последующих запросах.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Если обнаружены изменения, в отклик включается коллекция измененных групп. Отклик также содержит ссылку `nextLink` (если требуется получить несколько страниц) или `deltaLink`. Следует реализовать такой же порядок перехода по ссылкам `nextLinks`, как и раньше, сохраняя заключительную ссылку `deltaLink` для последующих вызовов.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
          {
              "displayName": "TestGroup3",
              "description": "A test group for change tracking",
              "id": "2e5807ce-58f3-4a94-9b37-ffff2e085957",
              "members@delta": [
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
                      "@removed": {
                          "reason": "deleted"
                      }
                  },
                  {
                      "@odata.type": "#microsoft.graph.user",
                      "id": "37de1ae3-408f-4702-8636-20824abda004"
                  }
              ]
          }
      ]
}
```

Ниже представлены некоторые примечания к приведенному выше примеру ответа.

- Объекты возвращаются с тем же набором свойств, который изначально указывался с помощью параметра запроса `$select`.

- Включены как измененные, так и оставшиеся без изменений свойства. В приведенном выше примере свойство `description` содержит новое значение, а свойство `displayName` не изменилось.

- Свойство `members@delta` содержит все изменения членства.

  - Первый пользователь в списке был удален из группы путем удаления членства или самого объекта пользователя. Это описывается свойством `@removed`. Только пользователи, которые были удалены без возможности восстановления, удаляются из групп. Пользователи, которые были удалены временно, сохраняют членство в группах и не будут отображаться в разностном результате до окончательного удаления. Дополнительные сведения см. в статье [Каталог (удаленные элементы)](/graph/api/resources/directory?view=graph-rest-1.0).

  - Второй пользователь был добавлен в группу.

## <a name="paging-through-members-in-a-large-group"></a>Постраничный переход в случае списка членов большой группы

Свойство `members@delta` включается в объекты групп по умолчанию, если параметр `$select` не указан в запросе или параметр `$select=members` указан в явном виде. Если в группе много членов, данные о них могут не поместиться в один отклик. В этом разделе описан порядок обработки таких случаев.

>**Примечание.** Этот шаблон применяется как к получению исходного состояния группы, так и к последующим разностным запросам на получение изменений.

Предположим, что выполняется следующий разностный запрос (либо для регистрации полного исходного состояния групп, либо для получения изменений):

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

1. Microsoft Graph может вернуть отклик, содержащий только один объект группы с большим списком членов в свойстве `members@delta`:

**Первая страница**

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "632f6bb2-3ec8-4c1f-9073-0027a8c6859",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "37de1ae3-408f-4702-8636-20824abda004"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

2. Перейдя по ссылке `nextLink`, вы снова можете получить отклик с таким же объектом группы. Будут возвращены те же значения свойств, но свойство `members@delta` теперь содержит другой список пользователей.

**Вторая страница**

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=<...>",
  "value": [
    {
      "displayName":"LargeGroup",
      "description":"A group containing thousands of users",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "c08a463b-7b8a-40a4-aa31-f9bf690b9551",
              "@removed": {
                  "reason": "deleted"
              }
          },
          {
              "@odata.type": "#microsoft.graph.user",
              "id": "23423fa6-821e-44b2-aae4-d039d33884c2"
          },
          <...more users here...>
      ]
    }
    <...no more groups included - this group filled out the entire response...>
  ]
}
```

3. В конечном итоге будет возвращен весь список членов, и в отклике начнут появляться другие группы.

Для корректной реализации этого порядка следуйте приведенным ниже рекомендациям.
- Всегда переходите по ссылке `nextLink` и локально выполняйте объединение для состояния каждой группы. По мере получения откликов для одной и той же группы составляйте полный список членов в приложении.
- Не рекомендуем предполагать, что отклики будут представлены в определенной последовательности. Предполагайте, что одна и та же группа может встречаться в любом месте последовательности `nextLink`, и обрабатывайте этот случай в логике объединения.


## <a name="see-also"></a>См. также
Обзор [запросов изменений Microsoft Graph](delta-query-overview.md).
