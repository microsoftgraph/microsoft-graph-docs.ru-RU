---
title: 'orgContact: delta'
description: Получение только что созданных, обновленных или удаленных контактов организации без необходимости выполнять полное чтение всей коллекции.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ce163bd35d82d67b52cd5984073b2b847ff9f080
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247219"
---
# <a name="orgcontact-delta"></a>orgContact: delta

Пространство имен: microsoft.graph

Получение только что созданных, обновленных или удаленных контактов организации без необходимости выполнять полное чтение всей коллекции. Дополнительные сведения см. в статье [Отслеживание изменений](/graph/delta-query-overview).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.  |
|Для приложений | OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы начать отслеживание изменений, выполните запрос, включая функцию delta в ресурсе контактов.

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений в контактах организации вызывает один или несколько вызовов **разностных** функций. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `@odata.nextLink` или `@odata.deltaLink`, включенного в отклик.

Необходимо указать параметры запроса только один раз заранее.

В последующих запросах скопируйте и примените URL-адрес `@odata.nextLink` из `@odata.deltaLink` предыдущего ответа. Этот URL-адрес уже содержит закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния, возвращенный](/graph/delta-query-overview) `@odata.deltaLink` в URL-адресе предыдущего вызова разностной функции для той же коллекции контактов организации, что указывает на завершение этого цикла отслеживания изменений. Сохраните и примените `@odata.deltaLink` весь URL-адрес, включая этот маркер, в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный `@odata.nextLink` в URL-адресе предыдущего вызова функции delta, указывающий на то, что в той же коллекции контактов организации будут отслеживаться дальнейшие изменения. |

### <a name="odata-query-parameters"></a>Параметры запросов OData

Этот метод поддерживает необязательные параметры запроса OData для настройки ответа.

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство **id** возвращается всегда.
- Имеется ограниченная поддержка параметра `$filter`:
  - Единственное поддерживаемое выражение `$filter` предназначено для отслеживания изменений в определенном объекте: `$filter=id+eq+{value}`. Допускается фильтрация нескольких объектов. Например, `https://graph.microsoft.com/v1.0/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Максимальное количество фильтруемых объектов: 50.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Носитель &lt;токен&gt;. Обязательный.|
| Prefer | return=minimal <br><br>Указание этого заголовка с запросом, использующим параметр `@odata.deltaLink`, приведет к возвращению только свойств объекта, измененных с момента последнего цикла. Необязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и ab [объект коллекции orgContact](../resources/orgcontact.md) в тексте отклика. Оклик также содержит URL-адрес `@odata.nextLink` или `@odata.deltaLink`.

- Если возвращается URL-адрес `@odata.nextLink`:
  - Это означает, что в сеансе должны быть извлечены дополнительные страницы данных. Приложение продолжает отправлять запросы, используя URL-адрес `@odata.nextLink`, пока в отклик не будет включен URL-адрес `@odata.deltaLink`.
  - Отклик включает тот же набор свойств, что и начальный разностный запрос. Это позволяет фиксировать полное текущее состояние объектов при запуске разностного цикла.

- Если возвращается URL-адрес `@odata.deltaLink`:
  - Это означает, что больше нет данных о существующем состоянии возвращаемого ресурса. Сохраните и используйте URL-адрес `@odata.deltaLink`, чтобы узнавать об изменениях ресурса в следующем цикле.
  - Вы можете указать заголовок `Prefer:return=minimal`, чтобы включить в значения отклика только свойства, измененные с момента создания `@odata.deltaLink`.

### <a name="default-return-the-same-properties-as-initial-delta-request"></a>По умолчанию: возвращение свойств, совпадающих с начальным разностным запросом

По умолчанию запросы с использованием `@odata.deltaLink` или `@odata.nextLink` возвращают те же свойства, которые выбраны в начальном разностном запросе, следующим образом:

- Если свойство изменилось, в отклике содержится новое значение. Сюда включаются свойства с заданным значением NULL.
- Если свойство не изменилось, в отклике содержится старое значение.
- Если свойство никогда не было задано ранее, оно не будет включено в ответ.


> **Примечание:** При таком поведении невозможно определить, изменяется ли свойство, просмотрев ответ. Кроме того, разностные ответы, как правило, являются большими, так как содержат все значения свойств, как показано в [примере 2](#example-2-selecting-three-properties).

### <a name="alternative-return-only-the-changed-properties"></a>Альтернатива: возвращение только измененных свойств

Добавление необязательного заголовка запроса `prefer:return=minimal` приводит к следующему результату:

- Если свойство изменилось, в отклике содержится новое значение. Сюда включаются свойства с заданным значением NULL.
- Если свойство не изменилось, оно не включается в отклик. (Отличается от поведения по умолчанию.)

> **Примечание.** Заголовок можно добавить в запрос `@odata.deltaLink` в любой момент разностного цикла. Заголовок влияет только на набор свойств, включенных в ответ, и не влияет на способ выполнения разностного запроса. См. [пример 3](#example-3-alternative-minimal-response-behavior).

## <a name="examples"></a>Примеры

### <a name="example-1-default-properties"></a>Пример 1. Свойства по умолчанию

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. Параметр `$select` отсутствует, поэтому отслеживается и возвращается набор свойств по умолчанию.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgContact_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/orgcontact-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/orgcontact-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика при использовании параметра `@odata.deltaLink`, полученного в начале запроса.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "id": "string (identifier)",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mailNickname": "mailNickname-value",
      "surname": "surname-value"
    }
  ]
}
```

### <a name="example-2-selecting-three-properties"></a>Пример 2. Выбор трех свойств

#### <a name="request"></a>Запрос

В следующем примере показан исходный запрос с выбором трех свойств для отслеживания изменений с поведением отклика по умолчанию.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta?$select=displayName,jobTitle,mail
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/orgcontact-delta-select-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/orgcontact-delta-select-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика при использовании параметра `@odata.deltaLink`, полученного в начале запроса. Обратите внимание, что все три свойства включаются в отклик, и неизвестно, какие из них изменились с момента получения `@odata.deltaLink`.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mail": null
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a>Пример 3. Альтернативное поведение минимального отклика

#### <a name="request"></a>Запрос

В следующем примере показан исходный запрос с выбором трех свойств для отслеживания изменений с альтернативным поведением отклика с минимальными результатами.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/delta?$select=displayName,jobTitle,mail
Prefer: return=minimal
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/orgcontact-delta-minimal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/orgcontact-delta-minimal-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика при использовании параметра `@odata.deltaLink`, полученного в начале запроса. Обратите внимание, что свойство `mail` не включено, то есть оно не изменилось с последнего разностного запроса; `displayName` и `jobTitle` включены, то есть их значения изменились.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a>См. также

- [Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).

<!-- uuid: 3B5A9A7C-6324-432F-8C66-AC4883DD71EF
2020-03-20 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

