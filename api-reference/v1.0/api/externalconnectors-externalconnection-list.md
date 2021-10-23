---
title: Список externalConnections
description: Получите список объектов externalConnection и их свойств.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 95d37bae58b81d7b6f19ce38e9203844e0f50c17
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560004"
---
# <a name="list-externalconnections"></a>Список externalConnections
Пространство имен: microsoft.graph.externalConnectors



Получите список объектов [externalConnection](../resources/externalconnectors-externalconnection.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Неприменимо|
|Делегированные (личная учетная запись Майкрософт)|Неприменимо|
|Application| ExternalConnection.ReadWrite.OwnedBy|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /external/connections
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов externalConnection](../resources/externalconnectors-externalconnection.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "list_externalconnection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/external/connections
```



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.externalConnectors.externalConnection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    }
  ]
}
```

