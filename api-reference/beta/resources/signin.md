---
title: Тип ресурса signIn
description: 'Этот ресурс представляет сведения о действиях входа пользователя или приложения в каталоге. '
localization_priority: Priority
ms.openlocfilehash: 3d9b9ffab6b588cbe0a465a637b12649110415d2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571851"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn
Этот ресурс представляет сведения о действиях входа пользователя или приложения в каталоге. 

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Чтение свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|String|Обозначает имя приложения, отображаемое на портале Azure.|
|appId|String|Обозначает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|clientAppUsed|String|Представляет устаревший клиент, использовавшийся для действия входа. Например: браузер, Exchange Active Sync, современные клиенты, IMAP, MAPI, SMTP, POP.|
|appliedConditionalAccessPolicy|Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)|Предоставляет список политик условного доступа, запускаемых соответствующим действием входа.|
|conditionalAccessStatus|string| Предоставляет состояние запущенной политики условного доступа. Возможные значения: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|originalRequestId|String|Идентификатор первого запроса в последовательности проверки подлинности.|
|isInteractive|Boolean|Указывает, является ли вход интерактивным.|
|tokenIssuerName|String|Имя поставщика удостоверений (например, sts.microsoft.com)|
|tokenIssuerType|String|Представляет тип identityProvider. Возможные значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|correlationId|String|Обозначает идентификатор, отправленный из клиента при инициации входа. Используется для устранения неполадок с соответствующим действием входа при вызове службы поддержки.|
|createdDateTime|DateTimeOffset|Предоставляет дату и время инициации входа. Тип Timestamp всегда представлен в формате времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|deviceDetail|[deviceDetail](devicedetail.md)|Предоставляет сведения об устройстве, с которого выполнен вход. Содержит такие сведения, как deviceId, ОС, браузер. |
|id|String|Указывает уникальный идентификатор, представляющий действие входа.|
|ipAddress|String|Предоставляет IP-адрес клиента, из которого выполнен вход.|
|location|[signInLocation](signinlocation.md)|Представляет город, область и 2-буквенный код страны, откуда выполнен вход.|
|processingTimeInMilliseconds|Int|Предоставляет время обработки запроса (в миллисекундах) в службе маркеров безопасности AD|
|riskDetail| enum-string |Предоставляет "причину" определенного состояния пользователя с риском, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что действия для пользователя или входа пока не выполнялись. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelAggregated| enum-string |Предоставляет объединенный уровень риска. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelDuringSignIn| enum-string |Предоставляет уровень риска при входе. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskEventTypes| enum-string |Предоставляет список типов событий риска, связанных с входом. Допустимые значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` и `unknownFutureValue`.|
|riskState|`riskState`|Представляет "состояние риска" пользователя с риском, входа или события риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|mfaDetail|[mfaDetail](mfadetail.md)|Предоставляет сведения, связанные с многофакторной проверкой подлинности (MFA), например "Требуется MFA", "Состояние MFA", для соответствующего входа.|
|networkLocationDetail| [deviceDetail](networklocationdetail.md) |Предоставляет сведения о сетевом расположении.|
|riskLevel|string| Представляет уровень риска, связанный с входом. Возможные значения: `low`, `medium`, `high`.|
|status|[signInStatus](signinstatus.md)|Представляет состояние входа. Возможные значения: `Success` и `Failure`.|
|userDisplayName|String|Указывает отображаемое имя пользователя.|
|userId|String|Указывает userId пользователя.|
|userPrincipalName|String|Указывает UPN пользователя.|
|resourceDisplayName|String|Указывает имя ресурса, в который вошел пользователь.|
|resourceId|String|Указывает идентификатор ресурса, в который вошел пользователь.|
|authenticationMethodsUsed|String|Указывает список примененных методов проверки подлинности|

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
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "originalRequestId": "String",
  "isInteractive": "String",
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "none | adminGeneratedTemporaryPassword | userPerformedSecuredPasswordChange | userPerformedSecuredPasswordReset | adminConfirmedSigninSafe | aiConfirmedSigninSafe | userPassedMFADrivenByRiskBasedPolicy | adminDismissedAllRiskForUser | adminConfirmedSigninCompromised | unknownFutureValue",
  "riskLevelAggregated": "enum-string",
  "riskLevelDuringSignIn": "enum-string",
  "riskState": "riskState",
  "riskEventTypes": "enum-string",
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
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
