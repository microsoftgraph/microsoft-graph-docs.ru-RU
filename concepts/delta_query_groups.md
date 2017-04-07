# <a name="get-incremental-changes-for-groups-preview"></a>Получение добавочных изменений для групп (предварительная версия)

[Запрос изменений](./delta_query_overview.md) позволяет запрашивать добавления, удаления или обновления групп с помощью серии вызовов функции [delta](../api-reference/beta/api/group_delta.md). Запрос изменений позволяет находить изменения в группах. При этом не требуется получать полный набор групп из Microsoft Graph и сравнивать изменения.

Запрос изменений поддерживает как полную синхронизацию с получением всех групп в клиенте, так и добавочную синхронизацию с получением тех групп, которые изменились с момента последней синхронизации. Как правило, сначала выполняется полная синхронизация групп в клиенте, а затем в группы периодически добавляются изменения. 

## <a name="tracking-group-changes"></a>Отслеживание изменений в группах

Как правило, цикл отслеживания изменений в группах состоит из одного или нескольких запросов GET с функцией **delta**. Запрос GET совершается практически так же, как и при [получении списка групп](../api-reference/beta/api/group_list.md), но в него нужно включить:

- функцию **delta**;
- [маркер состояния](./delta_query_overview.md) (_deltaToken_ или _skipToken_) из предыдущего вызова функции **delta** в запросе GET.

## <a name="example"></a>Пример

В следующем примере показана серия запросов для отслеживания изменений в группах:

1. [Исходный запрос](#initial-request) и [ответ](#initial-response)
2. [Запрос nextLink](#nextlink-request) и [ответ](#nextlink-response)
3. [Последний запрос nextLink](#final-nextlink-request) и [ответ](#final-nextlink-response)
4. [Запрос deltaLink ](#deltalink-request) и [ответ deltaLink](#deltalink-response)

## <a name="initial-request"></a>Исходный запрос

Чтобы начать отслеживать изменения в ресурсе группы, необходимо совершить к нему запрос, включающий функцию delta. 

Обратите внимание на следующее:

- Необязательный параметр $select включен в запрос, чтобы продемонстрировать, как параметры запроса автоматически включаются в последующие запросы.
- Исходный запрос не включает маркер состояния. Маркеры состояния будут использоваться в последующих запросах.

``` http
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description
```

### <a name="initial-response"></a>Исходный ответ

В случае успеха этот метод возвращает код ответа `200, OK` и объект коллекции [group](../api-reference/beta/resources/group.md) в тексте ответа. Если полный набор групп не помещается на одну страницу, ответ также будет включать маркер состояния nextLink.

В этом примере возвращается URL-адрес nextLink. Это означает, что в текущем сеансе можно получить дополнительные страницы данных. Параметр $select из исходного запроса кодируется в URL-адресе nextLink.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff"
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

## <a name="nextlink-request"></a>Запрос nextLink

Второй запрос указывает маркер `skipToken`, полученный из предыдущего ответа. Обратите внимание, что параметр `$select` указывать не обязательно, так как `skipToken` включает его в закодированном виде.

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a>Ответ nextLink

Ответ содержит ссылку `nextLink` и еще один маркер `skipToken`, означающий, что доступны дополнительные группы. Вы продолжаете совершать запросы с использованием URL-адреса nextLink, пока в ответе не будет возвращен URL-адрес deltaLink.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957"
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505"
    }
  ]
}
```

## <a name="final-nextlink-request"></a>Последний запрос nextLink

Третий запрос продолжает использовать маркер `skipToken`, полученный из последнего запроса на синхронизацию. 

``` http
GET https://graph.microsoft.com/beta/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Последний ответ nextLink

Когда возвращается URL-адрес deltaLink, это означает, что больше нет данных о текущем состоянии ресурса. В последующих запросах приложение использует URL-адрес deltaLink, чтобы узнавать об изменениях ресурса. Сохраните маркер `deltaToken` и используйте его в URL-адресе запроса, чтобы находить изменения в группах. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
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

С помощью маркера `deltaToken` из [последнего ответа](#final-nextlink-response) вы сможете получить группы, измененные (добавленные, удаленные или обновленные) с момента последнего запроса.

``` http
GET https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a>Ответ deltaLink

Если изменений не произошло, возвращается тот же маркер `deltatoken` без результатов.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

Если же обнаружены изменения, возвращается маркер `deltatoken`, включающий коллекцию измененных групп.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup7",
      "description":"Employees in test group 7",
      "id":"f764235c-ffff-4843-a14a-1d8826967260"
    }
  ]
}
```

## <a name="see-also"></a>См. также
Обзор [запросов изменений Microsoft Graph](../concepts/delta_query_overview.md).