---
title: Тип ресурса signIn
description: Сведения о действиях пользователя и приложения по входу в клиент (каталог).
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0c450ad78ca91ed49300f94f5bf96b2e2a6fbfe6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137153"
---
# <a name="signin-resource-type"></a>Тип ресурса signIn

Пространство имен: microsoft.graph

Сведения о действиях пользователя и приложения по входу в клиент (каталог). Для скачивания журналов входа с помощью API Microsoft Graph вам требуется лицензия Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Чтение свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appDisplayName|String|Имя приложения, отображаемая на портале Azure.|
|appId|String|Уникальный GUID, представляющий ИД приложения в Azure Active Directory.|
|appliedConditionalAccessPolicy|[Коллекция appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Предоставляет список политик условного доступа, запускаемых соответствующим действием входа.|
|clientAppUsed|String|Определяет устаревший клиент, используемый для действий при входе.  Включает Браузер, Exchange Active Sync, современные клиенты, IMAP, MAPI, SMTP и POP.|
|conditionalAccessStatus|string| Сообщает о состоянии активированной политики условного доступа. Возможные значения: `success` , , , и `failure` `notApplied` `unknownFutureValue` .|
|correlationId|String|ИД запроса, отправленный клиентом при инициале регистрации; используется для устранения неполадок при входе.|
|createdDateTime|DateTimeOffset|Дата и время (UTC) инициировался вход. Пример: полночь 1 января 2014 г. сообщается как `'2014-01-01T00:00:00Z'` .|
|deviceDetail|[deviceDetail](devicedetail.md)|Сведения об устройстве, из которых произошел вход; включает в себя ИД устройства, операционную систему и браузер. |
|id|String|Уникальный ИД, представляющий действие при входе.|
|ipAddress|String|IP-адрес клиента, используемого для входов.|
|isInteractive|Boolean|Указывает, является ли вход интерактивным.|
|location|[signInLocation](signinlocation.md)|Предоставляет код города, штата и страны, в которых был произведен вход.|
|resourceDisplayName|String|Имя ресурса, в который вписал пользователь.|
|resourceId|String|ИД ресурса, в который вписал пользователь.|
|riskDetail|riskDetail|Предоставляет "причину" определенного состояния пользователя с риском, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что действия для пользователя или входа пока не выполнялись. <br>**Примечание.** Для получения сведений об этом свойстве требуется лицензия Azure AD Premium P2. Другие лицензии возвращают это `hidden` значение.|
|riskEventTypes|Коллекция riskEventType|Типы событий риска, связанные со входом. Допустимые значения: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic` и `unknownFutureValue`.|
|riskEventTypes_v2|Коллекция String|Список типов событий риска, связанных со входом. Возможные значения: `unlikelyTravel` , , , , , , , `anonymizedIPAddress` или `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` .|
|riskLevelAggregated|riskLevel|Сводный уровень риска. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskLevelDuringSignIn|riskLevel|Уровень риска при входе. Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`. Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Для всех остальных пользователей возвращается значение `hidden`.|
|riskState|riskState|Сообщает о состоянии рискованных пользователей, входе в учетную записи или о событии риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|Состояние при входе. Включает код ошибки и описание ошибки (в случае сбоя при входе).|
|userDisplayName|String|Отображает имя пользователя, который инициировал вход.|
|userId|String|ИД пользователя, который инициировал вход.|
|userPrincipalName|String|Имя пользователя, который инициировал вход.|

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

