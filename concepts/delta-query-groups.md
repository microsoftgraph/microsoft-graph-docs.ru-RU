---
title: Получение добавочных изменений для групп
description: 'Использование дельта-запроса для обнаружения изменений без извлечения всего набора групп для сравнения изменений. В следующем примере показана серия запросов для отслеживания изменений в группах:'
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 63ac88b147b2a10d27bb93c5b61e332e33b8153a
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555718"
---
# <a name="get-incremental-changes-for-groups"></a>Получение добавочных изменений для групп

[Разностный запрос](./delta-query-overview.md) в Microsoft Graph позволяет запрашивать добавления, удаления или обновления [поддерживаемых ресурсов](delta-query-overview.md#supported-resources). Он включается с помощью серии [дельта](/graph/api/group-delta?)-запросов. Для групп дельта-запрос позволяет обнаруживать изменения, не извлекая весь набор групп для сравнения изменений.

Клиенты, синхронизирующие группы с локальным хранилищем профилей, могут использовать разностный запрос как для начальной полной синхронизации, так и для последующих добавочных синхронизаций. Как правило, клиент выполняет первоначальную полную синхронизацию всех групп в клиенте, а затем периодически получает добавочные изменения в группах.

## <a name="track-changes-to-groups"></a>Отслеживание изменений в группах

Отслеживайте изменения групп с помощью одного или нескольких запросов GET с помощью **дельта**-функции. Запрос GET похож на запрос [групп списка](/graph/api/group-list?), за исключением следующих дополнительных объектов в URL:

- функцию **delta**;
- [маркер состояния](./delta-query-overview.md) (_deltaToken_ или _skipToken_) из данных предыдущего вызова функции **delta** в запросе GET.

## <a name="example-track-changes-to-groups"></a>Пример отслеживания изменений в группах

В следующем примере показана серия запросов для отслеживания изменений в группах:

1. [Исходный запрос](#initial-request) и [ответ](#initial-response)
2. [Запрос nextLink](#nextlink-request) и [отклик](#nextlink-response)
3. [Последний запрос nextLink](#final-nextlink-request) и [отклик](#final-nextlink-response)
4. [Запрос deltaLink ](#deltalink-request) и [отклик deltaLink](#deltalink-response)

Обратите внимание на следующее в ответах:

- При удалении группы (группы Microsoft 365) элемент содержит заметку: `@removed` со значением `"reason": "changed"`.
- При окончательном удалении группы (группа безопасности или [окончательное удаление группы Microsoft 365](/graph/api/directory-deleteditems-list.)) элемент содержит заметку: `@removed` со значением `"reason": "deleted"`.
- Заметок о создании или восстановлении группы не существует.

### <a name="initial-request"></a>Исходный запрос

Чтобы отслеживать изменения в групповом ресурсе, сделайте запрос и включите **дельта**-функцию в виде сегмента URL-адреса.

Обратите внимание на следующие элементы:

- Необязательный параметр `$select` включен в запрос, чтобы продемонстрировать, как параметры запроса автоматически включаются в последующие запросы.
- Необязательный параметр запроса `$select` также используется, чтобы показать, как участников групп можно получать вместе с объектами групп. Это позволяет отслеживать изменения членства, например добавление или удаление пользователей из групп.
- Первоначальный запрос не включает токен состояния. Токены состояния будут использоваться в последующих запросах.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,members
```

### <a name="initial-response"></a>Исходный отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [group](/graph/api/resources/group) в тексте отклика. Если весь набор групп не помещается в один отклик, также будет включена ссылка `@odata.nextLink`, содержащая маркер состояния.

В этом примере в запрос включена ссылка `@odata.nextLink`. Исходный параметр запроса `$select` закодирован в маркере состояния.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"All Company",
      "description":"This is the default group for everyone in the network",
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
      "displayName":"sg-HR",
      "description":"All HR personnel",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

> [!NOTE]
> `members@delta`Свойство включено в первый групповой объект — **Вся компания**— и содержит двух текущих участников группы. В объекте **sg-HR** отсутствует это свойство, так как в группе нет участников.

### <a name="nextlink-request"></a>Запрос nextLink

Во втором запросе используется ссылка `@odata.nextLink` из предыдущего запроса, содержащая маркер `skipToken`. Обратите внимание, что параметр `$select` не виден, так как он закодирован и включен в маркер.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

### <a name="nextlink-response"></a>Ответ nextLink

Ответ содержит ссылку `@odata.nextLink` с новым значением `skipToken`, означающим, что доступны дополнительные изменения, которые были отслежены для групп. Используйте URL-адрес `@odata.nextLink` в других запросах, пока URL-адрес `@odata.deltaLink` (в параметре `@odata.deltaLink`) не будет возвращен в окончательном ответе, даже если значение является пустым массивом.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Mark 8 Project Team",
      "description":"Mark 8 Project Team",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "632f6bb2-3ec8-4c1f-9073-0027a8c68593"
               }
      ]
    },
    {
      "displayName":"Sales and Marketing",
      "description":"Sales and Marketing",
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

### <a name="final-nextlink-request"></a>Последний запрос nextLink

Третий запрос использует последний `@odata.nextLink`, полученный из последнего запроса на синхронизацию.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

### <a name="final-nextlink-response"></a>Последний отклик nextLink

URL-адрес `@odata.deltaLink` возвращается, когда больше нет данных о существующем состоянии пользовательских объектов. Для будущих запросов приложение использует URL-адрес `@odata.deltaLink`, чтобы узнать об изменениях других пользователей. Сохраните `deltaToken` и используйте его в следующем URL-адресе запроса, чтобы узнать больше об изменениях для пользователей.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"All Employees",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"Remote living",
      "description":"Remote living",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

### <a name="deltalink-request"></a>Запрос deltaLink

Используя `@odata.deltaLink` из [последнего отклика](#final-nextlink-response), вы получите изменения (добавления, удаления или обновления) в группах с момента последнего запроса. Изменения включают:

- создание объектов групп;
- удаление объектов групп;
- Групповые объекты, для которых изменено свойство (например, **displayName** изменено).
- добавление или удаление объектов членов в объектах групп.

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

### <a name="deltalink-response"></a>Отклик deltaLink

Если изменений не произошло, возвращается ссылка `@odata.deltaLink` без результатов (свойство **value** остается пустым). Обязательно замените предыдущую ссылку в приложении для использования в последующих запросах.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Если обнаружены изменения, в отклик включается коллекция измененных групп. Отклик также содержит ссылку `@odata.nextLink` (если требуется получить несколько страниц) или `@odata.deltaLink`. Реализуйте такой же порядок перехода по ссылкам `@odata.nextLink`, сохраняя заключительную ссылку `@odata.deltaLink` для последующих вызовов.

> [!NOTE]
> Этот запрос может иметь задержки репликации для недавно созданных, обновленных или удаленных групп. Повторите `@odata.nextLink` или `@odata.deltaLink` через некоторое время, чтобы получить последние изменения.

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

Ниже представлены некоторые примечания к предыдущему примеру отклика.

- Объекты возвращаются с тем же набором свойств, который изначально указывался с помощью параметра запроса `$select`.

- Включаются как измененные, так и неизмененные свойства. В приведенном выше примере свойство `description` имеет новое значение, в то время как свойство `displayName` не изменилось.

- `members@delta` содержит следующие изменения членства в группе.

  - Первый пользователь в списке был удален из группы путем удаления членства или самого объекта пользователя. Это описывается свойством `@removed`. Только пользователи, которые были удалены без возможности восстановления, удаляются из групп. Пользователи, которые были удалены временно, сохраняют членство в группах и не будут отображаться в разностном результате до окончательного удаления. Дополнительные сведения см. в статье [Каталог (удаленные элементы)](/graph/api/resources/directory).

  - Второй пользователь был добавлен в группу.

## <a name="paging-through-members-in-a-large-group"></a>Постраничный переход в случае списка членов большой группы

Свойство `members@delta` включается в объекты групп по умолчанию, если параметр `$select` не указан в запросе или параметр `$select=members` указан в явном виде. Для групп с большим количеством участников возможно, что все участники не смогут поместиться в один ответ. Реализуйте следующий шаблон в таких случаях.

> [!NOTE]
> Этот шаблон применяется как к начальному получению состояния группы, так и к последующим вызовам для получения дельта-изменений.

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

2. Перейдя по ссылке `@odata.nextLink`, вы можете получить отклик с таким же объектом группы. Будут возвращены те же значения свойств, но свойство `members@delta` теперь содержит другой список пользователей.

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
- Всегда переходите по ссылке `@odata.nextLink` и локально выполняйте объединение для состояния каждой группы. По мере получения откликов для одной и той же группы составляйте полный список членов в приложении.
- Не предполагайте определенную последовательность ответов. Предположим, что одна и та же группа может появиться в любом месте последовательности `@odata.nextLink`, и обработайте это в своей логике слияния.


## <a name="see-also"></a>См. также
Обзор [запросов изменений Microsoft Graph](delta-query-overview.md).
