---
title: Получение объекта signIn
doc_type: apiPageType
description: Получите объект signIn, содержащий все входы для Azure Active Directory клиента.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: 7a7b336a0c949141516e63e0e13bc13318ef70d8
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647150"
---
# <a name="get-signin"></a>Получение объекта signIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите [объект signIn,](../resources/signin.md) содержащий определенное событие для регистрации пользователя для клиента. Это включает входы, в которых пользователю будет предложено ввести имя пользователя или пароль, а также маркеры сеанса.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | AuditLog.Read.All и Directory.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
| Для приложений | AuditLog.Read.All и Directory.Read.All | 

> [!IMPORTANT]
> Этот API имеет [известные](/graph//graph/known-issues#license-check-errors-for-azure-ad-activity-reports) проблемы и в настоящее время требует согласия на оба **auditLog.Read.All** и **Directory.Read.All** разрешений.

Приложения должны быть [правильно зарегистрированы в](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD.

Помимо делегирования разрешений, пользователю, входиму в который, необходимо принадлежать к одной из следующих ролей каталога, которая позволяет ему читать отчеты о входе. Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)
+ Глобальный администратор
+ Глобальный читатель
+ Читатель отчетов
+ Администратор безопасности
+ Оператор безопасности
+ Читатель сведений о безопасности

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки ответа. Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Authorization | Bearer {token} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект signIn](../resources/signin.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signin-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"66ea54eb-blah-4ee5-be62-ff5a759b0100",
  "createdDateTime":"2021-06-30T16:34:32Z",
  "userDisplayName":"Test contoso",
  "userPrincipalName":"testaccount1@contoso.com",
  "userId":"26be570a-1111-5555-b4e2-a37c6808512d",
  "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
  "appDisplayName":"Azure Portal",
  "authenticationProtocol": "oAuth2",
  "incomingTokenType": "Primary Refresh Token",
  "ipAddress":"131.107.159.37",
  "clientAppUsed":"Browser",
  "userAgent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36 Edg/91.0.864.54",
  "correlationId":"5d295068-919b-4017-85d8-44be2f5f5483",
  "conditionalAccessStatus":"notApplied",
  "originalRequestId":"7dccb0d7-1041-4d82-b785-d865272e1400",
  "homeTenantId": "4f7a7bc2-28e2-46a3-b90e-5ade5bc90138",
  "homeTenantName": "",
  "isTenantRestricted": false,
  "isInteractive":true,
  "tokenIssuerName":"",
  "tokenIssuerType":"AzureAD",
  "processingTimeInMilliseconds":761,
  "riskDetail":"none",
  "riskLevelAggregated":"none",
  "riskLevelDuringSignIn":"none",
  "riskState":"none",
  "riskEventTypes_v2":[],
  "resourceDisplayName":"Windows Azure Service Management API",
  "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
  "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
  "resourceTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
  "homeTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
  "authenticationMethodsUsed":[],
  "authenticationRequirement":"singleFactorAuthentication",
  "signInIdentifier":"testaccount1@contoso.com",
  "signInEventTypes":["interactiveUser"],
  "servicePrincipalId":"",
  "userType":"member",
  "flaggedForReview":false,
  "isTenantRestricted":false,
  "autonomousSystemNumber":3598,
  "crossTenantAccessType":"none",
  "status":{
      "errorCode":50126,
      "failureReason":"Error validating credentials due to invalid username or password.",
      "additionalDetails":"The user didn't enter the right credentials. \u00a0It's expected to see some number of these errors in your logs due to users making mistakes."
    },
  "deviceDetail":{
      "deviceId":"",
      "displayName":"",
      "operatingSystem":"Windows 10",
      "browser":"Edge 91.0.864",
      "isCompliant":false,
      "isManaged":false,
      "trustType":""
    },
  "location":{
      "city":"Redmond",
      "state":"Washington",
      "countryOrRegion":"US",
      "geoCoordinates":{
        "altitude":null,
        "latitude":47.6807,
        "longitude":-122.1231
      }
    },
  "appliedConditionalAccessPolicies":[],
  "authenticationProcessingDetails":[
      {
        "key":"Login Hint Present",
        "value":"True"
      }
    ],
  "networkLocationDetails":[
      {
        "networkType":"namedNetwork",
        "networkNames":["North America"]
      }
    ],
  "authenticationDetails":[
      {
        "authenticationStepDateTime":"2021-06-30T16:34:32Z",
        "authenticationMethod":"Password",
        "authenticationMethodDetail":"Password in the cloud",
        "succeeded":false,
        "authenticationStepResultDetail":"Invalid username or password or Invalid on-premise username or password.",
        "authenticationStepRequirement":"Primary authentication"
      }
    ],
  "authenticationRequirementPolicies":[],
  "sessionLifetimePolicies":[]
}
```
