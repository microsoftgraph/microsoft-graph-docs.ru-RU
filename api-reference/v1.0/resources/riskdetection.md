---
title: Тип ресурса Рискдетектион
description: обнаружение рисков
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb770a5d44470d1b7467001dc2d16b819a9712a4
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581297"
---
# <a name="riskdetection-resource-type"></a>Тип ресурса Рискдетектион

Пространство имен: Microsoft. Graph представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD постоянно оценивает [риски пользователей](riskyuser.md) , риски, связанные с [входом](signin.md) пользователей и пользователями, на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
>Для использования API обнаружения риска необходима лицензия Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Рискдетектионс](../api/riskdetection-list.md)|Коллекция [рискдетектион](../resources/riskdetection.md)|Получение списка объектов [рискдетектион](../resources/riskdetection.md) и их свойств.|
|[Получение Рискдетектион](../api/riskdetection-get.md)|[рискдетектион](../resources/riskdetection.md)|Чтение свойств и связей объекта [рискдетектион](../resources/riskdetection.md) .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|activity|activityType|Указывает тип действия, с которым связан обнаруженный риск. . Возможные значения: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Дата и время, когда возникло опасное действие.|
|аддитионалинфо|String|Дополнительные сведения, связанные с определением риска в формате JSON.|
|correlationId|String|Корреляционный идентификатор входа, связанный с обнаружением риска. Это свойство имеет значение null, если обнаружение риска не связано с входом.|
|детектеддатетиме|DateTimeOffset|Дата и время обнаружения риска.|
|детектионтимингтипе|рискдетектионтимингтипе|Время обнаружения риска в режиме реального времени (режим реального времени/автономный режим). Возможные значения: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String|Уникальный идентификатор обнаружения риска. Наследуется от [объекта](../resources/entity.md)|
|ipAddress|String|Предоставляет IP-адрес клиента, с которого произошел риск.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения риска.|
|location|[signInLocation](../resources/signinlocation.md)|Расположение входа в систему.|
|requestId|String|Идентификатор запроса, связанный с обнаружением риска. Это свойство имеет значение null, если обнаружение риска не связано с входом.|
|riskDetail|riskDetail|Сведения об обнаруженном риске. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|рискевенттипе|String|Тип обнаруженного события риска. Возможные значения:,,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` и `unknownFutureValue` . Если обнаружение риска является определением Premium, отображается `generic`|
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние обнаруженного опасного пользователя или входа. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|String|Источник обнаружения риска. Например, "activeDirectory". |
|tokenIssuerType|tokenIssuerType|Указывает тип поставщика маркеров для обнаруженного риска при входе. Возможные значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|String|Имя участника-пользователя. |
|userId|String|Уникальный идентификатор пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "String (identifier)",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```