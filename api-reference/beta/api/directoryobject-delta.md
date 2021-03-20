---
title: 'directoryObject: delta'
description: 'Получите вновь созданные, обновленные или удаленные объекты каталога следующих типов: пользовательский, групповой и организационный контакт в одном запросе дельты. Дополнительные сведения см. в статье "Отслеживание изменений".'
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 88a78e85d640c5d6e5c62fef239f29485d820897
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946654"
---
# <a name="directoryobject-delta"></a>directoryObject: delta

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите вновь созданные, обновленные или удаленные объекты каталога следующих [типов:](../resources/user.md) [пользовательский,](../resources/group.md) групповой и организационный контакт [в](../resources/orgcontact.md)одном запросе дельты. Дополнительные сведения см. в статье [Отслеживание изменений](/graph/delta-query-overview).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.AccessAsUser.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.  |
|Для приложений | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы начать отслеживание изменений, необходимо сделать запрос, включив функцию дельты на ресурсе directoryObjects.

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений вызывает один или несколько вызовов функции **дельты.** Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик.

Параметры запроса нужно указать только один раз в первом запросе.

Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.

| Параметр запроса | Тип |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим маркером и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | строка | Этот [маркер состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Этот метод поддерживает необязательные параметры запросов OData для настройки отклика.

- С помощью специального оператора можно `$filter` `isOf` отфильтровать подмножество типов, полученных из directoryObject.
  - Вы можете объединить несколько выражений с помощью одного запроса дельты, отслеживая `or` несколько типов. Сведения [см. в третьем](#request-3) примере.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | return=minimal <br><br>Указание этого заголовка с запросом, использующим параметр `deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла. Необязательно. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

### <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [user](../resources/directoryobject.md) в тексте отклика. Оклик также содержит URL-адрес `nextLink` или `deltaLink`.

- Если возвращается URL-адрес `nextLink`:
  - Это означает, что во время сеанса получены не все страницы данных. Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.
  - Отклик включает тот же набор свойств, что и начальный разностный запрос. Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.

- Если возвращается URL-адрес `deltaLink`:
  - Это означает, что больше нет данных о текущем состоянии ресурса. Сохраните и используйте URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.
  - Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `deltaLink`.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом

По умолчанию запросы с использованием `deltaLink` или `nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:

- Если свойство изменилось, в отклике содержится новое значение. Сюда включаются свойства с заданным значением NULL.
- Если свойство не изменилось, в отклике содержится старое значение.
- Если свойство ранее никогда не настраивалось, оно не включается в отклик.


> **Примечание.** При таком поведении просмотр отклика не дает возможность определить, изменилось ли свойство. Кроме того, ответы дельты, как правило, большие, так как они содержат все значения свойств.

#### <a name="alternative-return-only-the-changed-properties"></a>Альтернатива: возвращение только измененных свойств

Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:

- Если свойство изменилось, в отклике содержится новое значение. Сюда включаются свойства с заданным значением NULL.
- Если свойство не изменилось, оно не включается в отклик. (Отличается от поведения по умолчанию.)

> **Примечание.** Заголовок можно добавить в запрос `deltaLink` в любой момент разностного цикла. Заголовок влияет только на набор свойств, включенный в отклик, и не влияет на способ выполнения разностного запроса.

## <a name="example"></a>Пример

### <a name="request-1"></a>Запрос 1

Ниже приведен пример запроса. Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directory_object_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directory-object-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directory-object-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directory-object-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directory-object-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a>Отклик 1

Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса. Фильтр не используется, поэтому возвращаются все типы, полученные из `isOf` directoryObject.

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
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
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
      "jobTitle": "string"
    }
  ]
}
```

### <a name="request-2"></a>Запрос 2

В следующем примере показано использование альтернативного минимального поведения отклика:

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a>Отклик 2

Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса. Обратите внимание, что возвращаются только фактически измененные свойства.

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
    }
  ]
}
```

### <a name="request-3"></a>Запрос 3

В следующем примере показан начальный запрос с помощью оператора для фильтрации только `isOf` пользовательских и групповых сущностями:

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a>Отклик 3

Ниже приведен пример отклика при использовании параметра `deltaLink`, полученного в начале запроса. Обратите внимание, что возвращаются только объекты пользователя и группы:

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
      "jobTitle": null
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp"
    }
  ]
}
```

- [Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).
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
  ]
}
-->


