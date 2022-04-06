---
title: List servicePrincipalRiskDetections
description: Извлечение свойств коллекции объектов servicePrincipalRiskDetection.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d9fc67aa8a0b8db0efd2db016392b790e43ebfe3
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510346"
---
# <a name="list-serviceprincipalriskdetections"></a>List servicePrincipalRiskDetections
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение свойств коллекции объектов [servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) .

>**Примечание:** Для использования API servicePrincipalRiskDetection необходимо иметь лицензию Azure AD Premium P1 или P2.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|IdentityRiskEvent.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|IdentityRiskEvent.Read.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/servicePrincipalRiskDetections
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$filter` `$select` запроса oData и OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы этот метод возвращает код отклика и коллекцию объектов [servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-list-risk-detections"></a>Пример 1. Список обнаружения рисков

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipalriskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/servicePrincipalRiskDetections
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipalriskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipalriskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipalriskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipalriskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-serviceprincipalriskdetection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.servicePrincipalRiskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
    "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
    "id": "2856d6e87c5c3a74021ff70291fa68107570c150d8dc145bdea5",
    "requestId": null,
    "correlationId": null,
    "riskEventType": "investigationsThreatIntelligence",
    "riskState": "atRisk",
    "riskLevel": "high",
    "riskDetail": "none",
    "source": "IdentityProtection",
    "detectionTimingType": "offline",
    "activity": "servicePrincipal",
    "tokenIssuerType": "AzureAD",
    "ipAddress": null,
    "location": null,
    "activityDateTime": "2021-10-26T00:00:00Z",
    "detectedDateTime": "2021-10-26T00:00:00Z",
    "lastUpdatedDateTime": "2021-10-26T16:28:17.8202975Z)",
    "servicePrincipalId": "99b8d28b-11ae-4e84-9bef-0e767e286grg",
    "servicePrincipalDisplayName": "Contoso App",
    "appId": "0grb38ac-a572-491d-a9db-b07197643457",
    "keyIds": [
      "9d9fea30-d8e3-481b-b57c-0ef569a989e5"
    ],
    "additionalInfo": "[{\"Key\":\"alertUrl\",\"Value\":null}]"
    }
  ]
}
```

### <a name="example-2-list-risk-detections-and-filter-the-results"></a>Пример 2. Список обнаружения рисков и фильтрация результатов

#### <a name="request"></a>Запрос
В следующем примере `$filter` `medium` показано, как использовать для получения коллекции основных обнаружений рисков службы, где находится уровень риска или тип события риска `investigationsThreatIntelligence`.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_serviceprincipalriskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/servicePrincipalRiskDetections?$filter=riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-serviceprincipalriskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-serviceprincipalriskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-serviceprincipalriskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-serviceprincipalriskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-filter-serviceprincipalriskdetection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.servicePrincipalRiskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
    "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
    "id": "2856d6e87c5c3a74021ff70291fa68107570c150d8dc145bdea5",
    "requestId": null,
    "correlationId": null,
    "riskEventType": "investigationsThreatIntelligence",
    "riskState": "atRisk",
    "riskLevel": "high",
    "riskDetail": "none",
    "source": "IdentityProtection",
    "detectionTimingType": "offline",
    "activity": "servicePrincipal",
    "tokenIssuerType": "AzureAD",
    "ipAddress": null,
    "location": null,
    "activityDateTime": "2021-10-26T00:00:00Z",
    "detectedDateTime": "2021-10-26T00:00:00Z",
    "lastUpdatedDateTime": "2021-10-26T16:28:17.8202975Z)",
    "servicePrincipalId": "99b8d28b-11ae-4e84-9bef-0e767e286grg",
    "servicePrincipalDisplayName": "Contoso App",
    "appId": "0grb38ac-a572-491d-a9db-b07197643457",
    "keyIds": [
      "9d9fea30-d8e3-481b-b57c-0ef569a989e5"
    ],
    "additionalInfo": "[{\"Key\":\"alertUrl\",\"Value\":null}]"
    }
  ]
}
```
