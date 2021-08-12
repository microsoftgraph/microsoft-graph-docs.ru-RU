---
title: Тип ресурса signIn
description: Сведения о действии пользователя и приложения для регистрации клиента (каталог).
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 90a6b1441a5f5cd4c0f83130f30d26983ac6aa05c2b1bc0551ec757d5de5b25c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124208"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

Сведения о действии пользователя и приложения для регистрации клиента (каталог). Необходимо иметь лицензию Azure AD Premium P1 или P2 для загрузки журналов входа с помощью API microsoft Graph.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Чтение свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|String|Имя приложения, отображаемая на портале Azure. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|appId|String|Уникальный GUID, представляющий ID приложения в Azure Active Directory. Поддерживает `$filter` `eq` (только оператор).|
|appliedConditionalAccessPolicy|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection|Предоставляет список политик условного доступа, запускаемых соответствующим действием входа.|
|clientAppUsed|String|Определяет устаревший клиент, используемый для действий по входу.  Включает `Browser` , `Exchange Active Sync` `modern clients` , , , `IMAP` , , `MAPI` `SMTP` и `POP` . Поддерживает `$filter` `eq` (только оператор).|
|conditionalAccessStatus|conditionalAccessStatus| Отчеты о состоянии активированной политики условного доступа. Возможные значения: `success`, `failure`, `notApplied` и `unknownFutureValue`. Поддерживает `$filter` `eq` (только оператор).|
|correlationId|String|ID запроса, отправленный от клиента при входе; для устранения неполадок при входе. Поддерживает `$filter` `eq` (только оператор).|
|createdDateTime|DateTimeOffset|Дата и время (UTC) началась входная точка. Пример: полночь 1 января 2014 г. сообщается как `2014-01-01T00:00:00Z` . Поддерживает `$orderby` и `$filter` `eq` `le` (и только `ge` операторов).|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения о устройстве, откуда произошла входная информация; включает ID устройства, операционную систему и браузер. Поддерживает `$filter` `eq` (и `startsWith` только операторы) в **свойствах браузера** **и operatingSytem.** |
|id|String|Уникальный ID, представляющий действие входного знака. Поддерживает `$filter` `eq` (только оператор).|
|ipAddress|String|IP-адрес клиента, используемого для входов. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|isInteractive|Boolean|Указывает, является ли вход интерактивным или нет.|
|location|[signInLocation](signinlocation.md)|Предоставляет код города, состояния и страны, в котором возникла входная подпись. Поддерживает (и только операторов) в свойствах `$filter` `eq` `startsWith` **city,** **state** и **countryOrRegion.**|
|resourceDisplayName|String|Имя ресурса, в который подписан пользователь. Поддерживает `$filter` `eq` (только оператор).|
|resourceId|String|ID ресурса, в который подписан пользователь. Поддерживает `$filter` `eq` (только оператор).|
|riskDetail|riskDetail|Предоставляет "причину" определенного состояния пользователя с риском, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что действия для пользователя или входа пока не выполнялись.  Поддерживает `$filter` `eq` (только оператор).<br>**Примечание:** Сведения об этом свойстве требуют Azure AD Premium P2 лицензии. Другие лицензии возвращают значение `hidden` .|
|riskEventTypes|коллекция riskEventType|Типы событий риска, связанные с входом. Допустимые значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` и `unknownFutureValue`. Поддерживает `$filter` `eq` (только оператор).|
|riskEventTypes_v2|Коллекция строк|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel` , , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` . Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|riskLevelAggregated|riskLevel|Совокупный уровень риска. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. Поддерживает `$filter` `eq` (только оператор). <br> **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelDuringSignIn|riskLevel|Уровень риска при входе. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD.  Поддерживает `$filter` `eq` (только оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskState|riskState|Отчеты о состоянии рискованного пользователя, входе или событии риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. Поддерживает `$filter` `eq` (только оператор).|
|status|[signInStatus](signinstatus.md)|Состояние регистрации. Включает код ошибки и описание ошибки (в случае сбоя при входе). Поддерживает `$filter` `eq` (только оператор) в **свойстве errorCode.**|
|userDisplayName|String|Отображение имени пользователя, который инициировал вход. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|userId|String|ID пользователя, который инициировал вход. Поддерживает `$filter` `eq` (только оператор).|
|userPrincipalName|String|Имя пользователя, который инициировал вход. Поддерживает `$filter` `eq` (и `startsWith` только операторов).|

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
  "isInteractive": true,
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

