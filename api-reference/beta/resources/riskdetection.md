---
title: тип ресурса riskDetection
description: Представляет все обнаружения рисков в клиентах AzureAD.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 40fa938f94f5f43a61c191a3d3c14b0dbbb10d6f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440138"
---
# <a name="riskdetection-resource-type"></a>тип ресурса riskDetection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD непрерывно [](riskyuser.md) оценивает риски пользователей и [](signin.md) рисков, связанных с входом приложения или пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)

>[!NOTE]
>Чтобы использовать API обнаружения рисков, необходимо иметь лицензию Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[List riskDetection](../api/riskdetection-list.md) | [коллекция riskDetection](riskdetection.md)|Список обнаружения рисков и их свойств.|
|[Get riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Получите определенное обнаружение рисков и его свойства.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|`id`|`string`|Уникальный ID обнаружения рисков. |
|`requestId`|`string`|Запрос iD входного знака, связанного с обнаружением рисков. Это свойство является null, если обнаружение риска не связано с входом.|
|`correlationId`|`string`|Корреляция ID входного знака, связанного с обнаружением риска. Это свойство является null, если обнаружение риска не связано с входом. |
|`riskEventType`|`string`|Тип обнаруженного события риска. Возможные `unlikelyTravel` значения: `anonymizedIPAddress` , `maliciousIPAddress` , , , , , , , , `unfamiliarFeatures` и `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . |
|`riskType`|`riskEventType`|Список типов событий риска.<br/>**Примечание:** Это свойство обесценилось. Вместо **этого используйте riskEventTypes.** |
|`riskState`|`riskState`|Состояние обнаруженного рискованного пользователя или входной записи. Возможные значения не являются никакими, подтвержденнымиSafe, исправленными, уволенными, atRisk, confirmedCompromised и unknownFutureValue. |
|`riskLevel`|`riskLevel`|Уровень обнаруженного риска. Возможные значения : низкие, средние, высокие, скрытые, неизвестные. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут `hidden` возвращены.|
|`riskDetail`|`riskDetail`|Сведения об обнаружении риска. Возможные значения не являются никакими, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue. **Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут `hidden` возвращены.|
|`source`|`string`|Источник обнаружения рисков. Например, "activeDirectory". |
|`detectionTimingType`|`riskDetectionTimingType`|Сроки обнаружения риска (в режиме реального времени и в автономном режиме). Возможные значения неDefined, realtime, nearRealtime, автономно, unknownFutureValue. |
|`activity`|`activityType`|Указывает тип активности, с чем связан обнаруженный риск. Возможные значения : signin, user, unknownFutureValue. |
|`tokenIssuerType`|`tokenIssuerType`|Указывает тип эмитента маркеров для обнаруженного риска входного знака. Возможные значения : AzureAD, ADFederationServices и unknownFutureValue. |
|`ipAddress`|`string`|Предоставляет IP-адрес клиента, откуда возник риск. |
|`location`|[signInLocation](signinlocation.md)|Расположение входного знака. |
|`activityDateTime`|`datetimeoffset`|Дата и время возникновения рискованных действий. |
|`detectedDateTime`|`datetimeoffset`|Дата и время обнаружения риска. |
|`lastUpdatedDateTime`|`datetime`|Дата и время последнего обновления обнаружения рисков. |
|`userId`|`string`|Уникальный идентификатор пользователя. |
|`userDisplayName`|`string`|Имя пользователя. |
|`userPrincipalName`|`string`|Имя участника-пользователя. |
|`additionalInfo`|`string`|Дополнительные сведения, связанные с обнаружением рисков в формате JSON. |

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
