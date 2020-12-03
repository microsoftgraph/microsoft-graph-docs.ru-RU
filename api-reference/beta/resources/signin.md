---
title: Тип ресурса signIn
doc_type: resourcePageType
description: Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге.
author: besiler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 97a3c3807c4abe25594ad918b8717efad4ce7770
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563683"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге. 

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Считывание свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|алтернатесигниннаме|String|Альтернативное удостоверение входа при входе в систему с помощью номера телефона.|
|appDisplayName|String|Имя приложения отображается на портале Azure.|
|appId|String|Идентификатор приложения в Azure Active Directory.|
|апплиедкондитионалакцессполиЦиес|Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)|Список политик условного доступа, которые вызываются соответствующими действиями при входе.|
|аусентикатиондетаилс|Коллекция [аусентикатиондетаил](authenticationdetail.md)|Результат попытки проверки подлинности и дополнительные сведения о методе проверки подлинности.|
|authenticationMethodsUsed|Коллекция объектов string|Используемые методы проверки подлинности. Возможные значения: `SMS` , `Authenticator App` , `App Verification code` , `Password` , `FIDO` , `PTA` , или `PHS` .|
|аусентикатионпроцессингдетаилс|Коллекция [keyValue](keyvalue.md)|Дополнительные сведения об обработке проверки подлинности, такие как имя агента в случае ПТА/ФС или Server/ферма, в случае федеративной проверки подлинности.|
|аусентикатионрекуиремент | string | Этот параметр содержит самый высокий уровень проверки подлинности, необходимый для успешного входа.|
|clientAppUsed|String|Устаревший клиент, используемый для входных действий. Например, браузер, Exchange Active Sync, современные клиенты, IMAP, MAPI, SMTP или POP.|
|conditionalAccessStatus|string| Состояние политики условного доступа, инициированной. Возможные значения: `success` , `failure` , `notApplied` , или `unknownFutureValue` .|
|correlationId|String|Идентификатор, который отправляется клиентом при запуске входа. Используется для устранения неполадок с соответствующими действиями при входе в службу поддержки.|
|createdDateTime|DateTimeOffset|Дата и время инициирования входа. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, с которого произошел вход. Включает такие сведения, как deviceId, OS и Browser. |
|id|String|Идентификатор, представляющий действие по входу.|
|ipAddress|String|IP-адрес клиента, с которого произошел вход.|
|isInteractive|Boolean|Указывает, является ли вход в систему интерактивным или нет.|
|location|[signInLocation](signinlocation.md)|Код города, штата и 2 буквенного кода страны, из которого произошла вход.|
|networkLocationDetails|Коллекция [networkLocationDetail](networklocationdetail.md)|Сведения о сетевом расположении, такие как IP-адрес, расположение входа, тип используемой сети и ее имена. Возможные значения: `Named Netowrk` , `Extranet` , `Intranet` , или `Trusted Network` .|
|originalRequestId|String|Идентификатор запроса первого запроса в последовательности проверки подлинности.|
|processingTimeInMilliseconds|Int|Время обработки запроса в миллисекундах в службе маркеров безопасности (в миллисекундах).|
|resourceDisplayName|String|Имя ресурса, в который пользователь выполнил вход.|
|resourceId|String|Идентификатор ресурса, в который пользователь выполнил вход.|
|riskDetail|riskDetail|Причина определенного состояния опасного пользователя, входа в систему или события риска. Возможные значения: `none` ,,,,, `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` , `userPassedMFADrivenByRiskBasedPolicy` , `adminDismissedAllRiskForUser` , `adminConfirmedSigninCompromised` или `unknownFutureValue` . Значение `none` означает, что действия для пользователя или входа пока не выполнялись. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные клиенты `hidden` .|
|riskEventTypes|Коллекция Рискевенттипе|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` ,,,,, `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` , `leakedCredentials` , `investigationsThreatIntelligence` ,  `generic` или `unknownFutureValue` .|
|riskEventTypes_v2|Коллекция объектов string|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` ,,,,, `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` , `leakedCredentials` , `investigationsThreatIntelligence` ,  `generic` или `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|Сводный уровень риска. Возможные значения: `none` , `low` , `medium` , `high` , `hidden` , или `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные клиенты `hidden` .|
|riskLevelDuringSignIn|riskLevel|Уровень риска во время входа. Возможные значения: `none` , `low` , `medium` , `high` , `hidden` , или `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные клиенты `hidden` .|
|riskState|riskState|Состояние риска рискованного пользователя, входа в систему или события риска. Возможные значения: `none` , `confirmedSafe` , `remediated` , `dismissed` , `atRisk` , `confirmedCompromised` , или `unknownFutureValue` .|
|сервицепринЦипалид|String|Идентификатор приложения, используемый для входа в систему. Это поле заполняется при входе с использованием приложения.|
|servicePrincipalName|String|Имя приложения, используемое для входа в систему. Это поле заполняется при входе с использованием приложения.|
|status|[signInStatus](signinstatus.md)|Состояние входа. Содержит код ошибки и описание ошибки (в случае сбоя входа).|
|tokenIssuerName|String|Имя поставщика удостоверений. Например, `sts.microsoft.com`.|
|tokenIssuerType|String|Тип поставщика удостоверений. Возможные значения: `AzureAD` , `ADFederationServices` , или `UnknownFutureValue` .|
|userAgent|String|Сведения о агенте пользователя, связанные с входом.|
|userDisplayName|String|Отображаемое имя пользователя.|
|userId|String|Идентификатор пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|

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


