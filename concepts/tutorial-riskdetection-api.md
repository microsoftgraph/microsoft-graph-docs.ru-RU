---
title: Учебник. Определение и устранение рисков с помощью API Microsoft Graph
description: Узнайте, как выявлять и устранять риски с помощью API Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0bec8dc51c81b9d2d0349294c0f0d1f6bd4c1e98
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664195"
---
# <a name="tutorial-identify-and-remediate-risks-using-microsoft-graph-apis"></a>Учебник. Определение и устранение рисков с помощью API Microsoft Graph

Защита идентификации Azure AD предоставляет организациям представление о риске на основе удостоверений и различных способах изучения и автоматического устранения риска. API защиты идентификации, используемые в этом руководстве, помогут вам определить риск и настроить рабочий процесс для подтверждения компрометации или устранения. Дополнительные сведения см. [в этой теме.](/azure/active-directory/identity-protection/concept-identity-protection-risks)

В этом руководстве вы узнаете, как создать рискованный пользователь и как устранять его рискованный статус с помощью политики условного доступа, которая требует многофакторной проверки подлинности (MFA). В дополнительном разделе показано, как заблокировать для пользователя вход с помощью политики условного доступа и снизить риск для пользователя.

>**Примечание.** Объекты ответа, показанные в этом руководстве, могут быть сокращены для учитаемости. 

## <a name="prerequisites"></a>Предварительные условия

Чтобы успешно выполнить это руководство, убедитесь, что у вас есть необходимые условия:

- Для использования API обнаружения рисков у вас должна быть лицензия Azure AD Premium P1 или P2.
- В этом руководстве используется браузер tor для анонимного вход на портал Azure. Для выполнения задачи можно использовать любой анонимный браузер. Чтобы скачать браузер tor, см. ["Скачать браузер tor".](https://www.torproject.org/download/)
- В этом руководстве предполагается, что вы используете проводник Microsoft Graph, но можете использовать Postman или создать собственное клиентские приложения для вызова Microsoft Graph. Чтобы вызвать API Microsoft Graph в этом руководстве, необходимо использовать учетную запись с ролью глобального администратора и соответствующими разрешениями. Чтобы настроить разрешения в проводнике Microsoft Graph, выполните следующие действия.
    1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
    2. Выберите **вход с помощью Майкрософт** и во входе с помощью учетной записи глобального администратора Azure AD. После успешного входе вы можете увидеть сведения об учетной записи пользователя в области слева.
    3. Выберите значок параметров справа от сведений учетной записи пользователя, а затем выберите **"Выбор разрешений".**

        ![Установка разрешений](./images/tutorial-riskdetection-api/set-permissions.png)
        
    4. Прокрутите список разрешений для этих разрешений:
        - **IdentityRiskEvents (2)**, развернуть и выбрать `IdentityRiskEvent.Read.All`
        - **IdentityRiskyUser (2)**, развернуть и выбрать `IdentityRiskyUser.ReadWrite.All`
        - **Политика (13),** развернуть, а затем выбрать `Policy.Read.All` и `Policy.ReadWrite.ConditionalAccess`
        - **Пользователь (8),** раз развернуть и выбрать `User.ReadWrite.All`
        
        ![Поиск разрешений](./images/tutorial-riskdetection-api/permissions-consent.png)
    
    5. Выберите **"Согласие",** а затем выберите **"Принять",** чтобы принять согласие на разрешения. Для получения этих разрешений не требуется согласие от имени вашей организации.

        ![Принятие разрешений](./images/tutorial-riskdetection-api/accept-permissions.png)

## <a name="step-1-create-a-user-account"></a>Шаг 1. Создание учетной записи пользователя

В этом руководстве вы создаете учетную запись пользователя, используемую для проверки обнаружения рисков. В теле запроса `contoso.com` измените доменное имя клиента. Сведения о клиенте можно найти на странице обзора Azure Active Directory.

### <a name="request"></a>Запрос

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

### <a name="response"></a>Отклик

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

## <a name="step-2-trigger-a-risk-detection"></a>Шаг 2. Запуск обнаружения рисков

### <a name="trigger-a-risk-detection"></a>Запуск обнаружения рисков

Один из способов обнаружения рисков для учетной записи пользователя — анонимный вход на портал Azure. В этом руководстве браузер tor используется для анонимного входов. 

1. Откройте браузер и введите `portal.azure.com` адрес сайта.
2. Во sign in to the portal using the credentials for the **MyTestUser1** account that you previously created. Вам будет предложено изменить существующий пароль.

### <a name="list-risk-detections"></a>Список обнаружений рисков

Когда вы вошел на портал Azure с помощью анонимного браузера, было `anonymizedIPAddress` обнаружено событие риска. Параметр запроса можно использовать для получения только обнаружений рисков, связанных с учетной записью `$filter` **пользователя MyTestUser1.**

#### <a name="request"></a>Запрос

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>Отклик

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#riskDetections",
  "value": [
    {
      "id": "d52a631815aaa527bf642b196715da5cf0f35b6879204ea5b5c99b21bd4c16f4",
      "requestId": "06f7fd18-b8f1-407d-86a3-f6cbe3a4be00",
      "correlationId": "2a38abff-5701-4073-a81e-fd3aac09cba3",
      "riskType": "anonymizedIPAddress",
      "riskEventType": "anonymizedIPAddress",
      "riskState": "atRisk",
      "riskLevel": "medium",
      "riskDetail": "none",
      "source": "IdentityProtection",
      "detectionTimingType": "realtime",
      "activity": "signin",
      "tokenIssuerType": "AzureAD",
      "ipAddress": "178.17.170.23",
      "activityDateTime": "2020-11-03T20:51:34.6245276Z",
      "detectedDateTime": "2020-11-03T20:51:34.6245276Z",
      "lastUpdatedDateTime": "2020-11-03T20:53:12.1984203Z",
      "userId": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com",
      "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
      "location": {
        "city": "Chisinau",
        "state": "Chisinau",
        "countryOrRegion": "MD",
        "geoCoordinates": {
          "latitude": 47.0269,
          "longitude": 28.8416
        }
      }
    }
  ]
}
```

> **Примечание.** Для возврата события может потребоваться несколько минут.

## <a name="step-3-create-a-conditional-access-policy"></a>Шаг 3. Создание политики условного доступа

Вы можете использовать политики условного доступа в организации, чтобы позволить пользователям самостоятельно устранять угрозы при обнаружении риска. Самостоятельное исправление позволяет пользователям разблокировать себя для безопасного доступа к своим ресурсам после выполнения запроса политики. На этом этапе создается политика условного доступа, которая требует, чтобы пользователь вошел с помощью MFA, если обнаружен средний или высокий риск.

### <a name="set-up-multi-factor-authentication"></a>Настройка многофакторной проверки подлинности

При настройке учетной записи для MFA можно выбрать один из нескольких способов проверки подлинности пользователя. Выберите лучший способ для вашей ситуации, чтобы завершить это руководство. 

1. Во sign in to the [keep your account secure](https://aka.ms/MFASetup) site using the **MyTestUser1** account.
2. Выполните процедуру настройки MFA, используя соответствующий метод для вашей ситуации, например, отправив на телефон текстовое сообщение.

### <a name="create-the-conditional-access-policy"></a>Создание политики условного доступа

Политика условного доступа позволяет устанавливать условия политики для определения уровней риска для входов. Уровни риска: `low` `medium` , , `high` `none` . В ответе, возвращенном из списка обнаружений рисков для **MyTestUser1,** мы видим, что уровень риска составляет `medium` . В этом примере показано, как требовать MFA для **MyTestUser1,** который был определен как рискованный пользователь.

#### <a name="request"></a>Запрос 

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies 
Content-type: application/json
 
{ 
  "displayName": "Policy for risky sign-in", 
  "state": "enabled", 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "applications": { 
      "includeApplications": ["All"]
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ] 
  } 
} 
```

#### <a name="response"></a>Отклик 

```
{ 
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity", 
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8", 
  "displayName": "Policy for risky sign-in", 
  "createdDateTime": "2020-11-03T20:56:38.6210843Z", 
  "modifiedDateTime": null, 
  "state": "enabled", 
  "sessionControls": null, 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "clientAppTypes": [  
      "all"  
    ], 
    "platforms": null, 
    "locations": null, 
    "applications": { 
      "includeApplications": [ 
        "All" 
      ], 
      "excludeApplications": [], 
      "includeUserActions": [] 
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ], 
      "excludeUsers": [], 
      "includeGroups": [], 
      "excludeGroups": [], 
      "includeRoles": [], 
      "excludeRoles": [] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ], 
    "customAuthenticationFactors": [], 
    "termsOfUse": [] 
  } 
} 
```

После применения этой политики условного доступа учетная запись **MyTestUser1** теперь необходима для использования MFA при входе, так как уровень риска для входов средний или   высокий. 

### <a name="sign-in-and-complete-multi-factor-authentication"></a>Вход и завершение многофакторной проверки подлинности 

При входе в анонимный браузер обнаруживается риск, но он устраняется с помощью MFA. 

1. Откройте браузер и введите  `portal.azure.com`   адрес сайта. 
2. Во sign in to the portal using the credentials for the **MyTestUser1**   account and complete the MFA process. 

### <a name="list-risk-detections"></a>Список обнаружений рисков

Так как MFA завершен. Теперь при составлении списка обнаружений рисков **событие riskState** показывается как `remediated` .

#### <a name="request"></a>Запрос

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>Отклик

```http
{
  "id": "ba9d45f16d8f87f6ae974efda7336b2120962a398cb362dfd9e5bdc8e9d149d0",
  "requestId": "156c01fb-31cf-4a10-b9a9-beee93e6a400",
  "correlationId": "a8aaac45-fe22-46df-babf-10a8dba85d62",
  "riskType": "anonymizedIPAddress",
  "riskEventType": "anonymizedIPAddress",
  "riskState": "remediated",
  "riskLevel": "medium",
  "riskDetail": "userPassedMFADrivenByRiskBasedPolicy",
  "source": "IdentityProtection",
  "detectionTimingType": "realtime",
  "activity": "signin",
  "tokenIssuerType": "AzureAD",
  "ipAddress": "185.220.101.213",
  "activityDateTime": "2020-11-12T23:45:22.4092789Z",
  "detectedDateTime": "2020-11-12T23:45:22.4092789Z",
  "lastUpdatedDateTime": "2020-11-12T23:47:57.7831423Z",
  "userId": "4b608561-9258-44ba-8cdb-3286dcbf0e3b",
  "userDisplayName": "MyTestUser1",
  "userPrincipalName": "MyTestUser1@contoso.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
  "location": {
    "city": "Schoenwalde-Glien",
    "state": "Brandenburg",
    "countryOrRegion": "DE",
    "geoCoordinates": {
      "latitude": 52.61983,
      "longitude": 13.12743
    }
  }
}
```

## <a name="step-4-optional-block-the-user-from-signing-in"></a>Шаг 4 (необязательно) Блокировка пользователя при входе

Вместо того чтобы предоставлять пользователю возможность самостоятельного устранения, можно заблокировать вход пользователя. На этом этапе создается новая политика условного доступа, которая блокирует вход пользователя в случае обнаружения среднего или высокого риска. Разница в политиках заключается в том, **что для builtInControls** установлено значение `block` .

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
  "displayName": "Policy for risky sign-in block access",
  "state": "enabled",
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "applications": {
      "includeApplications": ["All"]
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ]
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ]
  }
}
```

### <a name="response"></a>Отклик

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity",
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8",
  "displayName": "Policy for risky sign-in block access",
  "createdDateTime": "2020-11-03T20:56:38.6210843Z",
  "modifiedDateTime": null,
  "state": "enabled",
  "sessionControls": null,
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "clientAppTypes": [ 
      "all" 
    ],
    "platforms": null,
    "locations": null,
    "applications": {
      "includeApplications": [
        "All"
      ],
      "excludeApplications": [],
      "includeUserActions": []
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ],
      "excludeUsers": [],
      "includeGroups": [],
      "excludeGroups": [],
      "includeRoles": [],
      "excludeRoles": []
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ],
    "customAuthenticationFactors": [],
    "termsOfUse": []
  }
}
```

После данной политики условного доступа учетная запись **MyTestUser1** не может войти в нее, так как уровень риска для входов `medium` составляет или `high` .

![Заблокированный вход](./images/tutorial-riskdetection-api/conditionalaccess-policy.png)

## <a name="step-5-dismiss-risky-users"></a>Шаг 5. Отклонение рискованных пользователей

Если вы считаете, что пользователь не находится под угрозой и не хотите применять политику условного доступа, вы можете вручную отклонять этого пользователя.

### <a name="dismiss-the-risky-user"></a>Отклонение рискованных пользователей

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "4628e7df-dff3-407c-a08f-75f08c0806dc"
  ]
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No Content
```        

### <a name="list-risky-users"></a>Список рискованных пользователей

После того как пользователь с риском будет отклонен, вы увидите в ответе список рискованных пользователей, для учетной записи **пользователя MyTestUser1** теперь есть уровень риска и уровень `none` риска . `dismissed`

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>Отклик

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "isDeleted": false,
      "isProcessing": false,
      "riskLevel": "none",
      "riskState": "dismissed",
      "riskDetail": "adminDismissedAllRiskForUser",
      "riskLastUpdatedDateTime": "2020-11-03T21:48:53.4298425Z",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com"
    }
  ]
}
```

## <a name="step-6-clean-up-resources"></a>Шаг 6. Очистка ресурсов

На этом этапе удаляются созданные ресурсы.

### <a name="delete-the-user-account"></a>Удаление учетной записи пользователя

Удалите **учетную запись пользователя MyTestUser1.**

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/users/4628e7df-dff3-407c-a08f-75f08c0806dc
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

### <a name="delete-the-conditional-access-policy"></a>Удаление политики условного доступа

Удалите созданную политику условного доступа.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/groups/9ad78153-b1f8-4714-adc1-1445727678a8
```

#### <a name="response"></a>Отклик

```http
No Content - 204
```

## <a name="see-also"></a>См. также

В этом руководстве вы использовали множество API для выполнения задач. Изучите справочник по API для этих API, чтобы узнать больше о том, что могут делать API.

- [Что такое защита идентификации?](/azure/active-directory/identity-protection/overview-identity-protection)
- [Что такое условный доступ?](/azure/active-directory/conditional-access/overview)
- [Как это работает: многофакторная проверка подлинности Azure](/azure/active-directory/authentication/concept-mfa-howitworks)
- [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-1.0)
- [riskDetection](/graph/api/resources/riskdetection?view=graph-rest-1.0)
- [riskyUser](/graph/api/resources/riskyuser?view=graph-rest-1.0)
- [user](/graph/api/resources/user?view=graph-rest-1.0)