---
title: тип ресурса riskDetection
description: обнаружение рисков
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8818799c24bfffaf8ddb0494d5a13c45d2fb15e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103993"
---
# <a name="riskdetection-resource-type"></a>тип ресурса riskDetection

Пространство имен: microsoft.graph представляет сведения об обнаруженном риске в клиенте Azure AD. 

Azure AD непрерывно [](riskyuser.md) оценивает риски пользователей и [](signin.md) рисков, связанных с входом приложения или пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.

Дополнительные сведения о событиях риска см. [в Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)

>[!NOTE]
>Для использования API обнаружения рисков Azure AD Premium P1 или P2.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список riskDetections](../api/riskdetection-list.md)|[коллекция riskDetection](../resources/riskdetection.md)|Получите список объектов [riskDetection](../resources/riskdetection.md) и их свойств.|
|[Get riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|Ознакомьтесь с свойствами и отношениями объекта [riskDetection.](../resources/riskdetection.md)|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|действие|activityType|Указывает тип активности, с чем связан обнаруженный риск. . Возможные значения: `signin`, `user`, `unknownFutureValue`.|
|activityDateTime|DateTimeOffset|Дата и время возникновения рискованных действий. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь UTC 1 января 2014 г. выглядит так: `2014-01-01T00:00:00Z`|
|additionalInfo|Строка|Дополнительные сведения, связанные с обнаружением рисков в формате JSON.|
|correlationId|String|Корреляция ID входного знака, связанного с обнаружением риска. Это свойство, если обнаружение риска не связано `null` с входом.|
|detectedDateTime|DateTimeOffset|Дата и время обнаружения риска. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь UTC 1 января 2014 г. выглядит так: `2014-01-01T00:00:00Z`|
|detectionTimingType|riskDetectionTimingType|Сроки обнаружения риска (в режиме реального времени и в автономном режиме). Возможные значения: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|id|String|Уникальный ID обнаружения рисков. Унаследованный от [сущности](../resources/entity.md)|
|ipAddress|String|Предоставляет IP-адрес клиента, откуда возник риск.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления обнаружения рисков. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь UTC 1 января 2014 г. выглядит так: `2014-01-01T00:00:00Z`|
|location|[signInLocation](../resources/signinlocation.md)|Расположение входного знака.|
|requestId|Строка|Запрос iD входного знака, связанного с обнаружением рисков. Это свойство является null, если обнаружение риска не связано с входом.|
|riskDetail|riskDetail|Сведения об обнаружении риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventType|Строка|Тип обнаруженного события риска. Возможные `unlikelyTravel` значения: `anonymizedIPAddress` , `maliciousIPAddress` , , , , , , , , `unfamiliarFeatures` и `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `generic` `adminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . Если обнаружение риска является обнаружением премиум-класса, покажут `generic`|
|riskLevel|riskLevel|Уровень обнаруженного риска. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние обнаруженного рискованного пользователя или входной записи. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|source|String|Источник обнаружения рисков. Например, `activeDirectory`. |
|tokenIssuerType|tokenIssuerType|Указывает тип эмитента маркеров для обнаруженного риска входного знака. Возможные значения: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userDisplayName|String|Имя участника-пользователя. |
|userId|String|Уникальный идентификатор пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Отношения
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
