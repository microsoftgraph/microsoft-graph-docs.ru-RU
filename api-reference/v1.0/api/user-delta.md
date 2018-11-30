---
title: 'user: delta'
description: Get вновь созданных, обновлении или удалении пользователей без необходимости выполнять полное чтение коллекции всей пользователя. Отслеживание изменений для получения дополнительных сведений см.
ms.openlocfilehash: c460a15a63405a5f913096744b5eb150493c715d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028538"
---
# <a name="user-delta"></a>user: delta

Get вновь созданных, обновлении или удалении пользователей без необходимости выполнять полное чтение коллекции всей пользователя. Дополнительные сведения см [Отслеживание изменений](/graph/delta-query-overview) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | User.Read, User.ReadWrite    |
|Для приложений | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы начать отслеживать изменения, выполните запрос к ресурсу users, включающий функцию delta.

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений в пользователи могут возникать round один или несколько вызовов функций **дельты** . При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** . Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.

Параметры запроса нужно указать только один раз в первом запросе.

Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | строка | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | строка | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Этот метод поддерживает дополнительные параметры запроса OData для настройки ответа.

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.
- Ограниченная поддержка `$filter`:
  - Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`. Допускается фильтрация нескольких объектов. Например, `https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Максимальное количество фильтруемых объектов: 50.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | Возвращает = минимальный <br><br>Указание этот заголовок с запросом, который использует `deltaLink` возвращает свойства объекта, которые были изменены с момента последнего цикла. Необязательный параметр. |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

### <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` ответа [пользователя](../resources/user.md) и кода объект коллекции в теле ответа. Ответ также включает `nextLink` URL-адрес или `deltaLink` URL-адрес.

- Если `nextLink` возвращается URL-адрес:
  - Это означает, что существуют дополнительные страницы данных для получения в сеанс. Приложение по-прежнему производится выполняете запросы, используя `nextLink` URL-адрес, пока не `deltaLink` URL-адрес включен в ответе.
  - Ответ включает тот же набор свойств, как и в запросе начальной дельты. Это позволяет записывать полное текущего состояния объектов при начале цикла дельты.

- Если `deltaLink` возвращается URL-адрес:
  - Это означает, что нет дополнительных данных о состоянии существующих ресурсов должно быть возвращено. Сохраните и использовать `deltaLink` URL-адрес, чтобы узнать о изменяется с ресурсом в следующего цикла.
  - У вас есть выбор для указания `Prefer:return=minimal` заголовок, чтобы включить в ответ значения для свойств, которые были изменены со времени `deltaLink` был отправлен.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Значение по умолчанию: возврата же свойства, что запрос на начальное дельты

По умолчанию, запросы с помощью `deltaLink` или `nextLink` возврата же свойства, что выбранный в запросе начальной дельты следующими способами:

- При изменении свойства новое значение включается в ответе. Этот компонент включает свойства задаются на значение null.
- Если свойство не был изменен, старое значение включается в ответе.
- Если свойство имеет значение никогда не перед его не будут включены в ответе на всех.


> **Примечание:** С помощью этого поведения, посмотрев ответа не позволяет определить, будет ли свойство изменяется, или не. Кроме того ответы дельты, как правило больших так как они содержат все значения свойств - как показано в следующем [примере второй](#request-2) .

#### <a name="alternative-return-only-the-changed-properties"></a>Альтернатива: получить только измененные свойства

Добавление заголовка запроса на необязательный - `prefer:return=minimal` -приводит к следующим образом:

- При изменении свойства новое значение включается в ответе. Этот компонент включает свойства задаются на значение null.
- Если свойство не был изменен, свойство не включается в ответ на всех. (Отличается от поведения по умолчанию).

> **Примечание:** Можно добавить заголовок `deltaLink` запроса в любой момент времени в цикле дельты. Заголовок влияет только на набор свойств, включенных в ответ и не затрагивает как выполняется запрос дельты. В разделе в [третьем примере](#request-3) ниже.

### <a name="example"></a>Пример

#### <a name="request-1"></a>Запрос 1

Ниже приведен пример запроса. Существует не `$select` параметр, поэтому по умолчанию набор свойств, отслеживаемых и возвращаются.
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a>Ответ 1

Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса.

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a>Запрос 2

В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, с ответ по умолчанию:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a>Ответ 2

Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса. Обратите внимание на то, что все свойства 3 включенных в ответ и не известно, какие из них были изменены с момента `deltaLink` был получен.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a>Запрос 3

В следующем примере показаны начального запроса, выбрав пункт 3 свойства для отслеживания изменений, поведение альтернативный минимальной ответа:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a>Ответ 3

Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса. Обратите внимание, что `mobilePhone` свойство не указан, то есть не был изменен с момента последнего разностного запроса; `displayName` и `jobTitle` включены, что означает их значения были изменены.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- [Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).
- [Получение добавочные изменения для пользователей](/graph/delta-query-users).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->