---
title: 'directoryObject: Delta'
description: 'Получение новых, обновленных или удаленных объектов каталога для следующих типов: User, Group и Contact Contact в едином разностном запросе. Сведения об исправлениях приведены в разделе Tracking.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 56ee662050858ff3d46b12b6885ba9e418d0e59d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455172"
---
# <a name="directoryobject-delta"></a>directoryObject: Delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение новых, обновленных или удаленных объектов каталога для следующих типов: [User](../resources/user.md), [Group](../resources/group.md) и [Contact Contact](../resources/orgcontact.md)в едином разностном запросе. Сведения [](/graph/delta-query-overview) об исправлениях приведены в разделе Tracking.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.AccessAsUser.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.  |
|Для приложений | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы начать отслеживание изменений, создайте запрос, включающий функцию Delta в ресурсе Директорйобжектс.

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** . Если вы используете любой параметр запроса (кроме `$deltatoken` и `$skiptoken`), необходимо указать его в исходном запросе **Delta** . Microsoft Graph автоматически кодирует все заданные параметры в часть маркера или `nextLink` `deltaLink` URL-адрес, указанный в ответе.

Параметры запроса нужно указать только один раз в первом запросе.

Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.

| Параметр запроса | Тип |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | строка | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.

- `$filter` С помощью специального `isOf` оператора можно фильтровать подмножество типов, производных от directoryObject.
  - Можно объединить несколько выражений с помощью элемента `or`, который позволяет использовать одну разностную трассировку запросов нескольких типов. Более подробную информацию можно узнать в [третьем примере](#request-3) .

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | Возврат = минимум <br><br>При указании заголовка с запросом, который `deltaLink` использует объект, возвращаются только свойства объекта, которые были изменены с момента последнего цикла. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

### <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции [user](../resources/directoryobject.md) в тексте ответа. В ответ также включается `nextLink` URL-адрес `deltaLink` или URL-адрес.

- Если возвращается `nextLink` URL-адрес:
  - Это указывает на необходимость извлечения дополнительных страниц данных в сеансе. Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.
  - Ответ включает тот же набор свойств, что и в исходном запросе на разностный запрос. Это позволяет захватить полное текущее состояние объектов при инициации разностного цикла.

- Если возвращается `deltaLink` URL-адрес:
  - Это указывает на то, что больше нет данных о существующем состоянии ресурса, который необходимо возвратить. Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях ресурса в следующем цикле.
  - Вы можете указать `Prefer:return=minimal` заголовок, чтобы включить в значения отклика только те свойства, которые были изменены с момента `deltaLink` выпуска.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>По умолчанию: возврат тех же свойств, что и исходный запрос Дельта

По умолчанию запросы, использующие `deltaLink` или `nextLink` возвращающие те же свойства, что и выбранные в начальном запросе Дельта, запрашиваются следующими способами:

- Если свойство изменилось, в ответ включается новое значение. Сюда входят свойства, для которых задано значение null.
- Если свойство не изменилось, в ответ включается старое значение.
- Если свойство никогда не задается до тех пор, пока оно не будет включено в ответ вообще.


> **Примечание:** Таким образом, изучив ответ, можно определить, изменяется ли свойство. Кроме того, разностные ответы обычно имеют большой размер, так как они содержат все значения свойств.

#### <a name="alternative-return-only-the-changed-properties"></a>Альтернатива: возврат только измененных свойств

Добавление необязательного заголовка запроса `prefer:return=minimal` — приводит к следующему поведению:

- Если свойство изменилось, в ответ включается новое значение. Сюда входят свойства, для которых задано значение null.
- Если свойство не изменилось, свойство не включается в ответ вообще. (Отличается от поведения по умолчанию.)

> **Примечание:** Заголовок можно добавить в `deltaLink` запрос в любой момент времени в разностном цикле. Заголовок влияет только на набор свойств, включенных в ответ, и не влияет на то, как выполняется разностный запрос.

## <a name="example"></a>Пример

### <a name="request-1"></a>Запрос 1

Ниже приведен пример запроса. Параметр не `$select` задан, поэтому набор свойств по умолчанию отслеживается и возвращается.
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a>Отклик 1

Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса. Фильтр `isOf` не использовался, поэтому возвращаются все типы, производные от directoryObject.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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

В следующем примере показано использование альтернативного поведения минимального ответа:
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a>Отклик 2

Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса. Обратите внимание, что возвращаются только те свойства, которые действительно изменились.

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

В следующем примере показан начальный запрос с помощью `isOf` оператора для фильтрации только сущностей "пользователь" и "Группа":
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a>Отклик 3

Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса. Обратите внимание, что возвращаются только объекты user и Group:

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

- [Использование запроса изменений для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).
- [Получение добавочных изменений для пользователей](/graph/delta-query-users).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
