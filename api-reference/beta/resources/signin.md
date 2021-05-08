---
title: Тип ресурса signIn
doc_type: resourcePageType
description: Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге.
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
ms.openlocfilehash: c16e0b6752bc8bc9498eb269a1c225c5947ecbd6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240681"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге. Для загрузки журналов входа с помощью API microsoft Premium AD Premium или P Graph 2.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Считывание свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alternateSignInName|Строка|Альтернативный идентификатор регистрации при использовании номера телефона для регистрации. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|appDisplayName|String|Имя приложения, отображаемая на портале Azure. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|appId|String|Идентификатор приложения в Azure Active Directory. Поддерживает `$filter` `eq` (только оператор).|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection|Список политик условного доступа, которые вызываются соответствующей активностью регистрации.|
|authenticationDetails|[коллекция authenticationDetail](authenticationdetail.md)|Результат попытки проверки подлинности и дополнительные сведения о методе проверки подлинности.|
|authenticationMethodsUsed|Коллекция объектов string|Используемые методы проверки подлинности. Возможные значения: `SMS` , , , , , , или `Authenticator App` `App Verification code` `Password` `FIDO` `PTA` `PHS` .|
|authenticationProcessingDetails|Коллекция [keyValue](keyvalue.md)|Дополнительные сведения об обработке проверки подлинности, например имя агента в случае PTA/PHS или имени Server/farm в случае федератированной проверки подлинности.|
|authenticationRequirement | Строка | Это имеет наивысший уровень проверки подлинности, необходимой для успешной регистрации при входе. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|clientAppUsed|String|Устаревший клиент, используемый для действий по входу. Например: `Browser` `Exchange Active Sync` , `Modern clients` , , , `IMAP` , , `MAPI` или `SMTP` `POP` . Поддерживает `$filter` `eq` (только оператор). |
|conditionalAccessStatus|conditionalAccessStatus| Состояние срабатывуемой политики условного доступа. Возможные значения: `success` `failure` , , или `notApplied` `unknownFutureValue` . Поддерживает `$filter` `eq` (только оператор).|
|correlationId|String|Идентификатор, который отправляется от клиента при входе. Это используется для устранения неполадок соответствующей активности регистрации при вызове поддержки. Поддерживает `$filter` `eq` (только оператор).|
|createdDateTime|DateTimeOffset|Дата и время начала регистрации. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$orderby` и `$filter` `eq` `le` (и только `ge` операторов).|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, откуда произошла входная информация. Включает такие сведения, как deviceId, OS и браузер. Поддерживает `$filter` `eq` (и `startsWith` только операторы) в **свойствах браузера** **и operatingSytem.**|
|id|Строка|Идентификатор, представляющий действие входной записи. Поддерживает `$filter` `eq` (только оператор).|
|ipAddress|String|IP-адрес клиента, откуда произошла входная. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|isInteractive|Boolean|Указывает, является ли вход интерактивным или нет.|
|location|[signInLocation](signinlocation.md)|Код страны города, состояния и 2 буквы, откуда произошла входная. Поддерживает (и только операторов) в свойствах `$filter` `eq` `startsWith` **city,** **state** и **countryOrRegion.**|
|networkLocationDetails|Коллекция [networkLocationDetail](networklocationdetail.md)|Сведения о расположении сети, включая тип используемой сети и ее имена.|
|originalRequestId|String|Идентификатор первого запроса в последовательности проверки подлинности. Поддерживает `$filter` `eq` (только оператор).|
|processingTimeInMilliseconds|Int|Время обработки запроса в миллисекунде в AD STS.|
|resourceDisplayName|Строка|Имя ресурса, на который пользователь подписался. Поддерживает `$filter` `eq` (только оператор).|
|resourceId|String|Идентификатор ресурса, на который пользователь подписался. Поддерживает `$filter` `eq` (только оператор).|
|riskDetail|riskDetail|Причина определенного состояния рискованного пользователя, вход или событие риска. Возможные значения: `none` , , , , , , , , `adminGeneratedTemporaryPassword` или `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` . Значение `none` означает, что действия для пользователя или входа пока не выполнялись. Поддерживает `$filter` `eq` (только оператор).<br> **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskEventTypes|коллекция riskEventType|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` , , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` . Поддерживает `$filter` `eq` (только оператор).|
|riskEventTypes_v2|Коллекция объектов string|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` , , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` . Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|riskLevelAggregated|riskLevel|Совокупный уровень риска. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. Поддерживает `$filter` `eq` (только оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskLevelDuringSignIn|riskLevel|Уровень риска при входе. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. Поддерживает `$filter` `eq` (только оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Все остальные клиенты `hidden` возвращаются.|
|riskState|riskState|Состояние риска для рискованного пользователя, вход или событие риска. Возможные значения: `none` , , , , , , или `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` `unknownFutureValue` . Поддерживает `$filter` `eq` (только оператор).|
|servicePrincipalId|Строка|Идентификатор приложения, используемый для регистрации. Это поле заполняется при входе в приложение. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|servicePrincipalName|String|Имя приложения, используемого для регистрации. Это поле заполняется при входе в приложение. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|status|[signInStatus](signinstatus.md)|Состояние входного знака. Включает код ошибки и описание ошибки (в случае сбоя при входе). Поддерживает `$filter` `eq` (только оператор) в **свойстве errorCode.**|
|tokenIssuerName|String|Имя поставщика удостоверений. Например, `sts.microsoft.com`. Поддерживает `$filter` `eq` (только оператор).|
|tokenIssuerType|tokenIssuerType|Тип поставщика удостоверений. Возможные значения: `AzureAD` `ADFederationServices` , или `UnknownFutureValue` .|
|userAgent|Строка|Сведения агента пользователя, относящиеся к входу. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|userDisplayName|String|Отображаемое имя пользователя. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|userId|String|Идентификатор пользователя. Поддерживает `$filter` `eq` (только оператор).|
|userPrincipalName|String|UpN пользователя. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|

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


