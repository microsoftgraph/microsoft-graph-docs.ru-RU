---
title: Тип ресурса signIn
doc_type: resourcePageType
description: Описание ресурса signIn для API Microsoft Graph (REST), который помогает проводить аудит входа пользователей и входа в приложения (бета-версия).
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6197600854833f7887556c35a511fad61b4539d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965063"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

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
|riskDetail|`riskDetail`|Предоставляет "причину" определенного состояния пользователя с риском, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что действия для пользователя или входа пока не выполнялись. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelAggregated|`riskLevel`|Предоставляет агрегированный уровень риска. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelDuringSignIn|`riskLevel`|Предоставляет уровень риска при входе. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskEventTypes|Коллекция `riskEventType`|Предоставляет список типов событий риска, связанных с входом. Допустимые значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` и `unknownFutureValue`.|
|riskState|`riskState`|Представляет "состояние риска" пользователя с риском, входа или события риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|mfaDetail|[mfaDetail](mfadetail.md)|Предоставляет сведения, связанные с многофакторной проверкой подлинности (MFA), например "Требуется MFA", "Состояние MFA", для соответствующего входа.|
|networkLocationDetails|Коллекция [networkLocationDetail](networklocationdetail.md)|Предоставляет сведения о сетевом расположении.|
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
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "processingTimeInMilliseconds": 12356,
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}]
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
