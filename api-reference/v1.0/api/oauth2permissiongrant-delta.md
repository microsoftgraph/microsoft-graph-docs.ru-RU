---
title: 'oauth2permissiongrant: дельта'
description: Получить заново созданные, обновленные или удаленные oauth2permissiongrants без выполнения полного чтения всей коллекции ресурсов.
ms.localizationpriority: medium
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 23b4e38d5ea91d2b66507ed5e2f98e3f2a218290
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59015975"
---
# <a name="oauth2permissiongrant-delta"></a>oauth2permissiongrant: дельта

Пространство имен: microsoft.graph

Получить вновь созданные, обновленные или удаленные [объекты oauth2permissiongrant](../resources/oauth2permissiongrant.md) без полного чтения всей коллекции ресурсов. Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений вызывает один или несколько вызовов функции **дельты.** Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Необходимо указать параметры запроса только один раз. В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа. URL-адрес содержит закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущей функции дельты, вызываем для того же собрания ресурсов, что указывает на завершение этого раунда отслеживания `deltaLink` изменений.  Сохраните и примените весь URL-адрес, включая этот маркер, в первом запросе следующего раунда отслеживания `deltaLink` изменений для этой коллекции.|
| $skiptoken | string | Маркер [состояния,](/graph/delta-query-overview) возвращенный в URL-адрес предыдущего вызова функции дельты, указывает на то, что в том же собрании ресурсов необходимо отслеживать дальнейшие `nextLink` изменения.  |

### <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки ответа.

- Параметр запроса можно указать только свойства, необходимые `$select` для лучшей производительности. Свойство **id** возвращается всегда.
- Параметр запроса можно использовать только для отслеживания изменений на определенных `$filter` ресурсах с помощью ИД ресурса. Например, `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект коллекции oauth2permissiongrant](../resources/oauth2permissiongrant.md) в тексте ответа. Отклик также содержит URL-адрес `nextLink` или `deltaLink`.

- Если URL-адрес возвращается, в сеансе могут быть извлечены `nextLink` дополнительные страницы данных. **Oauth2permissiongrant** продолжает делать запросы с помощью URL-адреса до тех пор, пока URL-адрес не будет включен `nextLink` `deltaLink` в ответ.
- Если `deltaLink` URL-адрес возвращается, больше не возвращаются данные о ресурсе. Сохраните и используйте `deltaLink` URL-адрес, чтобы узнать об изменениях в ресурсе в будущем.

Подробные сведения см. в [материале Использование запроса delta.](/graph/delta-query-overview) Например, запросы см. [в рублях Получить дополнительные изменения для пользователей.](/graph/delta-query-users)

## <a name="example"></a>Пример
### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

