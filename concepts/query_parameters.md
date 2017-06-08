# <a name="customize-responses-optional-query-parameters"></a>Настройка откликов: необязательные параметры запросов

В Microsoft Graph предусмотрены необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных. Поддерживаются приведенные ниже параметры запросов.

|Имя|Описание|Примеры (щелкните пример, чтобы попробовать поработать с ним в [песочнице Graph][graph-explorer])
|:---------------|:--------|:-------|
|[$filter](#filter)|Фильтрует результаты (строки).|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[$select](#select)|Фильтрует свойства (столбцы).|[`/users?$select=givenName,surname`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[$expand](#expand)|Получает связанные ресурсы.|[`/groups/{id}?$expand=members`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/22be6ccb-15a5-459f-94ac-d1393bdd9e66?$expand=members&method=GET&version=v1.0)
|[$orderby](#orderby)|Упорядочивает результаты.|[`/users?$orderby=displayName,userPrincipalName desc`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$orderby=displayName,userPrincipalName%20DESC&method=GET&version=v1.0)
|[$top](#top)|Ограничивает результаты. Обычно используется вместе с параметром `$skipToken`.|[`/users?$top=2`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)
|[$skipToken](#skiptoken)|Используется вместе с параметром `$top` для получения страницы результатов.|Пример см. в описании `nextLink` из запроса $top.
|[$count](#count)|Возвращает общее количество соответствующих ресурсов.|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
<!-- TODO: figure out whether $search is actually used
|[`$search`](#search)|A property and value pair separated by a colon.|
-->

Эти параметры совместимы с [языком запросов OData версии 4][odata-query].

> **Примечание.** В конечной точке `beta` префикс `$` является необязательным. Например, вместо `$filter` можно использовать `filter`. Дополнительные сведения и примеры см. в статье [Поддержка параметров запросов без префиксов $ в Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).

**Кодирование параметров запросов.**

К значениям параметров запросов нужно применить процентное кодирование. Многие клиенты HTTP, браузеры и инструменты (например, [песочница Graph][graph-explorer]) помогут вам в этом. Если запрос неудачный, одна из возможных причин — не удалось должным образом закодировать значения параметров запросов.

URL-адрес, который не было закодирован, выглядит так:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

Закодированный должным образом URL-адрес выглядит так:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="filter"></a>filter

`$filter` можно использовать для получения только подмножества объектов коллекции. Например, чтобы найти пользователей, чье отображаемое имя начинается с `J`, используйте `startswith`.

[Попробовать в песочнице Graph](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

**Запрос:**

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

**Отклик:**

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
    "value": [
        {
            "id": "e013b9f3-a1ab-48d1-907b-e716c39d6363",
            "businessPhones": [
                "4255550100"
            ],
            "displayName": "Jan Madden",
            "givenName": "Jan",
            "jobTitle": null,
            "mail": "demo32@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": null,
            "preferredLanguage": null,
            "surname": "Madden",
            "userPrincipalName": "demo32@a830edad9050849NDA1.onmicrosoft.com"
        },
        {
            "id": "89efe8ed-d141-4151-a3e4-570a70022dff",
            "businessPhones": [
                "+1 425 555 0109"
            ],
            "displayName": "Janet Schorr",
            "givenName": "Janet",
            "jobTitle": "Product Marketing Manager",
            "mail": "janets@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": "18/2111",
            "preferredLanguage": null,
            "surname": "Schorr",
            "userPrincipalName": "janets@a830edad9050849NDA1.onmicrosoft.com"
        },
        ...
    ]
}
```

Для параметра `$filter` предусмотрен богатый синтаксис с большим количеством встроенных операторов. Логические операторы включают в себя "равно" (`eq`), "не равно" (`ne`), "больше чем" (`gt`), "больше чем или равно" (`gte`), "и" (`and`), "или" (`or`), "не" (`not`) и другие. Арифметические операторы включают в себя "добавить" (`add`), "вычесть" (`sub`) и другие. Строковые операторы включают в себя "содержит" (`contains`), "начинается с" (`startswith`) и другие. Лямбда-операторы включают в себя "любой" (`any`) и "все" (`all`). Дополнительные сведения о синтаксисе `$filter` см. в [статье о протоколе OData][odata-filter].


## <a name="select"></a>select

Чтобы задать вместо стандартного набора возвращаемых свойств другой, для коллекции или отдельного объекта используйте параметр запросов `$select`. С помощью параметра `$select` можно выбрать подмножество или супермножество стандартного набора возвращаемых свойств. Например, при получении сообщений можно задать возвращение только свойств `from` и `subject`.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<!--For example, when retrieving the children of an item on a drive, you want to select that only the `name` and `size` properties of items are returned.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name,size
```

By submitting the request with the `$select=name,size` query string, the objects
in the response will only have those property values included.

```json
{
  "value": [
    {
      "id": "13140a9sd9aba",
      "name": "Documents",
      "size": 1024
    },
    {
      "id": "123901909124a",
      "name": "Pictures",
      "size": 1012010210
    }
  ]
}
```-->

## <a name="expand"></a>expand

В запросах Microsoft Graph API пути к объекту или коллекции указанного элемента не разворачиваются автоматически. Эта особенность позволяет уменьшить сетевой трафик и время создания ответа службой. Однако в некоторых случаях эти результаты может потребоваться включить в ответ.

Чтобы API развернул дочерний объект или коллекцию и включил эти результаты, можно использовать параметр строки запроса `$expand`.

Например, с помощью параметра `$expand` можно получить сведения о корневом объекте drive и дочерних элементах верхнего уровня для объекта drive. Кроме того, в этом примере используется оператор [`$select`](#select), который возвращает только свойства `id` и `name` дочерних элементов.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> **Примечание.** Максимальное количество развернутых объектов в запросе — 20. Кроме того, запрашивая ресурс [`user`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user), можно использовать параметр `$expand`, чтобы получить свойства только одного дочернего объекта или коллекции за раз. В следующем примере возвращаются объекты `user`, каждый из которых содержит до 20 объектов `directReport` в развернутой коллекции `directReports`:

```http
GET https://graph.microsoft.com/v1.0/users?$expand=directReports
```

Другие ресурсы также могут иметь ограничения, поэтому всегда проверяйте наличие ошибок.

## <a name="orderby"></a>orderby

Чтобы указать порядок сортировки элементов, возвращаемых из API Microsof Graph, используйте параметр запросов `$orderby`.

Например, чтобы возвратить список пользователей в организации, упорядоченный по отображаемому имени, используйте следующий синтаксис:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

Вы также можете сортировать данные по объектам сложного типа. В следующем примере сообщения сортируются по полю `address` свойства `from` сложного типа `emailAddress`:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

Чтобы отсортировать результаты по возрастанию или убыванию, добавьте `asc` или `desc` к имени поля, добавив пробел для разделения, например: `?$orderby=name%20desc`.

 > **Примечание.** Запрашивая ресурс [`user`](../api-reference/v1.0/resources/user.md), параметр `$orderby` невозможно совместить с выражениями filter.

## <a name="top"></a>top

Чтобы указать максимальное количество элементов, возвращаемых в результирующем наборе, используйте параметр запросов `$top`. Параметр запросов `$top` определяет подмножество в коллекции. В это подмножество включаются первые N элементов набора, где N — положительное целое число, указанное этим параметром запросов. Например, чтобы возвратить первые пять сообщений в почтовом ящике пользователя, используйте следующий синтаксис:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

## <a name="skip"></a>skip

Чтобы задать количество элементов, которое необходимо пропустить, используйте параметр запросов `$skip`. Например, чтобы возвратить список событий, начиная с 21-го, отсортированный по дате создания, используйте указанный ниже синтаксис.

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

## <a name="skiptoken"></a>skipToken

Чтобы запросить вторую и последующие страницы данных Graph, задайте параметр запросов `$skipToken`. Он предоставляется в URL-адресах, возвращаемых Graph, когда возвращается подмножество результатов, что обычно происходит из-за подкачки на стороне сервера. Этот параметр указывает, на какой точке в коллекции сервер завершил отправку результатов, и передается обратно в Graph, чтобы указать, откуда необходимо возобновить отправку результатов. Например, значение параметра запросов `$skipToken` может определять десятый или двадцатый элемент в коллекции, содержащей 50 элементов, а также любую другую позицию в коллекции.

Некоторые отклики будут содержать значение `@odata.nextLink`, другие же — значение `$skipToken`. Значение `$skipToken` — это метка, которая сообщает службе, откуда необходимо возобновить обработку для следующего набора результатов. Ниже приведен пример значения `@odata.nextLink` из отклика, где список пользователей упорядочен по свойству `displayName`.

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27"
```

Чтобы вернуть следующую страницу списка пользователей в организации, используйте приведенный ниже синтаксис.

```http
GET  https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27
```

## <a name="count"></a>count

Используйте параметр запросов `$count`, чтобы включить общее количество элементов в коллекции вместе со страницей значений, возвращенных из Graph, как показано в следующем примере:

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

При этом возвращается коллекция `contacts`, а также количество элементов коллекции `contacts` в свойстве `@odata.count`.

>**Примечание.** Это не поддерживается для коллекций [`directoryObject`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/directoryobject).

## <a name="search"></a>search

Чтобы ограничить результаты запроса с помощью условия поиска, используйте параметр запросов `$search`.

> **Примечание.** Сейчас можно выполнять поиск **только** в коллекциях [message](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message) и [person](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/person). Запрос `$search` возвращает до 250 результатов. В поисковых запросах невозможно указать [`$filter`](#filter) или [`$orderby`](#orderby).

Условия поиска указываются с использованием расширенного синтаксиса запросов (AQS). Результаты сортируются по дате и времени отправки сообщения.

Вы можете указать следующие свойства для объекта `message` в условии `$search`: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`.

Если для поиска в сообщениях указано только значение, используются такие свойства поиска по умолчанию: `from`, `subject` и `body`.

Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово pizza в любом из трех свойств поиска по умолчанию:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

Следующий пример кода выполняет поиск всех сообщений в папке "Входящие" пользователя, отправленных с определенного электронного адреса:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
