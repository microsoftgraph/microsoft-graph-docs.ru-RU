---
title: Тип ресурса signIn
description: Сведения о действиях входа пользователей и приложений для клиента (каталога).
author: kholtz
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b9be21b34b291d4a4c7278242c56a3cf63c2c7ea
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124807"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

Сведения о действиях входа пользователей и приложений для клиента (каталога).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Чтение свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|String|Имя приложения отображается на портале Azure.|
|appId|String|Уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|appliedConditionalAccessPolicy|Коллекция [апплиедкондитионалакцессполици](appliedconditionalaccesspolicy.md)|Предоставляет список политик условного доступа, запускаемых соответствующим действием входа.|
|clientAppUsed|String|Определяет устаревший клиент, используемый для входа в систему.  Включает браузер, Exchange Active Sync, современные клиенты, IMAP, MAPI, SMTP и POP.|
|conditionalAccessStatus|string| Сообщает статус активированной политики условного доступа. `success`Возможные значения: `failure`,, `notApplied`и. `unknownFutureValue`|
|correlationId|String|Идентификатор запроса, отправленный клиентом при инициации входа; используется для устранения неполадок, связанных с входом.|
|createdDateTime|DateTimeOffset|Дата и время (в формате UTC), когда был инициирован вход. Пример: полночь 1 января, 2014 отображается как `'2014-01-01T00:00:00Z'`.|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, с которого произошел вход; включает идентификатор устройства, операционную систему и браузер. |
|id|Строка|Уникальный идентификатор, представляющий действия при входе.|
|ipAddress|String|IP-адрес клиента, используемого для входа.|
|isInteractive|Boolean|Указывает, является ли вход в систему интерактивным или нет.|
|location|[signInLocation](signinlocation.md)|Предоставляет код города, региона и страны, где поступил вход.|
|resourceDisplayName|String|Имя ресурса, в который пользователь выполнил вход.|
|resourceId|String|Идентификатор ресурса, в который пользователь выполнил вход.|
|riskDetail|riskDetail|Предоставляет "причину" определенного состояния пользователя с риском, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что действия для пользователя или входа пока не выполнялись. <br>**Примечание:** Для получения сведений о данном свойстве требуется лицензия Azure AD Premium P2. Другие лицензии возвращают значение `hidden`.|
|riskEventTypes|Коллекция Рискевенттипе|Типы событий риска, связанные с входом. Допустимые значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` и `unknownFutureValue`.|
|riskEventTypes_v2|Коллекция объектов string|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures` `malwareInfectedIPAddress`,, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence` `generic`, или `unknownFutureValue`.|
|riskLevelAggregated|riskLevel|Сводный уровень риска. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelDuringSignIn|riskLevel|Уровень риска во время входа. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskState|riskState|Сообщает о состоянии опасного пользователя, входа в систему или события риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|Состояние входа. Возможные значения: `Success` и `Failure`.|
|userDisplayName|String|Отображаемое имя пользователя, который инициировал вход.|
|userId|String|Идентификатор пользователя, который инициировал вход.|
|userPrincipalName|Строка|Имя участника пользователя, который инициировал вход в систему.|

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
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "isInteractive": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["string"],
  "riskEventTypes_v2": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
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
