---
title: 'user: delta'
description: Получение новых, обновленных или удаленных пользователей без выполнения полного чтения коллекции пользователей целиком. Сведения об исправлениях приведены в разделе Tracking.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537005"
---
# <a name="user-delta"></a>user: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение новых, обновленных или удаленных пользователей без выполнения полного чтения коллекции пользователей целиком. Сведения [](/graph/delta-query-overview) об исправлениях приведены в разделе Tracking.

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

Отслеживание изменений в пользователях приводит к округлению одного или нескольких вызовов функции **Delta** . Если вы используете любой параметр запроса (кроме `$deltatoken` и `$skiptoken`), необходимо указать его в исходном запросе **Delta** . Microsoft Graph автоматически кодирует все заданные параметры в часть маркера или `nextLink` `deltaLink` URL-адрес, указанный в ответе.

Параметры запроса нужно указать только один раз в первом запросе.

Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции пользователей и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | строка | Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что в коллекции пользователей остаются неотслеженные изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство *id* возвращается всегда.
- Существует ограниченная поддержка `$filter`:
  - Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`. Допускается фильтрация нескольких объектов. Например, `https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Максимальное количество фильтруемых объектов: 50.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer &lt;token&gt;|
| Content-Type  | application/json |
| Prefer | Возврат = минимум <br><br>При указании заголовка с запросом, который `deltaLink` использует объект, возвращаются только свойства объекта, которые были изменены с момента последнего цикла. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

### <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции [user](../resources/user.md) в тексте ответа. В ответ также включается `nextLink` URL-адрес `deltaLink` или URL-адрес.

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


> **Примечание:** Таким образом, изучив ответ, можно определить, изменяется ли свойство. Кроме того, разностные ответы обычно имеют большой размер, так как они содержат все значения свойств, как показано во [втором примере](#request-2) ниже.

#### <a name="alternative-return-only-the-changed-properties"></a>Альтернатива: возврат только измененных свойств

Добавление необязательного заголовка запроса `prefer:return=minimal` — приводит к следующему поведению:

- Если свойство изменилось, в ответ включается новое значение. Сюда входят свойства, для которых задано значение null.
- Если свойство не изменилось, свойство не включается в ответ вообще. (Отличается от поведения по умолчанию.)

> **Примечание:** Заголовок можно добавить в `deltaLink` запрос в любой момент времени в разностном цикле. Заголовок влияет только на набор свойств, включенных в ответ, и не влияет на то, как выполняется разностный запрос. Просмотрите [третий пример](#request-3) ниже.

### <a name="example"></a>Пример

#### <a name="request-1"></a>Запрос 1

Ниже приведен пример запроса. Параметр не `$select` задан, поэтому набор свойств по умолчанию отслеживается и возвращается.
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a>Отклик 1

Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

В следующем примере показан первоначальный запрос, в котором выбирается 3 свойства для отслеживания изменений с поведением ответа по умолчанию:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a>Отклик 2

Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса. Обратите внимание на то, что в ответ включены все 3 свойства, и они не известны, какие из `deltaLink` них были изменены с момента получения.

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

В следующем примере показано, как исходный запрос выбирает 3 свойства для отслеживания изменений с альтернативным поведением минимального ответа:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a>Отклик 3

Ниже приведен пример ответа, полученного при использовании метода `deltaLink` , полученного при инициализации запроса. Обратите внимание `mobilePhone` , что свойство не включается, что означает, что он не изменился с момента последнего запроса Дельта; `displayName` и `jobTitle` включены, что означает, что их значения изменились.

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
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
    "Error: /api-reference/beta/api/user-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
