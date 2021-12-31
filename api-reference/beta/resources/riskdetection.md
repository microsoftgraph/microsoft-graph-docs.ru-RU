---
title: тип ресурса riskDetection
description: Представляет все обнаружения рисков в клиентах AzureAD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d0acaeb29f80e38cb9a1ce88d2e15878a294a65
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647114"
---
# <a name="riskdetection-resource-type"></a>тип ресурса riskDetection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD непрерывно [](riskyuser.md) оценивает риски пользователей и [](signin.md) рисков, связанных с входом приложения или пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях риска см. [в Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)

>[!NOTE]
>Для использования API обнаружения рисков Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[List riskDetection](../api/riskdetection-list.md) | [коллекция riskDetection](riskdetection.md)|Список обнаружения рисков и их свойств.|
|[Get riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|Получите определенное обнаружение рисков и его свойства.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный ID обнаружения рисков. |
|requestId|string|Запрос iD входного знака, связанного с обнаружением рисков. Это свойство является null, если обнаружение риска не связано с входом.|
|correlationId|string|Корреляция ID входного знака, связанного с обнаружением риска. Это свойство является null, если обнаружение риска не связано с входом. |
|riskEventType|string|Тип обнаруженного события риска. Возможные `unlikelyTravel` значения: `anonymizedIPAddress` , `maliciousIPAddress` , , , , , , , , `unfamiliarFeatures` и `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `generic` `adminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . |
|riskState|riskState|Состояние обнаруженного рискованного пользователя или входной записи. Возможные значения `none` , `confirmedSafe` `remediated` , , , `dismissed` , и `atRisk` `confirmedCompromised` `unknownFutureValue` . |
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения `low` , `medium` `high` , , `hidden` , `none` `unknownFutureValue` . <br />**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут `hidden` возвращены.|
|riskDetail|riskDetail|Сведения об обнаружении риска. Возможные `none` значения: `adminGeneratedTemporaryPassword` , `userPerformedSecuredPasswordChange` , , , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` , `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` , . <br />**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2. Клиенты P1 будут `hidden` возвращены.|
|source|string|Источник обнаружения рисков. Например, `activeDirectory`. |
|detectionTimingType|riskDetectionTimingType|Сроки обнаружения риска (в режиме реального времени и в автономном режиме). Возможные значения `notDefined` , `realtime` `nearRealtime` , , `offline` `unknownFutureValue` . |
|действие|activityType|Указывает тип активности, с чем связан обнаруженный риск. Возможные значения `signin` , `user` `unknownFutureValue` . |
|tokenIssuerType|tokenIssuerType|Указывает тип эмитента маркеров для обнаруженного риска входного знака. Возможные значения: `AzureAD`, `ADFederationServices` и `unknownFutureValue`. |
|ipAddress|string|Предоставляет IP-адрес клиента, откуда возник риск. |
|location|[signInLocation](signinlocation.md)|Расположение входного знака. |
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков. |
|userId|строка|Уникальный идентификатор пользователя.  Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|userDisplayName|string|Имя пользователя. |
|userPrincipalName|string|Имя участника-пользователя. |
|additionalInfo|string|Дополнительные сведения, связанные с обнаружением рисков в формате JSON. |
|riskType (неподготовленный)|riskEventType|Список типов событий риска.<br />**Примечание:** Это свойство обесценилось. Вместо **этого используйте riskEventType.** |

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
