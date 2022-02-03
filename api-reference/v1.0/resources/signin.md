---
title: Тип ресурса signIn
description: Сведения о действии пользователя и приложения для регистрации клиента (каталог).
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d19cb940729ec0d8140f229473e11f9295e655a1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343489"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

Сведения о действии пользователя и приложения для регистрации клиента (каталог). Необходимо иметь лицензию Azure AD Premium P1 или P2 для загрузки журналов входа с помощью API microsoft Graph. 

Доступность журналов входа регулируется политиками хранения данных [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Чтение свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|String|Имя приложения, отображаемая на портале Azure. `$filter` Поддерживает (`eq`и `startsWith` только операторов).|
|appId|String|Уникальный GUID, представляющий ID приложения в Azure Active Directory. `$filter` Поддерживает (`eq`только оператор).|
|appliedConditionalAccessPolicy|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection|Предоставляет список политик условного доступа, запускаемых соответствующим действием входа.|
|clientAppUsed|String|Определяет клиента, используемого для действия входной записи. Современные клиенты проверки подлинности включают `Browser` и `modern clients`. Устаревшие клиенты проверки подлинности `Exchange ActiveSync`включают `IMAP`, , `MAPI`, , `SMTP`и `POP``other clients`. `$filter` Поддерживает (`eq`только оператор).|
|conditionalAccessStatus|conditionalAccessStatus| Отчеты о состоянии активированной политики условного доступа. Возможные значения: `success`, `failure`, `notApplied` и `unknownFutureValue`. `$filter` Поддерживает (`eq`только оператор).|
|correlationId|String|ID запроса, отправленный от клиента при входе; для устранения неполадок при входе. `$filter` Поддерживает (`eq`только оператор).|
|createdDateTime|DateTimeOffset|Дата и время (UTC) началась входная точка. Пример: полночь 1 января 2014 г. сообщается как `2014-01-01T00:00:00Z`. Поддерживает и `$orderby` `$filter` (`eq`и `le`только `ge` операторов).|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения о устройстве, откуда произошла входная информация; включает ID устройства, операционную систему и браузер. `$filter` Поддерживает (`eq`и `startsWith` только операторы) в **свойствах браузера** **и operatingSytem**. |
|id|String|Уникальный ID, представляющий действие входного знака. `$filter` Поддерживает (`eq`только оператор).|
|ipAddress|String|IP-адрес клиента, используемого для входов. `$filter` Поддерживает (`eq`и `startsWith` только операторов).|
|isInteractive|Boolean|Указывает, является ли вход интерактивным или нет.|
|location|[signInLocation](signinlocation.md)|Предоставляет код города, состояния и страны, в котором возникла входная подпись. `$filter` Поддерживает (`eq`и `startsWith` только операторов) в свойствах **города**, **штата** и **countryOrRegion**.|
|resourceDisplayName|String|Имя ресурса, в который подписан пользователь. `$filter` Поддерживает (`eq`только оператор).|
|resourceId|String|ID ресурса, в который подписан пользователь. `$filter` Поддерживает (`eq`только оператор).|
|riskDetail|riskDetail|Предоставляет "причину" определенного состояния пользователя с риском, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что действия для пользователя или входа пока не выполнялись.  `$filter` Поддерживает (`eq`только оператор).<br>**Примечание:** Сведения об этом свойстве требуют Azure AD Premium P2 лицензии. Другие лицензии возвращают значение `hidden`.|
|riskEventTypes|коллекция riskEventType|Типы событий риска, связанные с входом. Допустимые значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` и `unknownFutureValue`. `$filter` Поддерживает (`eq`только оператор).|
|riskEventTypes_v2|Коллекция объектов string|Список типов событий риска, связанных с входом. Возможные значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, , `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`или `generic``unknownFutureValue`. `$filter` Поддерживает (`eq`и `startsWith` только операторов).|
|riskLevelAggregated|riskLevel|Совокупный уровень риска. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. `$filter` Поддерживает (`eq`только оператор). <br> **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelDuringSignIn|riskLevel|Уровень риска при входе. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD.  `$filter` Поддерживает (`eq`только оператор). <br>**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskState|riskState|Отчеты о состоянии рискованного пользователя, входе или событии риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. `$filter` Поддерживает (`eq`только оператор).|
|status|[signInStatus](signinstatus.md)|Состояние регистрации. Включает код ошибки и описание ошибки (в случае сбоя при входе). `$filter` Поддерживает (только`eq` оператор) в **свойстве errorCode**.|
|userDisplayName|String|Отображение имени пользователя, который инициировал вход. `$filter` Поддерживает (`eq`и `startsWith` только операторов).|
|userId|String|ID пользователя, который инициировал вход. `$filter` Поддерживает (`eq`только оператор).|
|userPrincipalName|String|Имя пользователя, который инициировал вход. `$filter` Поддерживает (`eq`и `startsWith` только операторов).|

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

