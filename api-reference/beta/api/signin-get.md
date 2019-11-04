---
title: Получение объекта signIn
doc_type: apiPageType
description: Получение объекта SignIn, содержащего все входные сведения о клиенте Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ed96154c2104dc0b06ee24f01080203a8bb61b15
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938374"
---
# <a name="get-signin"></a>Получение объекта signIn

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объекта [SignIn](../resources/signin.md) , содержащего конкретное пользовательское событие входа для вашего клиента. Сюда входят входы, в которых пользователю предлагается ввести имя пользователя или пароль, а также маркеры сеансов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | Аудитлог. Read. ALL, Directory. Read. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
| Для приложений | Аудитлог. Read. ALL, Directory. Read. ALL | 

Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки ответа. Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [SignIn](../resources/signin.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a>Пример 1: пользователь подписывается с помощью MFA, который активируется политикой условного доступа. Основной способ проверки подлинности — Фидо.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [ 
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"FIDO2",
          "authenticationMethodDetail":"1G54395783",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        },
        {
          "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
          "authenticationMethod":"Claim in access token",
          "authenticationMethodDetail":null,
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"MFA"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"applied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a>Пример 2: пользователь входит только с основной проверкой подлинности. Первичная проверка подлинности осуществляется с помощью облачного пароля.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
