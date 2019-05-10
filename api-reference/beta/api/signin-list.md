---
title: Перечисление входов
description: Описан метод перечисления ресурсов signIn (объектов) из API Microsoft Graph API (REST), что помогает при аудите действий в каталоге (клиенте) (бета-версия).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fdb1358d36a0e1da34779de5505c5f18f901e681
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638685"
---
# <a name="list-signins"></a>Перечисление входов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получает входы пользователей Azure AD для клиента. Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.  Последние входы возвращаются первыми.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AuditLog.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается   |
|Для приложений | AuditLog.Read.All | 

Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика. Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).

|Имя     |Описание                            |Пример|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|Фильтрует результаты (строки). |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|Задает размер страницы результатов.|`/auditLogs/signIns?$top=1`|
|[$skiptoken](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Список атрибутов, поддерживаемых параметром $filter
|Имя атрибута |Поддерживаемые операторы|
|:----------------|:------|
|id|eq|
|userId|eq|
|appId|eq|
|createdDateTime| eq, le, ge|
|userDisplayName| eq, startswith|
|userPrincipalName| eq, startswith|
|appDisplayName| eq, startswith|
|ipAddress| eq, startswith|
|location/city| eq, startswith|
|location/state| eq, startswith|
|location/countryOrRegion| eq, startswith|
|status/errorCode|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq, startswith|
|clientAppUsed| eq|
|conditionalAccessStatus | eq|
|deviceDetail/browser| eq, startswith|
|deviceDetail/operatingSystem| eq, startswith|
|correlationId| eq|
|riskDetail| eq|
|riskLevelAggregated| eq|
|riskLevelDuringSignIn| eq|
|riskEventTypes| eq|
|riskState| eq|
|originalRequestId| eq|
|tokenIssuerName| eq|
|tokenIssuerType| eq|
|resourceDisplayName| eq|
|resourceId| eq|


## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signins-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

        ]
        }
    
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
