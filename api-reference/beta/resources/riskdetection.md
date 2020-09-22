---
title: Тип ресурса Рискдетектион
description: Представляет все обнаруженные риски в клиентах AzureAD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0be7f15424c7e949207c8fa129df0536ecb83c22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021156"
---
# <a name="riskdetection-resource-type"></a>Тип ресурса Рискдетектион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD постоянно оценивает [риски пользователей](riskyuser.md) , риски, связанные с [входом](signin.md) пользователей и пользователями, на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).

>[!NOTE]
>Для использования API обнаружения риска необходима лицензия Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список Рискдетектион](../api/riskdetection-list.md) | Коллекция [рискдетектион](riskdetection.md)|Перечисление обнаруженных рисков и их свойств.|
|[Получение Рискдетектион](../api/riskdetection-get.md) | [рискдетектион](riskdetection.md)|Получение определенного опасного обнаружения и его свойств.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|`id`|`string`|Уникальный идентификатор обнаружения риска. |
|`requestId`|`string`|Идентификатор запроса, связанный с обнаружением риска. Это свойство имеет значение null, если обнаружение риска не связано с входом.|
|`correlationId`|`string`|Корреляционный идентификатор входа, связанный с обнаружением риска. Это свойство имеет значение null, если обнаружение риска не связано с входом. |
|`riskEventType`|`string`|Тип обнаруженного события риска. Возможные значения:,,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` и `unknownFutureValue` . |
|`riskType`|`riskEventType`|Список типов событий риска.<br/>**Примечание:** Это свойство является устаревшим. Вместо этого используйте **рискевенттипес** . |
|`riskState`|`riskState`|Состояние обнаруженного опасного пользователя или входа. Возможные значения: None, Конфирмедсафе, remediateо, Атриск, Конфирмедкомпромисед и unknownFutureValue. |
|`riskLevel`|`riskLevel`|Уровень обнаруженного риска. Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden` .|
|`riskDetail`|`riskDetail`|Сведения об обнаруженном риске. Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут возвращены `hidden` .|
|`source`|`string`|Источник обнаружения риска. Например, "activeDirectory". |
|`detectionTimingType`|`riskDetectionTimingType`|Время обнаружения риска в режиме реального времени (режим реального времени/автономный режим). Возможные значения: Нотдефинед, реального времени, Неарреалтиме, offline, unknownFutureValue. |
|`activity`|`activityType`|Указывает тип действия, с которым связан обнаруженный риск. Возможные значения: Signing, User, unknownFutureValue. |
|`tokenIssuerType`|`tokenIssuerType`|Указывает тип поставщика маркеров для обнаруженного риска при входе. Возможные значения: AzureAD, Адфедератионсервицес и unknownFutureValue. |
|`ipAddress`|`string`|Предоставляет IP-адрес клиента, с которого произошел риск. |
|`location`|[signInLocation](signinlocation.md)|Расположение входа в систему. |
|`activityDateTime`|`datetimeoffset`|Дата и время, когда возникло опасное действие. |
|`detectedDateTime`|`datetimeoffset`|Дата и время обнаружения риска. |
|`lastUpdatedDateTime`|`datetime`|Дата и время последнего обновления обнаружения риска. |
|`userId`|`string`|Уникальный идентификатор пользователя. |
|`userDisplayName`|`string`|Имя пользователя. |
|`userPrincipalName`|`string`|Имя участника-пользователя. |
|`additionalInfo`|`string`|Дополнительные сведения, связанные с определением риска в формате JSON. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


