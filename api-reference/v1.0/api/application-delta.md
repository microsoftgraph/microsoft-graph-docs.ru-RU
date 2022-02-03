---
title: 'приложение: дельта'
description: Создайте, обновим или удаляйте приложения без полного чтения всей коллекции ресурсов.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 59f7de435c4d1858e623c69fc5a808ed5f25e58e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342478"
---
# <a name="application-delta"></a>приложение: дельта

Пространство имен: microsoft.graph

Создавайте, обновляйте или удаляйте приложения без необходимости чтения всей коллекции ресурсов. Подробные сведения см. в [материале Использование delta-запроса](/graph/delta-query-overview).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.All, Directory.Read.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы начать отслеживание изменений, необходимо сделать запрос, включив функцию delta на **ресурсе** приложения. 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений вызывает один или несколько вызовов функции **дельты** . Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Необходимо указать параметры запроса только один раз. В последующих запросах скопируйте и примените `nextLink` URL-адрес `deltaLink` из предыдущего ответа. Этот URL-адрес уже содержит закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в `deltaLink` URL-адрес предыдущей  функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес `nextLink` предыдущего  вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие изменения. |

### <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки ответа.

- Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство **id** возвращается всегда.
- Имеется ограниченная поддержка параметра `$filter`:
  * Единственным поддерживаемым `$filter` выражением является отслеживание изменений для определенных ресурсов по их ID:  `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`. Количество url-адресов, которые можно указать, ограничено максимальной длиной URL-адреса.


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Носитель &lt;токен&gt;. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного применения этот метод возвращает код `200 OK` отклика [и объект коллекции](../resources/application.md) приложений в тексте ответа. Отклик также содержит URL-адрес `nextLink` или `deltaLink`.

- Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных. Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.
- Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса. Сохраните и используйте URL-адрес `deltaLink` , чтобы узнать об изменениях в ресурсе в будущем.

Подробные сведения см. в [материале Использование delta-запроса](/graph/delta-query-overview). Например, запросы см. [в рублях Получить дополнительные изменения для пользователей](/graph/delta-query-users).

## <a name="example"></a>Пример
### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/application-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/application-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

