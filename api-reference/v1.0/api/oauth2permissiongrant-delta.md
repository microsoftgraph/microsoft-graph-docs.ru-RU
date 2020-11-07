---
title: 'oauth2permissiongrant: Delta'
description: Получите только что созданный, обновленный или удаленный oauth2permissiongrants, не выполняя полный просмотр всей коллекции ресурсов.
localization_priority: Normal
author: psignoret
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef244ecab046800ccd877d4c3f26414fa8ce1de9
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932502"
---
# <a name="oauth2permissiongrant-delta"></a>oauth2permissiongrant: Delta

Пространство имен: microsoft.graph

Получение только что созданных, обновленных или удаленных объектов [oauth2permissiongrant](../resources/oauth2permissiongrant.md) без выполнения полного считывания всей коллекции ресурсов. Подробнее: [Использование запроса изменений](/graph/delta-query-overview).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|oauth2permissiongrant | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a>Параметры запроса

Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** . Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в начальном запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в маркере, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в отклик. Параметры запроса необходимо указывать только один раз. В последующих запросах скопируйте и примените `nextLink` `deltaLink` URL-адрес из предыдущего ответа. URL-адрес содержит закодированные параметры.

| Параметр запроса      | Тип   |Описание|
|:---------------|:--------|:----------|
| $deltatoken | string | [Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции ресурсов, что указывает на завершение этого круга отслеживания изменений. Сохраните и примените весь `deltaLink` URL-адрес, включая этот маркер, в первом запросе следующего цикла отслеживания изменений для этой коллекции.|
| $skiptoken | string | [Маркер состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая на то, что в коллекции ресурсов имеются дальнейшие изменения, которые необходимо отслеживать. |

### <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки ответа.

- `$select`С помощью параметра запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности. Свойство **id** возвращается всегда.
- `$filter`Параметр Query можно использовать только для отслеживания изменений определенных ресурсов с помощью идентификатора ресурса. Например, `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}` .


## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [oauth2permissiongrant](../resources/oauth2permissiongrant.md) в тексте отклика. Отклик также содержит URL-адрес `nextLink` или `deltaLink`.

- Если `nextLink` возвращается URL-адрес, дополнительные страницы данных можно получить в сеансе. **Oauth2permissiongrant** продолжает совершать запросы, используя `nextLink` URL-адрес, пока `deltaLink` в ответ не будет включен URL-адрес.
- Если `deltaLink` возвращается URL-адрес, дополнительные данные о ресурсе не возвращаются. Следует оставить и использовать `deltaLink` URL-адрес для получения сведений об изменениях в ресурсе в будущем.

Подробнее: [Использование запроса изменений](/graph/delta-query-overview). Примеры запросов приведены в статье [получение добавочных изменений для пользователей](/graph/delta-query-users).

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
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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

