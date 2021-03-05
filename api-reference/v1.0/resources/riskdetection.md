---
title: тип ресурса riskDetection
description: обнаружение рисков
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e52fb1b67d82091360f83383d941552316d107b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449007"
---
# <a name="riskdetection-resource-type"></a>тип ресурса riskDetection

Пространство имен: microsoft.graph представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD непрерывно [](riskyuser.md) оценивает риски пользователей и [](signin.md) рисков, связанных с входом приложения или пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)

>[!NOTE]
>Чтобы использовать API обнаружения рисков, необходимо иметь лицензию Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список riskDetections](../api/riskdetection-list.md)|[коллекция riskDetection](../resources/riskdetection.md)|Получите список объектов [riskDetection](../resources/riskdetection.md) и их свойств.|
|[Get riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Ознакомьтесь с свойствами и отношениями объекта [riskDetection.](../resources/riskdetection.md)|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|действие|activityType|Указывает тип активности, с чем связан обнаруженный риск. . Возможные значения: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий.|
|additionalInfo|String|Дополнительные сведения, связанные с обнаружением рисков в формате JSON.|
|correlationId|String|Корреляция ID входного знака, связанного с обнаружением риска. Это свойство является null, если обнаружение риска не связано с входом.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска.|
|detectionTimingType|riskDetectionTimingType|Сроки обнаружения риска (в режиме реального времени и в автономном режиме). Возможные значения: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String|Уникальный ID обнаружения рисков. Унаследованный от [сущности](../resources/entity.md)|
|ipAddress|String|Предоставляет IP-адрес клиента, откуда возник риск.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков.|
|location|[signInLocation](../resources/signinlocation.md)|Расположение входного знака.|
|requestId|String|Запрос iD входного знака, связанного с обнаружением рисков. Это свойство является null, если обнаружение риска не связано с входом.|
|riskDetail|riskDetail|Сведения об обнаружении риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventType|String|Тип обнаруженного события риска. Возможные `unlikelyTravel` значения: `anonymizedIPAddress` , `maliciousIPAddress` , , , , , , , , `unfamiliarFeatures` и `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . Если обнаружение риска является обнаружением премиум-класса, покажут `generic`|
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние обнаруженного рискованного пользователя или входной записи. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|String|Источник обнаружения рисков. Например, "activeDirectory". |
|tokenIssuerType|tokenIssuerType|Указывает тип эмитента маркеров для обнаруженного риска входного знака. Возможные значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
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
