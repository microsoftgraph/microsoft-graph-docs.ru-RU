---
title: Получение подключения
description: Получение свойств и связей внешнего соединения.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ea800fc1b154b61f70e3573110ef980bf8ef278b
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629337"
---
# <a name="get-connection"></a>Получение подключения

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей [внешнего соединения](../resources/externalconnectors-externalconnection.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | ExternalConnection.ReadWrite.OwnedBy, ExternalConnection.Read.All, ExternalConnection.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | ExternalConnection.ReadWrite.OwnedBy, ExternalConnection.Read.All, ExternalConnection.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [externalConnection](../resources/externalconnectors-externalconnection.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-connection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-connection-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contosohr",
  "ingestedItemsCount": 700000,
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "state": "ready",
  "configuration": {
    "authorizedAppIds": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
