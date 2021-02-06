---
title: Тип ресурса signIn
doc_type: resourcePageType
description: Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге.
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
ms.openlocfilehash: 6d5c8680d93c5fd480efae9c3f11bcbe4475e05b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133049"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о входе пользователей или входе в приложения в вашем каталоге. Для скачивания журналов входа с помощью API Microsoft Graph вам требуется лицензия Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Считывание свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alternateSignInName|Строка|Альтернативное удостоверение для регистрации при использовании номера телефона для регистрации.|
|appDisplayName|String|Имя приложения, отображаемая на портале Azure.|
|appId|String|Идентификатор приложения в Azure Active Directory.|
|appliedConditionalAccessPolicies|Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)|Список политик условного доступа, запускаемого соответствующей активностью при входе.|
|authenticationDetails|[Коллекция authenticationDetail](authenticationdetail.md)|Результат попытки проверки подлинности и дополнительные сведения о методе проверки подлинности.|
|authenticationMethodsUsed|Коллекция объектов string|Используемые методы проверки подлинности. Возможные значения: `SMS` , , , , , , или `Authenticator App` `App Verification code` `Password` `FIDO` `PTA` `PHS` .|
|authenticationProcessingDetails|Коллекция [keyValue](keyvalue.md)|Дополнительные сведения об обработке проверки подлинности, например имя агента в случае имени PTA/PHS или сервера или фермы в случае федерационной проверки подлинности.|
|authenticationRequirement | string | Это самый высокий уровень проверки подлинности, необходимый для успешного регистрации при входе.|
|clientAppUsed|String|Устаревший клиент, используемый для действий при входе. Например, Browser, Exchange Active Sync, современные клиенты, IMAP, MAPI, SMTP или POP.|
|conditionalAccessStatus|string| Состояние срабатывуемой политики условного доступа. Возможные значения: `success` , , , или `failure` `notApplied` `unknownFutureValue` .|
|correlationId|String|Идентификатор, который отправляется клиентом при инициале регистрации. Это используется для устранения неполадок с соответствующими действиями при входе в службу поддержки.|
|createdDateTime|DateTimeOffset|Дата и время запуска регистрации. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, с которых произошел вход. Включает такие сведения, как deviceId, ОС и браузер. |
|id|Строка|Идентификатор, представляющий действие при входе.|
|ipAddress|String|IP-адрес клиента, с которой произошел вход.|
|isInteractive|Boolean|Указывает, является ли вход интерактивным.|
|location|[signInLocation](signinlocation.md)|Город, штат и 2 буквы кода страны, из которых был совершен вход.|
|networkLocationDetails|Коллекция [networkLocationDetail](networklocationdetail.md)|Сведения о сетевом расположении, например IP-адрес, расположение для регистрации, тип используемой сети и ее имена. Возможные значения: `Named Netowrk` , , , или `Extranet` `Intranet` `Trusted Network` .|
|originalRequestId|String|Идентификатор первого запроса в последовательности проверки подлинности.|
|processingTimeInMilliseconds|Int|Время обработки запроса в миллисекунах в AD STS.|
|resourceDisplayName|Строка|Имя ресурса, в который вписались пользователи.|
|resourceId|String|Идентификатор ресурса, в который вписались пользователи.|
|riskDetail|riskDetail|Причина определенного состояния рискованных пользователей, вход в учетную записи или событие риска. Возможные значения: `none` , , , , , , , `adminGeneratedTemporaryPassword` или `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` . Значение `none` означает, что действия для пользователя или входа пока не выполнялись. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные `hidden` клиенты.|
|riskEventTypes|Коллекция riskEventType|Список типов событий риска, связанных со входом. Возможные значения: `unlikelyTravel` , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskEventTypes_v2|Коллекция объектов string|Список типов событий риска, связанных со входом. Возможные значения: `unlikelyTravel` , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|Сводный уровень риска. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные `hidden` клиенты.|
|riskLevelDuringSignIn|riskLevel|Уровень риска при входе. Возможные значения: `none` , , , , , или `low` `medium` `high` `hidden` `unknownFutureValue` . Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Возвращаются все остальные `hidden` клиенты.|
|riskState|riskState|Состояние риска для рискованных пользователей, вход в учетную записи или событие риска. Возможные значения: `none` , , , , , , или `confirmedSafe` `remediated` `dismissed` `atRisk` `confirmedCompromised` `unknownFutureValue` .|
|servicePrincipalId|Строка|Идентификатор приложения, используемый для входов. Это поле заполняется при входе в приложение.|
|servicePrincipalName|String|Имя приложения, используемого для входов. Это поле заполняется при входе в приложение.|
|status|[signInStatus](signinstatus.md)|Состояние для входов. Включает код ошибки и описание ошибки (в случае сбоя при входе).|
|tokenIssuerName|String|Имя поставщика удостоверений. Например, `sts.microsoft.com`.|
|tokenIssuerType|String|Тип поставщика удостоверений. Возможные значения: `AzureAD` , `ADFederationServices` , или `UnknownFutureValue` .|
|userAgent|Строка|Сведения об агенте пользователя, связанные со входом.|
|userDisplayName|String|Отображаемое имя пользователя.|
|userId|String|Идентификатор пользователя.|
|userPrincipalName|String|Имя пользователя.|

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


