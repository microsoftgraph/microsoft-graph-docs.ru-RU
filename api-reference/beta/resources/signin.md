---
title: Тип ресурса signIn
doc_type: resourcePageType
description: Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге.
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
ms.openlocfilehash: affc874a27af4aa9037bf6f9b7a212dc33f75995
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955002"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге. Для загрузки журналов входа с помощью API Microsoft Graph необходимо иметь лицензию Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Считывание свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alternateSignInName|Строка|Альтернативный идентификатор регистрации при использовании номера телефона для регистрации.|
|appDisplayName|String|Имя приложения, отображаемая на портале Azure.|
|appId|String|Идентификатор приложения в Azure Active Directory.|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection|Список политик условного доступа, которые вызываются соответствующей активностью регистрации.|
|authenticationDetails|[коллекция authenticationDetail](authenticationdetail.md)|Результат попытки проверки подлинности и дополнительные сведения о методе проверки подлинности.|
|authenticationMethodsUsed|Коллекция строк|Используемые методы проверки подлинности. Возможные значения: `SMS` , , , , , , или `Authenticator App` `App Verification code` `Password` `FIDO` `PTA` `PHS` .|
|authenticationProcessingDetails|Коллекция [keyValue](keyvalue.md)|Дополнительные сведения об обработке проверки подлинности, например имя агента в случае PTA/PHS или имени Server/farm в случае федератированной проверки подлинности.|
|authenticationRequirement | Строка | Это имеет наивысший уровень проверки подлинности, необходимой для успешной регистрации при входе.|
|clientAppUsed|String|Устаревший клиент, используемый для действий по входу. Например: `Browser` `Exchange Active Sync` , `Modern clients` , , , `IMAP` , , `MAPI` или `SMTP` `POP` .|
|conditionalAccessStatus|conditionalAccessStatus| Состояние срабатывуемой политики условного доступа. Возможные значения: `success` `failure` , , или `notApplied` `unknownFutureValue` .|
|correlationId|String|Идентификатор, который отправляется от клиента при входе. Это используется для устранения неполадок соответствующей активности регистрации при вызове поддержки.|
|createdDateTime|DateTimeOffset|Дата и время начала регистрации. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, откуда произошла входная информация. Включает такие сведения, как deviceId, OS и браузер. |
|id|Строка|Идентификатор, представляющий действие входной записи.|
|ipAddress|String|IP-адрес клиента, откуда произошла входная.|
|isInteractive|Boolean|Указывает, является ли вход интерактивным или нет.|
|location|[signInLocation](signinlocation.md)|Код страны города, состояния и 2 буквы, откуда произошла входная.|
|networkLocationDetails|Коллекция [networkLocationDetail](networklocationdetail.md)|Сведения о расположении сети, включая тип используемой сети и ее имена.|
|originalRequestId|String|Идентификатор первого запроса в последовательности проверки подлинности.|
|processingTimeInMilliseconds|Int|Время обработки запроса в миллисекунде в AD STS.|
|resourceDisplayName|Строка|Имя ресурса, на который пользователь подписался.|
|resourceId|String|Идентификатор ресурса, на который пользователь подписался.|
|riskDetail|riskDetail|Причина определенного состояния рискованного пользователя, вход или событие риска. Возможные значения: `none` , , , , , , , , `adminGeneratedTemporaryPassword` или `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` . Значение `none` означает, что действия для пользователя или входа пока не выполнялись. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskEventTypes|коллекция riskEventType|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` , , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskEventTypes_v2|Коллекция строк|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` , , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|Совокупный уровень риска. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskLevelDuringSignIn|riskLevel|Уровень риска при входе. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskState|riskState|Состояние риска для рискованного пользователя, вход или событие риска. Возможные значения: `none` , , , , , , или `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` `unknownFutureValue` .|
|servicePrincipalId|Строка|Идентификатор приложения, используемый для регистрации. Это поле заполняется при входе в приложение.|
|servicePrincipalName|String|Имя приложения, используемого для регистрации. Это поле заполняется при входе в приложение.|
|status|[signInStatus](signinstatus.md)|Состояние входного знака. Включает код ошибки и описание ошибки (в случае сбоя при входе).|
|tokenIssuerName|String|Имя поставщика удостоверений. Например, `sts.microsoft.com`.|
|tokenIssuerType|tokenIssuerType|Тип поставщика удостоверений. Возможные значения: `AzureAD` `ADFederationServices` , или `UnknownFutureValue` .|
|userAgent|Строка|Сведения агента пользователя, относящиеся к входу.|
|userDisplayName|String|Отображаемое имя пользователя.|
|userId|String|Идентификатор пользователя.|
|userPrincipalName|String|UpN пользователя.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signIn"
}-->

```json
{
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "authenticationDetails": [{"@odata.type": "microsoft.graph.authenticationDetail"}],
  "authenticationMethodsUsed": ["String"],
  "authenticationProcessingDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "string",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "id": "String (identifier)",
  "ipAddress": "String",
  "isInteractive": true,
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": 1024,
  "resourceDisplayName": "String",
  "resourceId": "String",
  "riskDetail": "string",
  "riskEventTypes": ["string"],
  "riskEventTypes_v2": ["String"],
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "tokenIssuerName": "String",
  "tokenIssuerType": "string",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


