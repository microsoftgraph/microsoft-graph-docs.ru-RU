# <a name="use-query-parameters-to-customize-responses"></a>Настройка ответов с помощью параметров запроса

В Microsoft Graph предусмотрены необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных. Поддерживаются указанные ниже параметры запросов.

>**Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].

|Имя|Описание|Пример|
|:---------------|:--------|:-------|
|[$count](#count)|Возвращает общее количество соответствующих ресурсов.|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
|[$expand](#expand)|Получает связанные ресурсы.|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)
|[$filter](#filter)|Фильтрует результаты (строки).|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[$orderby](#orderby)|Упорядочивает результаты.|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)
|[$search](#search)| Возвращает результаты на основании условий поиска. В настоящее время поддерживается в коллекциях `messages` и `person`.|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)
|[$select](#select)|Фильтрует свойства (столбцы).|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[$skip](#skip)|Применяется для индексации в результирующем наборе. Также используется некоторыми API для разбиения по страницам и может использоваться вместе с параметром `$top` для разбиения результатов по страницам вручную.  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)
|[$skipToken](#skiptoken)|Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. (Вместо этого параметра некоторые API используют `$skip`.) | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`
|[$top](#top)|Задает размер страницы результатов. |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)

Эти параметры совместимы с [языком запросов OData версии 4][odata-query]. Параметры, которые поддерживаются всеми API Microsoft Graph для конечной точки `v1.0`, могут значительно отличаться от таковых для конечной точки `beta`. 

> **Примечание.** В конечной точке `beta` префикс `$` является необязательным. Например, вместо `$filter` можно использовать `filter`. Дополнительные сведения и примеры см. в статье [Поддержка параметров запросов без префиксов $ в Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).

## <a name="encoding-query-parameters"></a>Кодирование параметров запроса

К значениям параметров запросов нужно применить процентное кодирование. Многие клиенты HTTP, браузеры и инструменты (например, [песочница Graph][graph-explorer]) помогут вам в этом. Если запрос неудачный, одна из возможных причин — не удалось должным образом закодировать значения параметров запросов.

URL-адрес, который не было закодирован, выглядит так:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

Закодированный должным образом URL-адрес выглядит так:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count"></a>count

Параметр запроса `$count` позволяет включить общее количество элементов коллекции вместе со страницей значений, возвращенных из Microsoft Graph. 

Например, следующий запрос возвращает коллекцию `contacts` текущего пользователя, а также ряд элементов коллекции `contacts` в свойстве `@odata.count`.

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


>**Примечание.** Параметр `$count` не поддерживается коллекциями ресурсов, производных от [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md), такими как коллекции [user](../api-reference/v1.0/resources/user.md) или [group](../api-reference/v1.0/resources/group.md).

## <a name="expand"></a>expand

Многие ресурсы Microsoft Graph выводят как объявленные свойства ресурса, так и его связи с другими ресурсами. Эти связи также называются свойствами ссылки или навигации и могут ссылаться как на один ресурс, так и на коллекцию ресурсов. Например, папки почты, руководитель и подчиненные пользователя выводятся как связи. 

Как правило, в одном запросе можно отдельно (но не одновременно) запросить или свойства ресурса, или одно из отношений. С помощью строкового параметра запроса `$expand` в результаты можно включить расширенный ресурс или коллекцию, на которые ссылается одно отношение (свойство навигации).

В приведенном ниже примере возвращаются сведения о корневом каталоге, а также дочерние элементы верхнего уровня на диске.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

Кроме того, некоторые коллекции ресурсов позволяют указывать свойства, которые должны быть возвращены в расширенных ресурсах, с помощью параметра `$select`. В следующем примере выполняется то же запрос, что и в предыдущем, но используется оператор [`$select`](#select), с помощью которого для расширенных дочерних элементов возвращаются только свойства `id` и `name`.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)

> **Примечание.** Не все отношения и ресурсы поддерживают параметр запроса `$expand`. Например, можно расширить отношения пользователя `directReports`, `manager` и `memberOf`, но не отношения `events`, `messages` или `photo`. Не все ресурсы и отношения поддерживают использование параметра `$select` для расширенных элементов. 
> 
> Ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), поддерживают параметр `$expand` только в `beta`, и обычно он возвращает не более 20 элементов расширенных отношений.

## <a name="filter"></a>filter

Параметр запроса `$filter` позволяет получить только подмножество объектов коллекции. 

Например, чтобы найти пользователей, чье отображаемое имя начинается с буквы J, используйте `startswith`.

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

Поддержка операторов `$filter` зависит от того, какой API Microsoft Graph используется. В большинстве случаев поддерживаются следующие операторы: 

- `eq` (равняется);
- `ne` (не равняется);
- `gt` (больше чем);
- `ge` (не меньше чем);
- `lt` (меньше чем), `le` (не больше чем);
- `and` (и);
- `or` (или);
- `not` (не).
 
Часто поддерживается строковый оператор `startswith`. Некоторые API поддерживают лямбда-оператор `any`. Примеры использования см. в приведенной ниже таблице. Дополнительные сведения о синтаксисе `$filter` см. в [статье о протоколе OData][odata-filter].  

Приведенная ниже таблица содержит несколько примеров использования параметра запроса `$filter`.

>**Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].

|Описание|Пример|
|:--------|:-------|
|  Поиск пользователей с именем Mary по нескольким свойствам. | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| Получение всех событий для вошедшего пользователя, которые начинаются после 01.07.2017 г. | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| Получение всех сообщений с определенного адреса, полученных вошедшим пользователем. | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| Получение всех сообщений, полученных вошедшим пользователем в апреле 2017 г. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| Получение всех непрочитанных сообщений в папке "Входящие" вошедшего пользователя. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| Получение списка всех групп Office 365 в организации. | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> **Примечание.** Ресурсы Azure AD не поддерживают следующие операторы `$filter`: `ne`, `gt`, `ge`, `lt`, `le` и `not`. В настоящее время строковый оператор `contains` не поддерживается ни одним ресурсом Microsoft Graph.

## <a name="orderby"></a>orderby

Параметр запроса `$orderby` позволяет указать порядок сортировки элементов, возвращаемых из Microsoft Graph.

Например, следующий запрос возвращает список пользователей в организации, упорядоченный по отображаемому имени:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

Вы также можете сортировать данные по объектам сложного типа. В следующем запросе сообщения сортируются по полю `address` свойства `from` сложного типа `emailAddress`:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

Чтобы отсортировать результаты по возрастанию или убыванию, добавьте `asc` или `desc` к имени поля, используя пробел для разделения, например: `?$orderby=name%20desc`.

Некоторые API позволяют упорядочивать результаты по нескольким свойствам. Например, приведенный ниже запрос позволяет упорядочить сообщения в папке "Входящие" пользователя сначала по имени отправителей по убыванию (от Я до А), а затем — по возрастанию (по умолчанию).

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > **Примечание.** Ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), не позволяют объединять параметр `$orderby` с выражениями `$filter`. 

## <a name="search"></a>поиск

Параметр запроса `$search` позволяет ограничить результаты запроса с помощью условия поиска.

> **Примечание.** Сейчас можно выполнять поиск **только** в коллекциях [message](../api-reference/v1.0/resources/message.md) и [person](../api-reference/v1.0/resources/person.md). Запрос `$search` возвращает до 250 результатов. В поисковых запросах невозможно указать [`$filter`](#filter) или [`$orderby`](#orderby).

### <a name="using-search-on-message-collections"></a>Использование параметра $search в коллекциях `message`

Условия поиска сообщений указываются с использованием [расширенного синтаксиса запросов (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7). Результаты сортируются по дате и времени отправки сообщения.

Вы можете указать следующие свойства для объекта `message` в условии `$search`:

- `attachments`
- `bccRecipients`
- `body`
- `category`
- `ccRecipients`
- `content`
- `from`
- `hasAttachments`
- `participants`
- `receivedDateTime`
- `sender`
- `subject`
- `toRecipients`

Если для поиска в сообщениях указано только значение, используются такие свойства поиска по умолчанию: `from`, `subject` и `body`.

Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово pizza в любом из трех свойств поиска по умолчанию:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

Следующий пример кода выполняет поиск всех сообщений в папке "Входящие" пользователя, отправленных с определенного электронного адреса: 

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

### <a name="using-search-on-person-collections"></a>Использование параметра $search в коллекциях `person`

API People Microsoft Graph можно использовать для получения сведений о наиболее релевантных для пользователя людях. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. API People поддерживает параметр запроса `$search`.

Поиск людей выполняется по свойствам `displayName` и `emailAddress` ресурса [person](../api-reference/v1.0/resources/person.md). В поиске применяется алгоритм нечетких соответствий. Возвращаются результаты, основанные на точном совпадении, а также на выводы, связанные с целью поиска. Предположим, в коллекции `people` вошедшего в систему пользователя есть пользователь с отображаемым именем Tyler Lee и электронным адресом tylerle@example.com. Во всех приведенных ниже примерах поиск возвращает результаты, содержащие имя Tyler.

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

Можно также выполнить поиск людей, которым интересна определенная тема. Поиск выполняется на основе заключений, выведенных из переписки пользователя по электронной почте. Например, приведенный ниже поиск возвращает список людей, релевантных для вошедшего в систему пользователя, которые в беседах с ним интересовались пиццей. Обратите внимание, что фраза для поиска заключена в кавычки.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

И, наконец, в одном запросе можно объединить поиск людей и тем, используя вместе два вида выражений поиска.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
В этом запросе фактически выполняется два поиска: нечеткий поиск по свойствам `displayName` и `emailAddress` людей, релевантных для вошедшего пользователя, и поиск по теме "pizza" в отношении этих людей. Результаты ранжируются, упорядочиваются и возвращаются. Обратите внимание, что поиск не имеет ограничений, поэтому результаты могут содержать список пользователей с нечетким соответствием имени "tyl" или пользователей, интересующихся темой "pizza", или и тех, и других.

Дополнительные сведения об API поиска людей см. в статье [Получение сведений о релевантных людях](./people_example.md).  

## <a name="select"></a>select

Параметр запроса `$select` позволяет возвратить набор свойств, отличный от набора по умолчанию, для отдельного ресурса или коллекции ресурсов. С помощью параметра $select можно указать подмножество или супермножество свойств по умолчанию.

Например, при получении сообщений вошедшего пользователя можно указать, что необходимо вернуть только свойства `from` и `subject`:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> **Важно!** Как правило, параметр `$select` рекомендуется использовать, чтобы запрос возвращал только те свойства, которые необходимы вашему приложению. Это особенно касается запросов, которые могут возвращать большой результирующий набор. Ограничение набора свойств, возвращаемых в каждой строке, позволяет уменьшить сетевую нагрузку и повысить производительность вашего приложения.
>
> В `v1.0` некоторые ресурсы Azure AD, производные от [directoryObject](../api-reference/v1.0/resources/directoryobject.md), такие как [user](../api-reference/v1.0/resources/user.md) и [group](../api-reference/v1.0/resources/group.md), возвращают при чтении ограниченное подмножество свойств по умолчанию. С этими ресурсами параметр `$select` необходимо использовать для возврата свойств, не входящих в набор по умолчанию.  

## <a name="skip"></a>skip

Параметр запроса `$skip` позволяет задать количество элементов, которое необходимо пропустить в начале коллекции. Например, следующий запрос возвращает события пользователя, отсортированные по дате создания, начиная с 21-го события в коллекции:

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> **Примечание.** Некоторые API Microsoft Graph, например для почты и календарей Outlook (`message`, `event`, `calendar`), используют `$skip` для разбиения по страницам. Если результаты запроса занимают несколько страниц, эти API возвращают свойство `@odata:nextLink` с URL-адресом, содержащим параметр `$skip`. Этот URL-адрес можно использовать для возврата следующей страницы результатов. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).

## <a name="skiptoken"></a>skipToken

Некоторые запросы возвращают несколько страниц данных. Это происходит из-за разбиения по страницам на стороне сервера или из-за использования параметра [`$top`](#top), который ограничивает размер возвращаемых страниц. Многие API Microsoft Graph используют параметр запроса `skipToken` для ссылки на следующие страницы результатов. Параметр `$skiptoken` содержит непрозрачный маркер, который ссылается на следующую страницу результатов и возвращается в URL-адресе, указанном в свойстве `@odata.nextLink`. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).


## <a name="top"></a>top

Параметр запроса `$top` позволяет задать размер страницы в результирующем наборе. 

Если результирующий набор будет содержать больше одной страницы элементов, тело отклика будет содержать параметр `@odata.nextLink`. Этот параметр содержит URL-адрес, с помощью которого можно получить следующую страницу результатов. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md). 

Например, следующий запрос возвращает первые пять сообщений в почтовом ящике пользователя:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a>Обработка ошибок параметров запроса

Некоторые запросы возвращают сообщение об ошибке, если указанный параметр запроса не поддерживается. Например, невозможно использовать `$expand` для связи `user/photo`. 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

При этом необходимо отметить, что указанные в запросе параметры могут просто не сработать. Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание. В таких случаях необходимо проверить возвращенные запросом данные и определить, дали ли указанные параметры запроса желаемый результат. 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356