---
title: Перечисление симуляций
description: Получение списка кампаний моделирования атак для клиента.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d1ee63b72436f74e44d9e416c20b2c1c40b36b57
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203591"
---
# <a name="list-simulations"></a>Перечисление симуляций
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка кампаний моделирования атак для клиента.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | SecurityEvents.Read.All                     |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | SecurityEvents.Read.All                     |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает следующие параметры запроса OData для настройки ответа: , , , , , `$select``$top`. `$orderby``$skiptoken``$filter``$count`

Поддерживаются следующие свойства `$filter` `$orderby`: **attackTechnique**, **attackType**, **completionDateTime**, **displayName**, **isAutomated**, **launchDateTime**, **status**.

Используется `@odata.nextLink` для разбиения на страницы.

Ниже приведены примеры их использования.

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations?$count=true
GET /security/attackSimulation/simulations?$filter={property} eq '{property-value}'
GET /security/attackSimulation/simulations?$filter={property} eq '{property-value}'&$top=5
GET /security/attackSimulation/simulations?$orderby={property}
GET /security/attackSimulation/simulations?$top=1
GET /security/attackSimulation/simulations?$select={property}
```

Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [имитации](../resources/simulation.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_simulation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-simulation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-simulation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-simulation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-simulation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-simulation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-simulation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.simulation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "f1b13829-3829-f1b1-2938-b1f12938b1f1",
      "displayName": "Sample Simulation",
      "description": "Sample Simulation Description",
      "attackType": "social",
      "attackTechnique": "credentialHarvesting",
      "status": "scheduled",
      "createdDateTime": "2021-01-01T01:01:01.01Z",
      "createdBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      },
      "lastModifiedDateTime": "2021-01-01T01:01:01.01Z",
      "lastModifiedBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      },
      "launchDateTime": "2021-01-01T02:01:01.01Z",
      "completionDateTime": "2021-01-07T01:01:01.01Z",
      "isAutomated": false,
      "automationId": "f1b13829-3829-f1b1-2938-b1f12938b1ab",
      "payloadDeliveryPlatform": "email"
    }
  ]
}
```

