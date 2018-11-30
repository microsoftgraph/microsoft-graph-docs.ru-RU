---
title: 'directoryObject: дельты'
description: 'Get вновь созданных, обновлении или удалении объектов каталога из следующих типов: пользователей, группы и организационной контакт в запросе единого дельты. Отслеживание изменений для получения дополнительных сведений см.'
ms.openlocfilehash: 98674a141c0567defb06da7b1ccd95a209aaa4f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076684"
---
# <a name="directoryobject-delta"></a>directoryObject: дельты

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Get вновь созданных, обновлении или удалении объектов каталога из следующих типов: [пользователей](../resources/user.md), [группы](../resources/group.md) и [организационной контактов](../resources/orgcontact.md), в запросе единого дельты. Дополнительные сведения см [Отслеживание изменений](/graph/delta-query-overview) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.AccessAsUser.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.  |
|Для приложений | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы начать отслеживание изменений, внесите запроса, включая функцию дельты на directoryObjects ресурсов.

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений приводит к round один или несколько вызовов функций **дельты** . При использовании любого параметра запроса (отличный от `$deltatoken` и `$skiptoken`), необходимо указать его в запрос начальной **дельты** . Microsoft Graph автоматически Кодирует указанный параметров в маркеров часть `nextLink` или `deltaLink` URL-адреса, приведенные в ответе.

Параметры запроса нужно указать только один раз в первом запросе.

Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.

| Параметр запроса | Тип |Описание|
|:---------------|:--------|:----------|
| $deltatoken | строка | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | строка | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Этот метод поддерживает дополнительные параметры запроса OData для настройки ответа.

- Можно использовать `$filter` с специальные `isOf` оператор для фильтрации подмножество типов, производные от directoryObject.
  - Вы можете сочетать несколько выражений с помощью `or`, позволяет запросе единого дельты отслеживание нескольких типов. [Третий пример](#request-3) для получения дополнительных сведений см.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | Возвращает = минимальный <br><br>Указание этот заголовок с запросом, который использует `deltaLink` возвращает свойства объекта, которые были изменены с момента последнего цикла. Необязательный параметр. |

## <a name="request-body"></a>Тело запроса

Не указывайте тело запроса для этого метода.

### <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` ответа [пользователя](../resources/directoryobject.md) и кода объект коллекции в теле ответа. Ответ также включает `nextLink` URL-адрес или `deltaLink` URL-адрес.

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


> **Примечание:** С помощью этого поведения, посмотрев ответа не позволяет определить, будет ли свойство изменяется, или не. Кроме того ответы дельты приводят к занимать много места, так как они содержат все значения свойств.

#### <a name="alternative-return-only-the-changed-properties"></a>Альтернатива: получить только измененные свойства

Добавление заголовка запроса на необязательный - `prefer:return=minimal` -приводит к следующим образом:

- При изменении свойства новое значение включается в ответе. Этот компонент включает свойства задаются на значение null.
- Если свойство не был изменен, свойство не включается в ответ на всех. (Отличается от поведения по умолчанию).

> **Примечание:** Можно добавить заголовок `deltaLink` запроса в любой момент времени в цикле дельты. Заголовок влияет только на набор свойств, включенных в ответ и не затрагивает как выполняется запрос дельты.

## <a name="example"></a>Пример

### <a name="request-1"></a>Запрос 1

Ниже приведен пример запроса. Существует не `$select` параметр, поэтому по умолчанию набор свойств, отслеживаемых и возвращаются.
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a>Ответ 1

Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса. Не `isOf` был использован фильтр, поэтому возвращаются все типы, производные от directoryObject.

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",
      "id": "string (identifier)",
      "jobTitle": "string",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-2"></a>Запрос 2

В следующем примере показано использование поведение альтернативный минимальной ответа:
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a>Ответ 2

Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса. Обратите внимание, что возвращаются только свойства, которые фактически были изменены.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-3"></a>Запрос 3

В следующем примере показано использование начального запроса `isOf` оператор для фильтрации объектов пользователей и групп:
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a>Ответ 3

Ниже приведен пример ответа при использовании `deltaLink` полученных при инициализации запроса. Обратите внимание на то, что возвращаются только объекты пользователей и групп:

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
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
