---
title: Тип ресурса вход
description: 'Этот ресурс подробно описывает активность пользователя или приложения входа в каталоге. '
ms.openlocfilehash: f176f707e87b3e88292c32fba3748b9e70110e87
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184541"
---
# <a name="signin-resource-type"></a>Тип ресурса вход
Этот ресурс подробно описывает активность пользователя или приложения входа в каталоге. 

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список вход](../api/signin-list.md) | [Вход](signin.md) |Чтение свойств и отношений между объектами вход.|
|[Получение вход](../api/signin-get.md) | [Вход](signin.md) |Чтение свойства и связи объекта вход.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|Строка|Ссылается на имя приложения, отображаемые на портале Azure.|
|appId|String|Указывает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|clientAppUsed|Строка|Предоставляет устаревший клиент, используемый для входа в activty.E.g. включает в себя браузера, протокол Exchange Active Sync, современный клиентов, IMAP, MAPI, SMTP, POP.|
|appliedConditionalAccessPolicy|[conditionalAccessPolicy](conditionalaccesspolicy.md) коллекции|Предоставляет список политик условного доступа, которые запускаются с помощью соответствующего действия входа в.|
|conditionalAccessStatus|строка| Предоставляет сведения о состоянии политики условного доступа запущено. Возможные значения: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|originalRequestId|Строка|Идентификатор запроса на первый запрос в последовательность проверки подлинности.|
|isInteractive|Boolean|Указывает, является ли вход интерактивные или нет.|
|tokenIssuerName|Строка|Имя идентификатора поставщика (например, sts.microsoft.com)|
|tokenIssuerType|Строка|Предоставляет тип identityProvider. Возможные значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|correlationId|String|Ссылается на идентификатор, который отправляется из клиента при входе в. Используется для устранения неполадок соответствующего действия входа при вызове служба технической поддержки или в службу поддержки.|
|createdDateTime|DateTimeOffset|Содержит дату и время входа в инициированного. Тип метки времени — всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|deviceDetail|[deviceDetail](devicedetail.md)|Предоставляет сведения о устройства из входа в возникновения. Его сведения inclules как deviceId, операционная система, браузер. |
|id|Строка|Указывает уникальный идентификатор, представляющий операции регистрации.|
|ipAddress|String|Предоставляет IP-адрес клиента, с которой входа в произошла.|
|location|[signInLocation](signinlocation.md)|Предоставляет Город, состояний и код страны 2 букв от входа в возникновения.|
|processingTimeInMilliseconds|Int|Содержит время в миллисекундах, в AD STS обработки запросов|
|riskDetail|`riskDetail`|Предоставляет «причина» за с определенным состоянием рискованный пользователя, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что никакие действия не выполнены на пользователя или входа в данный момент.|
|riskLevelAggregated|`riskLevel`|Предоставляет сводные риском. Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`. Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.|
|riskLevelDuringSignIn|`riskLevel`|Предоставляет уровень риска при входе в систему. Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`. Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.|
|riskEventTypes|`riskEventTypes`|Содержит список типов событий рисков, связанных с входа в. Возможные значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, и `unknownFutureValue`.|
|riskState|`riskState`|Предоставляет «состояние риска» рискованный пользователя, входа или события риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|mfaDetail|[mfaDetail](mfadetail.md)|Предоставляет многофакторной проверкой Подлинности связанные сведения, как требуется многофакторной проверкой Подлинности, состояние многофакторной проверкой Подлинности для соответствующих входа в.|
|networkLocationDetail|[networkLocationDetail](networklocationdetail.md)|Предоставляет сведения о сетевой папке.|
|riskLevel|строка| Предоставляет уровень риска, связанный с входа в программу. Возможные значения: `low`, `medium`, `high`.|
|status|[signInStatus](signinstatus.md)|Предоставляет состояние входа. Возможные значения `Success` и `Failure`.|
|userDisplayName|String|Указывает отображаемое имя пользователя.|
|userId|String|Указывает идентификатор пользователя пользователя.|
|userPrincipalName|Строка|Указывает имя участника-пользователя.|
|resourceDisplayName|Строка|Указывает имя ресурса, когда пользователь входил в|
|resourceId|String|Указывает идентификатор ресурса, когда пользователь входил в.|
|authenticationMethodsUsed|Строка|Указывает список методов проверки подлинности используется|

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
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": "string",
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
