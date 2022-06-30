---
title: Настройка ответов с помощью параметров запроса
description: В Microsoft Graph предусмотрены необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных. Включает в себя общие параметры.
author: mumbi-o
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 5902ece88a3174cc93f30859b15bbf57e31efb78
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555970"
---
# <a name="use-query-parameters-to-customize-responses"></a>Настройка ответов с помощью параметров запроса

В Microsoft Graph поддерживаются необязательные параметры запросов, с помощью которых можно указывать и регулировать объем возвращаемых данных. Поддержка определенных параметров запросов варьируется для разных операций API и в зависимости от API может отличаться в конечных точках версии 1.0 и бета-версии.

> [!TIP] 
> В конечной точке бета-версии префикс `$` является необязательным. Например, вместо `$filter` можно использовать `filter`. В конечной точке версии 1 префикс `$` является необязательным только для подмножества API-интерфейсов. Для простоты всегда включайте `$`, если используется конечная точка версии 1.

Параметрами запроса могут быть [системные параметры запроса OData](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part2-url-conventions.html#_Toc31360955) или другие параметры запроса.

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

> [!NOTE]
> [RFC 3986](https://www.rfc-editor.org/rfc/rfc3986#section-2.2) требует, чтобы зарезервированные символы кодировались в процентах в URL-адресах. Однако этот документ может не отображать символы, закодированные в процентах, для удобочитаемости. Тем не менее зарезервированные символы, такие как запятая (`,`) в выражении `startsWith`, должны быть закодированы в запросах в процентах.

## <a name="odata-system-query-options"></a>Системные параметры запроса OData
API Microsoft Graph может поддерживать один или несколько из указанных ниже системных параметров запроса OData. Эти параметры запроса совместимы с [языком запросов OData версии 4][odata-query].

> [!NOTE]
> OData 4.0 поддерживает параметры системного запроса только в операциях GET.

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

Чтобы узнать параметры запроса системы OData, поддерживаемые API и его свойствами, см. таблицу **Свойства** на странице ресурса и раздел **Параметры необязательных запросов** для операций LIST и GET для API.

## <a name="other-query-parameters"></a>Другие параметры запроса

| Имя                     | Описание | Пример
|:-------------------------|:------------|:---------|
| [$skipToken](#skiptoken-parameter) | Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. (Вместо этого параметра некоторые API используют `$skip`.) | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a>Другие возможности URL-адресов OData

Следующие возможности OData 4.0 являются сегментами URL-адресов, а не параметрами запросов.

| Имя                     | Описание | Пример 
|:-------------------------|:------------|:---------|
| [$count](/graph/api/user-list#example-3-get-only-a-count-of-users)| Получает целочисленную сумму коллекции. | `GET /users/$count` <br> `GET /groups/{id}/members/$count`|
| [$ref](/graph/api/group-post-members) | Обновляет принадлежность объектов к коллекции. | `POST /groups/{id}/members/$ref` |
| [$value](/graph/api/profilephoto-get) | Возвращает или обновляет двоичное значение элемента. | `GET /me/photo/$value` |
| [$batch](/graph/json-batching) | Объединение нескольких HTTP-запросов в пакетный запрос. | `POST /$batch` |

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

### <a name="escaping-single-quotes"></a>Экранирование одинарных кавычек

В запросах, использующих одинарные кавычки, если любой параметр также содержит одинарные кавычки, их нужно экранировать дважды; в противном случае запрос завершится сбоем из-за недопустимого синтаксиса. В приведенном примере строковое значение `let''s meet for lunch?` содержит экранированную одинарную кавычку.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a>Параметр count

Используйте параметр `$count` запроса, чтобы получить общее количество элементов в коллекции или совпадение с выражением. `$count` можно использовать следующими способами:

1. В качестве параметра строки запроса с синтаксисом `$count=true` включить общее количество элементов в коллекции вместе со страницей значений данных, возвращаемой из Microsoft Graph. Например, `users?$count=true`.
2. В качестве [сегмента URL-адреса](#other-odata-url-capabilities) можно получить только целочисленную сумму коллекции. Например, `users/$count`.
3. В `$filter` выражении с операторами равенства для получения коллекции данных, где отфильтрованное свойство является пустой коллекцией. См [ примеры ниже](#examples-using-the-filter-query-operator).

> [!NOTE]
> 1. Для ресурсов, производных от [directoryObject](/graph/api/resources/directoryobject), `$count` это поддерживается только в расширенных запросах. См. [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).
> 2. Использование `$count` не поддерживается в клиентах Azure AD B2C.

Например, приведенный ниже запрос возвращает коллекцию **contact** текущего пользователя, а также ряд элементов коллекции **contact** в свойстве `@odata.count`.

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

Параметр запроса `$count` поддерживается для коллекций ресурсов и их связей, производных от [directoryObject](/graph/api/resources/directoryobject), причем только в [расширенных запросах](/graph/aad-advanced-queries):
- [administrativeUnit](/graph/api/resources/administrativeunit)
- [application](/graph/api/resources/application)
- [orgContact](/graph/api/resources/orgcontact)
- [device](/graph/api/resources/device)
- [group](/graph/api/resources/group)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [user](/graph/api/resources/user)

## <a name="expand-parameter"></a>Параметр expand

Многие ресурсы Microsoft Graph возвращают как объявленные свойства ресурса, так и его связи с другими ресурсами. Эти связи также называются свойствами ссылки или навигации и могут ссылаться как на один ресурс, так и на коллекцию ресурсов. Например, папки почты, руководитель и подчиненные пользователя выводятся как связи. 

Как правило, в одном запросе можно отдельно (но не одновременно) запросить или свойства ресурса, или одну из связей. С помощью строкового параметра запроса `$expand` в результаты можно включить расширенный ресурс или коллекцию, на которые ссылается одна связь (свойство навигации). В одном запросе можно расширить только одну связь.

В приведенном ниже примере возвращаются сведения о корневом каталоге, а также дочерние элементы верхнего уровня на диске.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```


Кроме того, некоторые коллекции ресурсов позволяют указывать свойства, которые должны быть возвращены в расширенных ресурсах, благодаря параметру `$select`. В следующем примере выполняется тот же запрос, что и в предыдущем, но используется оператор [`$select`](#select-parameter), с помощью которого для расширенных дочерних элементов возвращаются только свойства **id** и **name**.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> [!NOTE]
> + Не все связи и ресурсы поддерживают параметр запроса `$expand`. Например, можно расширить связи пользователя **directReports**, **manager** и **memberOf**, но не связи **events**, **messages** или **photo**. Не все ресурсы и связи поддерживают использование параметра `$select` для расширенных элементов. 
> 
> + С ресурсами Azure AD, производными от [directoryObject](/graph/api/resources/directoryobject), такими как [user](/graph/api/resources/user) и [group](/graph/api/resources/group), `$expand` обычно возвращает не более 20 элементов для расширенных связей и не содержит [@odata.nextLink](./paging.md). См. другие [известные проблемы](known-issues.md#query-parameters).
>
> + `$expand` в настоящее время не поддерживается в [расширенных запросах](/graph/aad-advanced-queries).

## <a name="filter-parameter"></a>Параметр filter

Параметр запроса `$filter` позволяет получить только подмножество объектов коллекции. Параметр запроса `$filter` также используется для извлечения таких связей, как members, memberOf, transitiveMembers и transitiveMemberOf. Например, получите все группы безопасности, участником которых являетесь.

В следующем примере выполняется поиск пользователей, чье отображаемое имя начинается с буквы J.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

Поддержка операторов `$filter` зависит от того, какой API Microsoft Graph используется. В большинстве случаев поддерживаются следующие операторы:

| Тип оператора | Оператор |
| --- | --- |
| Операторы равенства | <ul><li> Равно (`eq`) </li><li> Не равно (`ne`)</li><li> Логическое отрицание (`not`)</li><li> В (`in`)</li></ul> |
| Операторы отношения | <ul><li> Меньше (`lt`) </li><li> Больше (`gt`)</li><li> Меньше или равно (`le`)</li><li> Больше или равно (`ge`)</li></ul> |
| Лямбда-операторы | <ul><li> Любой (`any`) </li><li> Все (`all`)</li></ul>|
| Условные операторы | <ul><li> И (`and`) </li><li> Или (`or`)</li> |
| Functions | <ul><li> Начинается с (`startsWith`) </li><li> Оканчивается на (`endsWith`)</li><li> Содержит (`contains`)</li></ul>|

> [!NOTE]
> Поддержка этих операторов зависит от сущности, а некоторые свойства поддерживают `$filter` только в [расширенных запросах](/graph/aad-advanced-queries). Дополнительные сведения см. в документации по конкретным сущностям.

### <a name="filter-using-lambda-operators"></a>Фильтрация с помощью лямбда-операторов

OData определяет операторы `any` и `all` для проверки совпадений у свойств с несколькими значениями (т. е. либо коллекции примитивов, например типа String, либо коллекции сущностей).

#### <a name="any-operator"></a>Оператор  `any`

Оператор `any` итеративно применяет логическое выражение к каждому элементу коллекции и возвращает `true`, если выражение равно `true` для *любого элемента* коллекции. В противном случае этот оператор возвращает `false`. Ниже приводится синтаксис оператора `any`:

```http
$filter=param/any(var:var/subparam eq 'value-to-match')
```

Где
+ *param* — свойство, содержащее коллекцию значений или коллекцию сущностей.
+ *var:var* — переменная диапазона, содержащая текущий элемент коллекции во время итерации. Этой переменной можно назначить любое имя, например *adele:adele* или *x:x*.
+ *subparam* требуется, когда запрос применяется к коллекции сущностей. Он представляет свойство сложного типа, значение которого мы сравниваем.
+ *value-to-match* представляет элемент коллекции, с которым мы выполняем сравнение.

Например, свойство **imAddresses** ресурса user может содержать коллекцию простого типа String. Следующий запрос получает только пользователей, у которых свойство imAddress имеет значение `admin@contoso.com`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=imAddresses/any(s:s eq 'admin@contoso.com')
```

Свойство **assignedLicenses** ресурса user содержит коллекцию объектов **assignedLicense**, сложный тип с двумя свойствами **skuId** и **disabledPlans**. Следующий запрос получает только пользователей с назначенной лицензией, которая идентифицируется по **skuId** `184efa21-98c3-4e5d-95ab-d07053a96e67`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=assignedLicenses/any(s:s/skuId eq 184efa21-98c3-4e5d-95ab-d07053a96e67)
```

Чтобы инвертировать результат выражения внутри предложения `any`, используйте оператор `not`, а не `ne`. Например, следующий запрос получает только пользователей, у которых свойству **imAddress** не назначено значение `admin@contoso.com`.

> [!NOTE]
> Для объектов каталога, таких как пользователи, операторы `not` и `ne` поддерживаются только в [расширенных запросах](/graph/aad-advanced-queries).

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=NOT(imAddresses/any(s:s eq 'admin@contoso.com'))&$count=true
ConsistencyLevel: eventual
```

#### <a name="all-operator"></a>Оператор  `all`

Оператор `all` применяет логическое выражение к каждому элементу коллекции и возвращает `true`, если выражение равно `true` для *всех элементов* коллекции. В противном случае этот оператор возвращает `false`. Он не поддерживается никакими свойствами.

### <a name="examples-using-the-filter-query-operator"></a>Примеры использования оператора фильтрации запросов

Приведенная ниже таблица содержит несколько примеров использования параметра запроса `$filter`. Дополнительные сведения о синтаксисе `$filter` см. в статье [Протокол OData][odata-filter].

> [!NOTE]
> Щелкните примеры, чтобы попробовать поработать с ними в [песочнице Graph][graph-explorer].

| Описание | Пример
|:------------|:--------|
| Получение всех пользователей с именем Маша по нескольким свойствам. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) `../users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')` |
| Получение всех пользователей с почтовым доменом "hotmail.com" | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@hotmail.com')`. Это [расширенный запрос](/graph/aad-advanced-queries). |
| Получение всех пользователей без назначенных лицензий | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedLicenses%2F%24count%2Bne%2B0%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedLicenses/$count eq 0&$count=true`. Это [расширенный запрос](/graph/aad-advanced-queries). |
| Получение всех событий для вошедшего в систему пользователя, начинающихся начинаются после 01.07.2017 г. | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) `../me/events?$filter=start/dateTime ge '2017-07-01T08:00'`. <br/>**ПРИМЕЧАНИЕ.** Свойство **dateTime** относится к строковому типу. |
| Получение всех сообщений с определенного адреса, полученных вошедшим пользователем. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) `../me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'` |
| Получение всех сообщений, полученных вошедшим пользователем в апреле 2017 г. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01` |
| Получение всех непрочитанных сообщений в папке "Входящие" вошедшего пользователя. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=isRead eq false` |
| Получение всех пользователей в отделах розничной торговли и продаж. | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3Ddepartment%20in%20('Retail'%2C%20'Sales')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) `../users?$filter=department in ('Retail', 'Sales')`| 
| Перечисление пользователей с определенным планом обслуживания,находящимся в приостановленном состоянии. | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedPlans%2Fany(a%3Aa%2FservicePlanId%20eq%202e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2%20and%20a%2FcapabilityStatus%20eq%20'Suspended')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedPlans/any(a:a/servicePlanId eq 2e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2 and a/capabilityStatus eq 'Suspended')&$count=true`. Это [расширенный запрос](/graph/aad-advanced-queries). |
| Перечисление всех групп, не входящих в Microsoft 365, в организации. | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DNOT%20groupTypes%2Fany(c%3Ac%20eq%20'Unified')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=NOT groupTypes/any(c:c eq 'Unified')&$count=true`. Это [расширенный запрос](/graph/aad-advanced-queries). |
| Перечисление всех пользователей, у которых название компании не определено (т. е. не является значением `null`) или равно Microsoft. | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`. Это [расширенный запрос](/graph/aad-advanced-queries). |
| Перечисление всех пользователей, у которых название компании не определено или равно Microsoft. | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20in%20(null%2C%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName in (null, 'Microsoft')&$count=true`. Это [расширенный запрос](/graph/aad-advanced-queries). |
| Используйте преобразование OData, чтобы получить транзитивное членство в группах с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов. | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`. Это [расширенный запрос](/graph/aad-advanced-queries). |

## <a name="format-parameter"></a>Параметр format

Параметр запроса `$format` позволяет указать формат мультимедиа для элементов, возвращаемых из Microsoft Graph.

Например, указанный ниже запрос возвращает список пользователей организации в формате JSON.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$format=json
```

> [!NOTE]
> Параметр запроса `$format` поддерживает ряд форматов (например, атом, xml и json), но результаты могут быть возвращены не во всех форматах.

## <a name="orderby-parameter"></a>Параметр orderby

Параметр запроса `$orderby` позволяет указать порядок сортировки элементов, возвращаемых из Microsoft Graph. По умолчанию используется сортировка по возрастанию.

Например, следующий запрос возвращает список пользователей в организации, упорядоченный по отображаемому имени:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

Вы также можете сортировать данные по объектам сложного типа. Приведенный ниже запрос позволяет получить сообщения и отсортировать их по полю **address** свойства **from**, принадлежащего к сложному типу **emailAddress**.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

Чтобы отсортировать результаты по возрастанию или убыванию, добавьте `asc` или `desc` к имени поля, используя пробел для разделения, например: `?$orderby=name%20desc`. Если порядок сортировки не указан, используется порядок сортировки по умолчанию (по возрастанию).

Некоторые API дают возможность упорядочивать результаты по нескольким свойствам. Например, следующий запрос позволяет упорядочить сообщения в папке "Входящие" пользователя сначала по имени отправителя по убыванию (от Я до А), а затем — по теме по возрастанию (по умолчанию).

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

> [!NOTE]
> Если указать `$filter`, сервер выведет порядок сортировки результатов. Если вы одновременно используете `$orderby` и `$filter` для получения сообщений, так как сервер всегда определяет порядок сортировки результатов `$filter`, [необходимо задать свойства определенным образом](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).


В приведенном ниже примере показан запрос, отфильтрованный по свойствам **subject** и **importance**, а затем отсортированный по свойствам **subject**, **importance** и **receivedDateTime** в порядке убывания.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```


> [!NOTE] 
> Для объектов каталога поддерживаются параметры запросов `$orderby` и `$filter`. См. [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

## <a name="search-parameter"></a>Параметр search

Параметр запроса `$search` позволяет ограничить результаты запроса с помощью условия поиска. Синтаксис и поведение различаются для разных операций API. Сведения о синтаксисе `$search` для разных ресурсов см. в статье [Использование параметра запроса $search для сопоставления с условием поиска](/graph/search-query-parameter).

## <a name="select-parameter"></a>Параметр select

Параметр запроса `$select` позволяет возвратить набор свойств, отличный от набора по умолчанию, для отдельного ресурса или коллекции ресурсов. С помощью `$select` можно указать подмножество или надмножество свойств по умолчанию.

Например, при получении сообщений вошедшего пользователя можно указать, что необходимо вернуть только свойства **from** и **subject**:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

> [!IMPORTANT]
> В общем, мы рекомендуем вам использовать `$select`, чтобы ограничить свойства, возвращаемые запросом, теми, которые необходимы вашему приложению. Это особенно касается запросов, которые могут возвращать большой результирующий набор. Ограничение набора свойств, возвращаемых в каждой строке, позволяет уменьшить сетевую нагрузку и повысить производительность вашего приложения.
>
> В `v1.0` некоторые ресурсы Azure AD, производные от [directoryObject](/graph/api/resources/directoryobject), такие как [user](/graph/api/resources/user) и [group](/graph/api/resources/group), возвращают при чтении ограниченное подмножество свойств по умолчанию. С этими ресурсами параметр `$select` необходимо использовать для возврата свойств, не входящих в набор по умолчанию.  

## <a name="skip-parameter"></a>Параметр skip

Параметр запроса `$skip` позволяет задать количество элементов, которое необходимо пропустить в начале коллекции. Например, следующий запрос возвращает события пользователя, отсортированные по дате создания, начиная с 21-го события в коллекции:

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

> [!NOTE]
> Некоторые API Microsoft Graph, такие как Почта и календари Outlook (**сообщение**, **событие** и **календарь**), используют `$skip` для реализации разбиения по страницам. Если результаты запроса занимают несколько страниц, эти API возвращают свойство `@odata:nextLink` с URL-адресом, содержащим параметр `$skip`. Этот URL-адрес можно использовать для возврата следующей страницы результатов. [Подробнее…](./paging.md)
>
> Заголовок **ConsistencyLevel** требуется для расширенных запросов объектов каталога. Этот заголовок по умолчанию не включен в запросы последующих страниц. Его необходимо явным образом задавать на последующих страницах.

## <a name="skiptoken-parameter"></a>Параметр skipToken

Некоторые запросы возвращают несколько страниц данных. Это происходит из-за разбиения по страницам на стороне сервера или из-за использования параметра [`$top`](#top-parameter), который ограничивает размер возвращаемых страниц. Многие API Microsoft Graph используют параметр запроса `skipToken` для ссылки на следующие страницы результатов.  
Параметр `$skiptoken` содержит непрозрачный маркер, который ссылается на следующую страницу результатов и возвращается в URL-адресе, указанном в свойстве `@odata.nextLink` отклика. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md).

> [!NOTE]
> Если вы используете OData Count (добавляя `$count=true` в строку запроса) для запросов к объектам каталога, свойство `@odata.count` присутствует только на первой странице.
>
> Заголовок **ConsistencyLevel** требуется для расширенных запросов объектов каталога. Этот заголовок по умолчанию не включен в запросы последующих страниц. Его необходимо явным образом задавать на последующих страницах.

## <a name="top-parameter"></a>Параметр top

Параметр запроса `$top` позволяет задать размер страницы в результирующем наборе. 

Если результирующий набор будет содержать больше одной страницы элементов, тело отклика будет содержать параметр `@odata.nextLink`. Этот параметр содержит URL-адрес, с помощью которого можно получить следующую страницу результатов. Дополнительные сведения см. в статье о [разбиении по страницам](./paging.md). 

Минимальное значение $top является 1, а максимальное зависит от соответствующего API.  

Например, следующий запрос [сообщений списка](/graph/api/user-list-messages) возвращает первые пять сообщений в почтовом ящике пользователя:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

> [!NOTE]
> Заголовок **ConsistencyLevel** требуется для расширенных запросов объектов каталога. Этот заголовок по умолчанию не включен в запросы последующих страниц. Его необходимо явным образом задавать на последующих страницах.

## <a name="error-handling-for-query-parameters"></a>Обработка ошибок параметров запроса

Некоторые запросы возвращают сообщение об ошибке, если указанный параметр запроса не поддерживается. Например, невозможно использовать `$expand` для связи `user/photo`. 

```http
https://graph.microsoft.com/v1.0/me?$expand=photo
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

## <a name="see-also"></a>См. также

- [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries)
- [Использование параметра запроса $search для сопоставления с условием поиска](/graph/search-query-parameter)
- [Ограничения параметров запроса](known-issues.md#query-parameters)
