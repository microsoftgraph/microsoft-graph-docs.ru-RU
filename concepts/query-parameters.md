---
title: Настройка ответов с помощью параметров запроса
description: В Microsoft Graph предусмотрены необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 51bf43360c3580011ab39e2c385b4c23d3bfc5a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962415"
---
# <a name="use-query-parameters-to-customize-responses"></a>Настройка ответов с помощью параметров запроса

В Microsoft Graph поддерживаются необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных. Поддержка определенных параметров запросов варьируется для разных операций API и в зависимости от API может отличаться в конечных точках версии 1.0 и бета-версии. 

> [!TIP] 
> В конечной точке бета-версии префикс `$` является необязательным. Например, вместо `$filter` можно использовать `filter`. В конечной точке версии 1 префикс `$` является необязательным только для подмножества API-интерфейсов. Для простоты всегда включайте `$`, если используется конечная точка версии 1.

Параметрами запроса могут быть системные параметры запроса OData или другие параметры запроса. 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a>Системные параметры запроса OData
API Microsoft Graph может поддерживать один или несколько из указанных ниже системных параметров запроса OData. Эти параметры запроса совместимы с [языком запросов OData версии 4][odata-query].

>**Примечание.** OData 4.0 поддерживает системные параметры запросов только в операциях GET.

Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].

| Имя                     | Описание | Пример
|:-------------------------|:------------|:---------|
| [$count](#count-parameter)         | Возвращает общее количество соответствующих ресурсов. | [`/me/messages?$top=2&$count=true`][count-example]
| [$expand](#expand-parameter)       | Получает связанные ресурсы.|[`/groups?$expand=members`][expand-example]
| [$filter](#filter-parameter)       | Фильтрует результаты (строки).|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [$format](#format-parameter)       | Возвращает результаты в указанном формате мультимедиа.|[`/users?$format=json`][format-example]
| [$orderby](#orderby-parameter)     | Упорядочивает результаты.|[`/users?$orderby=displayName desc`][orderby-example]
| [$search](#search-parameter)       | Возвращает результаты на основании условий поиска. |[`/me/messages?$search=pizza`][search-example]
| [$select](#select-parameter)       | Фильтрует свойства (столбцы).|[`/users?$select=givenName,surname`][select-example]
| [$skip](#skip-parameter)           | Применяется для индексации в результирующем наборе. Также используется некоторыми API для разбиения по страницам и может использоваться вместе с параметром `$top` для разбиения результатов по страницам вручную. | [`/me/messages?$skip=11`][skip-example]
| [$top](#top-parameter)             | Задает размер страницы результатов. |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a>Другие параметры запроса

| Имя                     | Описание | Пример
|:-------------------------|:------------|:---------|
| [$skipToken](#skiptoken-parameter) | Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. (Вместо этого параметра некоторые API используют `$skip`.) | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a>Другие возможности URL-адресов OData

Следующие возможности OData 4.0 являются сегментами URL-адресов, а не параметрами запросов.

| Имя                     | Описание | Пример 
|:-------------------------|:------------|:---------|
| [$ref](/graph/api/group-post-members) | Обновляет принадлежность объектов к коллекции. | `POST /groups/{id}/members/$ref` |
| [$value](/graph/api/profilephoto-get) | Возвращает или обновляет двоичное значение элемента. | `GET /me/photo/$value` |

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

### <a name="escaping-single-quotes"></a>Пропуск одинарных кавычек

В запросах, использующих одинарные кавычки, если любой параметр также содержит одинарные кавычки, их нужно пропустить дважды; в противном случае запрос завершится сбоем из-за недопустимого синтаксиса. В приведенном примере строковое значение `let''s meet for lunch?` содержит пропускаемую одинарную кавычку.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a>Параметр count

Параметр запроса `$count` позволяет включить общее количество элементов коллекции вместе со страницей значений, возвращенных из Microsoft Graph. 

Например, приведенный ниже запрос возвращает коллекцию **contact** текущего пользователя, а также ряд элементов коллекции **contact** в свойстве `@odata.count`.

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


Параметр запроса `$count` поддерживается для таких коллекций ресурсов и их отношений, которые являются производными от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true)
- [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
- [orgContact](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
- [device](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
- [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
- [users](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).

## <a name="expand-parameter"></a>Параметр expand

Многие ресурсы Microsoft Graph возвращают как объявленные свойства ресурса, так и его связи с другими ресурсами. Эти связи также называются свойствами ссылки или навигации и могут ссылаться как на один ресурс, так и на коллекцию ресурсов. Например, папки почты, руководитель и подчиненные пользователя выводятся как связи. 

Как правило, в одном запросе можно отдельно (но не одновременно) запросить или свойства ресурса, или одно из отношений. С помощью строкового параметра запроса `$expand` в результаты можно включить расширенный ресурс или коллекцию, на которые ссылается одно отношение (свойство навигации).

В приведенном ниже примере возвращаются сведения о корневом каталоге, а также дочерние элементы верхнего уровня на диске.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

Кроме того, некоторые коллекции ресурсов позволяют указывать свойства, которые должны быть возвращены в расширенных ресурсах, благодаря параметру `$select`. В следующем примере выполняется тот же запрос, что и в предыдущем, но используется оператор [`$select`](#select-parameter), с помощью которого для расширенных дочерних элементов возвращаются только свойства **id** и **name**.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[Попробовать в песочнице Graph][expand-example]

> **Примечание.** Не все связи и ресурсы поддерживают параметр запроса `$expand`. Например, можно расширить связи пользователя **directReports**, **manager** и **memberOf**, но не связи **events**, **messages** или **photo**. Не все ресурсы и связи поддерживают использование параметра `$select` для расширенных элементов. 
> 
> Ресурсы Azure AD, производные от [directoryObject](/graph/api/resources/directoryobject), такие как [user](/graph/api/resources/user) и [group](/graph/api/resources/group), поддерживают параметр `$expand` только в `beta`, и обычно он возвращает не более 20 элементов расширенных отношений.

## <a name="filter-parameter"></a>Параметр filter

Параметр запроса `$filter` позволяет получить только подмножество объектов коллекции. Параметр запроса `$filter` также используется для извлечения таких отношений, как members, memberOf, transitiveMembers и transitiveMemberOf. Например, получите все группы безопасности, участником которых являетесь.

Также чтобы найти пользователей, чье отображаемое имя начинается с буквы J, используйте `startsWith`.

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

[Попробовать в песочнице Graph][filter-example]

Поддержка операторов `$filter` зависит от того, какой API Microsoft Graph используется. В большинстве случаев поддерживаются следующие операторы:

- равно `eq` / не равно `ne`
- меньше `lt` / больше `gt`
- меньше или равно `le` / больше или равно `ge`
- и `and` / или `or`
- в `in`
- Отрицание `not`
- лямбда-оператор "любой" `any`
- лямбда-оператор "все" `all`
- Начинается с `startsWith`
- Заканчивается на `endsWith`

> **Примечание.** Поддержка этих операторов зависит от сущности. Дополнительные сведения см. в документации по конкретным сущностям. 
>
> В настоящее время строковый оператор `contains` не поддерживается ни одним ресурсом Microsoft Graph.

Примеры использования см. в приведенной ниже таблице. Дополнительные сведения о синтаксисе `$filter` см. в [статье о протоколе OData][odata-filter].  
Приведенная ниже таблица содержит несколько примеров использования параметра запроса `$filter`.

> **Примечание.** Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].

| Описание | Пример
|:------------|:--------|
| Получение всех пользователей с именем Маша по нескольким свойствам. | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| Получение всех пользователей с почтовым доменом "hotmail.com" | [`https://graph.microsoft.com/v1.0/users?$count=true&$filter=endsWith(mail,'@hotmail.com')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| Получение всех событий для вошедшего пользователя, которые начинаются после 01.07.2017 г. | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| Получение всех сообщений с определенного адреса, полученных вошедшим пользователем. | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| Получение всех сообщений, полученных вошедшим пользователем в апреле 2017 г. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| Получение всех непрочитанных сообщений в папке "Входящие" вошедшего пользователя. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| Получение списка всех групп Microsoft 365 в организации. | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |
| Используйте преобразование OData, чтобы получить транзитивное членство в группах с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов. | [`https://graph.microsoft.com/beta/me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`](https://developer.microsoft.com/graph/graph-explorer?request=me/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName,'a')&method=GET&version=v1.0) |

## <a name="format-parameter"></a>Параметр format

Параметр запроса `$format` позволяет указать формат мультимедиа для элементов, возвращаемых из Microsoft Graph.

Например, указанный ниже запрос возвращает список пользователей организации в формате JSON.

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

[Попробовать в песочнице Graph][format-example]

> **Примечание.** Параметр запросов `$format` поддерживает ряд форматов (например, Atom, XML и JSON), но результаты могут не возвращаться во всех форматах.

## <a name="orderby-parameter"></a>Параметр orderby

Параметр запроса `$orderby` позволяет указать порядок сортировки элементов, возвращаемых из Microsoft Graph.

Например, следующий запрос возвращает список пользователей в организации, упорядоченный по отображаемому имени:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[Попробовать в песочнице Graph][orderby-example]

Вы также можете сортировать данные по объектам сложного типа. Приведенный ниже запрос позволяет получить сообщения и отсортировать их по полю **address** свойства **from**, принадлежащего к сложному типу **emailAddress**.

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

> **Примечание.** Если вы укажете $filter, сервер определит порядок сортировки результатов. Если вы одновременно используете `$orderby` и `$filter` для получения сообщений, так как сервер всегда определяет порядок сортировки результатов `$filter`, [необходимо задать свойства определенным образом](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).


В приведенном ниже примере показан запрос, отфильтрованный по свойствам **subject** и **importance**, а затем отсортированный по свойствам **subject**, **importance** и **receivedDateTime** в порядке убывания.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[Попробовать в песочнице Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

> **Примечание.** Сочетание параметров запросов `$orderby` и `$filter` поддерживается в бета-версии конечной точки для следующих ресурсов AD и их связей, полученных из [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):
>
>- [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
>- [orgContact](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
>- [device](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
>- [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
>- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
>- [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
>
> Чтобы использовать вместе `$orderby` и `$filter` (или `$filter` и `endsWith`), вам требуется:
>
> - Добавить `$count=true` в параметры запроса
> - Добавить заголовок запроса `ConsistencyLevel: eventual`
>
> Дополнительные сведения см. в разделе [необязательных пользовательских параметров запросов](/graph/api/user-list?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

## <a name="search-parameter"></a>Параметр search

Параметр запроса `$search` позволяет ограничить результаты запроса с помощью условия поиска.

### <a name="using-search-on-message-collections"></a>Использование параметра $search в коллекциях message

Можно искать сообщения, основываясь на их конкретных свойствах. Результаты поиска сортируются по дате и времени отправки сообщения. Запрос `$search` возвращает до 250 результатов.

Если при поиске сообщений указано только значение, а конкретные свойства не заданы, поиск выполняется по свойствам поиска по умолчанию: **from**, **subject** и **body**.

Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово "pizza" в любом из трех свойств поиска по умолчанию:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

[Попробовать в песочнице Graph][search-example]

Кроме того, для поиска сообщений можно указать в таблице ниже их имена свойств, распознаваемые синтаксисом языка запросов по ключевым словам (KQL). Эти имена свойств соответствуют свойствам, определенным в сущности **message** в Microsoft Graph. Синтаксис KQL поддерживается в Outlook и других приложениях Microsoft 365, например SharePoint. Благодаря этому возможно использование общего домена обнаружения для соответствующих хранилищ данных.


| Свойство электронных писем, по которому можно выполнять поиск                | Описание | Пример 
|:-------------------------|:------------|:---------|
| **attachment**           | Имена файлов, вложенных в сообщение электронной почты.|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| **bcc**           | Поле **Скрытая копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| **body**           | Текст сообщения электронной почты.|[`me/messages?$search="body:excitement"`][search-body-example]
| **cc**           | Поле **Копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| **from**           | Отправитель сообщения электронной почты, на которого указывает SMTP-адрес, отображаемое имя или псевдоним.|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| **hasAttachment** | Значение TRUE означает, что сообщение электронной почты содержит вложение, не являющееся встроенным. В противном случае задается значение FALSE. |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| **importance**           | Важность сообщения, которую отправитель может указать при отправке. Возможные значения — `low`, `medium` и `high`.|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| **kind**           | Тип сообщения. Допустимые значения — `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` и `voicemail`.|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| **participants**           | Такие поля сообщения электронной почты, как **От**, **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.|[`me/messages?$search="participants:danas"`][search-part-example]
| **received**           | Дата получения сообщения адресатом.|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| **recipients**           | Такие поля сообщения электронной почты, как **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| **sent**           | Дата отправки сообщения отправителем.|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| **size**           | Размер элемента в байтах.|[`me/messages?$search="size:1..500000"`][search-size-example]
| **subject**           | Текст в строке темы сообщения электронной почты. .|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| **to**           | Поле **Кому** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


Дополнительные сведения о доступных для поиска свойствах, синтаксисе KQL, поддерживаемых операторах и подсказках для поиска вы найдете в таких статьях:

- [Свойства, доступные для поиска в Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)

- [Руководство по синтаксису языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [Свойства сообщений и операторы поиска для обнаружения электронных данных на месте в Exchange 2016](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators).

### <a name="using-search-on-person-collections"></a>Использование параметра $search в коллекциях person

API People Microsoft Graph можно использовать для получения сведений о наиболее релевантных для пользователя людях. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. API People поддерживает параметр запроса `$search`. Запрос `$search` возвращает до 250 результатов.

Поиск людей выполняется по свойствам **displayName** и **emailAddress** ресурса [person](/graph/api/resources/person).

По приведенному ниже запросу выполняется поиск человека с именем Irene McGowen в свойствах **displayName** и **emailAddress** всех людей из коллекции **people** вошедшего пользователя. Так как человек с именем Irene McGowan является релевантным для вошедшего пользователя, возвращается информация о нем.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

Ниже показан пример ответа. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

Дополнительные сведения об API поиска людей см. в [этой статье](./people-example.md#search-people).  

### <a name="using-search-on-directory-object-collections"></a>Использование $search в коллекциях объектов каталога

Вы можете использовать параметр запроса `$search`, чтобы отфильтровать результаты с помощью разметки. Поиск с разметкой выполняется путем извлечения слов из входной и выходной строки, использования пробелов, разного регистра и символов для разделения слов, как показано ниже.

* **Пробелы**: `hello world` => `hello`, `world`
* **Разный регистр**⁽¹⁾: `HelloWorld` или `helloWORLD` => `hello`, `world`
* **Символы**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`
* **Числа**: `hello123world` => `hello`, `123`, `world`

⁽¹⁾ В настоящее время разметка работает только в том случае, когда регистр изменяется с нижнего на верхний, поэтому `HELLOworld` считается одним маркером: `helloworld`, а `HelloWORld` — двумя маркерами: `hello`, `world`. ⁽²⁾ Логика разметки также объединяет слова, разделенные только символами, например поиск по запросу `helloworld` выдаст результаты `hello-world` и `hello.world`.

> **Примечание**. После разметки маркеры сопоставляются независимо от исходного регистра, и они сопоставляются в любом порядке.
> Параметр запроса `$search` в коллекции объектов каталога **требует** специального заголовка запроса: `ConsistencyLevel: eventual`.

Поддержка поиска с разметкой работает только в полях **displayName** и **description**. Любое поле можно поместить в `$search`, поля, отличные от **displayName** и **description** по умолчанию представляют собой поведение `$filter` "startswith". Например:

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

В результате будут выводиться все группы с именами типа "OneVideo". `$search` можно использовать вместе с `$filter`. Пример:

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

В результате будут выводиться все группы с включенной поддержкой почты с именами типа "OneVideo". Результаты ограничены на основе логического соединения `$filter` ("И") и всего запроса в `$search`. Искомый текст маркируется с учетом регистра, но совпадения выполняются без его учета. Например, "OneVideo" разбивается на два маркера ввода "one" и "video", но не учитывает регистр.

В синтаксисе поиска применяются следующие правила:

* Универсальный формат: $search="clause1" \[И \| ИЛИ\] "\[clauseX\]"\.
* Поддерживается любое количество предложений. Также поддерживаются круглые скобки для приоритета.
* Синтаксис каждого предложения — "\<property>:\<text to search>".
* Имя свойства должно быть указано в предложении. Любое свойство, которое можно использовать в `$filter`, можно также использовать в `$search`. В зависимости от свойства поведение поиска является либо "search", либо "startswith", если поиск не поддерживается в свойстве.
* Вся часть предложения должна быть заключена в двойные кавычки.
* Логический оператор "И" "ИЛИ" не должен быть в двойных кавычках. Они должны быть прописными.
* Учитывая, что вся часть предложения должна быть помещена в двойные кавычки, если она содержит двойные кавычки и обратную косую черту, ее необходимо экранировать с помощью обратной косой черты. Другие символы не требуются экранировать.

В таблице ниже приведено несколько примеров.

| Класс объекта | Описание | Пример |
| ------------ | ----------- | ------- |
| Пользователь | Отображаемое имя пользователя из адресной книги. | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr"` |
| Пользователь | Отображаемое имя пользователя или электронная почта из адресной книги. | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"` |
| Группа | Отображаемое имя пользователя или описание из адресной книги. | `https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")` |
| Группа | Отображаемое имя адресной книги в группе с поддержкой почты. | `https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |

Строки ввода, указанные в `$search`, а также свойства для поиска, разделяются на части с помощью пробелов, различных регистров и типов символов (чисел и специальных символов).

## <a name="select-parameter"></a>Параметр select

Параметр запроса `$select` позволяет возвратить набор свойств, отличный от набора по умолчанию, для отдельного ресурса или коллекции ресурсов. С помощью параметра $select можно указать подмножество или супермножество свойств по умолчанию.

Например, при получении сообщений вошедшего пользователя можно указать, что необходимо вернуть только свойства **from** и **subject**:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[Попробовать в песочнице Graph][select-example]

> **Важно!** Как правило, параметр `$select` рекомендуется использовать, чтобы запрос возвращал только те свойства, которые необходимы вашему приложению. Это особенно касается запросов, которые могут возвращать большой результирующий набор. Ограничение набора свойств, возвращаемых в каждой строке, позволяет уменьшить сетевую нагрузку и повысить производительность вашего приложения.
>
> В `v1.0` некоторые ресурсы Azure AD, производные от [directoryObject](/graph/api/resources/directoryobject), такие как [user](/graph/api/resources/user) и [group](/graph/api/resources/group), возвращают при чтении ограниченное подмножество свойств по умолчанию. С этими ресурсами параметр `$select` необходимо использовать для возврата свойств, не входящих в набор по умолчанию.  

## <a name="skip-parameter"></a>Параметр skip

Параметр запроса `$skip` позволяет задать количество элементов, которое необходимо пропустить в начале коллекции. Например, следующий запрос возвращает события пользователя, отсортированные по дате создания, начиная с 21-го события в коллекции:

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[Попробовать в песочнице Graph][skip-example]

> **Примечание.** Некоторые API Microsoft Graph, например для почты и календарей Outlook (**message**, **event** и **calendar**), используют `$skip` для разбиения по страницам. Если результаты запроса занимают несколько страниц, эти API возвращают свойство `@odata:nextLink` с URL-адресом, содержащим параметр `$skip`. Этот URL-адрес можно использовать для возврата следующей страницы результатов. [Подробнее…](./paging.md)

## <a name="skiptoken-parameter"></a>Параметр skipToken

Некоторые запросы возвращают несколько страниц данных. Это происходит из-за разбиения по страницам на стороне сервера или из-за использования параметра [`$top`](#top-parameter) для ограничения размера возвращаемых страниц. Многие API Microsoft Graph используют параметр запроса `skipToken` для ссылки на следующие страницы результатов.  
Параметр `$skiptoken` содержит непрозрачный маркер, который ссылается на следующую страницу результатов и возвращается в URL-адресе, указанном в свойстве `@odata.nextLink` отклика. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).
> **Примечание.** Если вы используете счетчик OData (путем добавления `$count=true` в строку запроса), свойство `@odata.count` будет представлено только на первой странице.

## <a name="top-parameter"></a>Параметр top

Параметр запроса `$top` позволяет задать размер страницы в результирующем наборе. 

Если результирующий набор будет содержать больше одной страницы элементов, тело отклика будет содержать параметр `@odata.nextLink`. Этот параметр содержит URL-адрес, с помощью которого можно получить следующую страницу результатов. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md). 

Минимальное значение $top является 1, а максимальное зависит от соответствующего API.  

Например, следующий запрос [сообщений списка](/graph/api/user-list-messages) возвращает первые пять сообщений в почтовом ящике пользователя:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[Попробовать в песочнице Graph][top-example]


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
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0



## <a name="see-also"></a>См. также

- [Ограничения параметров запроса](known-issues.md#query-parameter-limitations)
