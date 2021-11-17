---
title: Get identityApiConnector
description: Ознакомьтесь с свойствами соединитетеля API.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fbd079976a64c89c9fa7bb8bea5221ecab25c6c5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027683"
---
# <a name="get-identityapiconnector"></a>Get identityApiConnector

Пространство имен: microsoft.graph

Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | APIConnectors.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.  |
| Для приложений                            | APIConnectors.ReadWrite.All |

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор внешних Flow удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Вы можете использовать `$expand` для расширения определенных свойств, которые не расширяются по умолчанию. Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityapiconnector"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-identityapiconnector-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"370eeb68-dfd3-4a47-8160-8824c2358321",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
