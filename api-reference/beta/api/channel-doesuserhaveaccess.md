---
title: 'channel: doesUserHaveAccess'
description: Определите, имеет ли пользователь доступ к общему каналу.
author: devjha-ms
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 808814a7c535a8a2ba9856eda0d8ec36a1170670
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211079"
---
# <a name="channel-doesuserhaveaccess"></a>channel: doesUserHaveAccess
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определите, [имеет ли пользователь](../resources/useridentity.md) доступ к общему [каналу](../resources/channel.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись) | ChannelMember.Read.All, ChannelMember.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | ChannelMember.Read.All, ChannelMember.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/channels/{channel-id}/doesUserHaveAccess
```

## <a name="function-parameters"></a>Параметры функции
В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.
В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.

|Параметр|Тип|Описание|
|:---|:---|:---|
|tenantId|String|Идентификатор клиента Azure Active Directory[, к которой](../resources/useridentity.md) принадлежит пользователь. Значением по умолчанию для этого свойства является **текущий идентификатор клиента** вошедвшего пользователя или приложения.|
|userId|String|Уникальный идентификатор [пользователя](../resources/useridentity.md). Укажите **userId или** **свойство userPrincipalName** в запросе.|
|userPrincipalName|String|Имя участника-пользователя (UPN) [пользователя](../resources/useridentity.md). Укажите **userId или** **свойство userPrincipalName** в запросе.|


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не предоставляйте текст запроса для этой функции.

## <a name="response"></a>Отклик

В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-check-access-for-an-internal-user"></a>Пример 1. Проверка доступа для внутреннего пользователя

Ниже приведен пример запроса, который проверяет, имеет ли внутренний пользователь доступ к общему каналу.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userId='6285581g-484b-4845-9e01-60667f8b12ae')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```


### <a name="example-2-check-access-for-an-external-user"></a>Пример 2. Проверка доступа для внешнего пользователя

Ниже приведен пример запроса, который использует свойство **tenantId** для проверки наличия у внешнего пользователя доступа к общему каналу.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess_externaluser"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userId='62855810-484b-4823-9e01-60667f8b12ae', tenantId='57fb72d0-d811-46f4-8947-305e6072eaa5')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-externaluser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-externaluser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-externaluser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-externaluser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```


### <a name="example-3-check-user-access-for-a-user-using-the-user-principal-name"></a>Пример 3. Проверка доступа пользователя с помощью имени участника-пользователя

Ниже приведен пример запроса, который использует свойство **userPrincipalName** для проверки того, имеет ли внутренний пользователь доступ к общему каналу.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel_doesuserhaveaccess_usingupn"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userPrincipalName='john.doe@contoso.com')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-doesuserhaveaccess-usingupn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-doesuserhaveaccess-usingupn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-doesuserhaveaccess-usingupn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-doesuserhaveaccess-usingupn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": false
}
```

