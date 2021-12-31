---
title: тип ресурса conditionalAccessRulesSatisfied
description: Указывает правила условного доступа, удовлетворены во время события проверки подлинности.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c86ffeaa52941d863529ed4ed3a72d7216359480
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647080"
---
# <a name="conditionalaccessrulessatisfied-resource-type"></a>тип ресурса conditionalAccessRulesSatisfied

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|conditionalAccessCondition|conditionalAccessConditions|Относится к условиям политики условного доступа, которые удовлетворены. Возможные значения: `none` `application` , , , , , , , `users` , `devicePlatform` `location` `clientType` `signInRisk` `userRisk` `time` `deviceState` `client` `ipAddressSeenByAzureAD` `ipAddressSeenByResourceProvider` `unknownFutureValue` `servicePrincipals` `servicePrincipalRisk` . Обратите внимание, что для получения следующих значений в этом развиваемом переуме- `Prefer: include-unknown-enum-members` [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `servicePrincipals` `servicePrincipalRisk`|
|RuleSatisfied|conditionalAccessRule|Относится к условиям политики условного доступа, которые были удовлетворены. Возможные значения: `allApps` `firstPartyApps` , , `office365` `appId` `acr` `appFilter` `allUsers` `guest` `groupId` `roleId` `userId` `allDevicePlatforms` `devicePlatform` `allLocations` `insideCorpnet` `allTrustedLocations` `locationId` `allDevices` `deviceFilter` `deviceState` `unknownFutureValue` , `deviceFilterIncludeRuleNotMatched` `allDeviceStates` . Обратите внимание, что для получения следующих значений в этом развиваемом переуме- `Prefer: include-unknown-enum-members` [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `deviceFilterIncludeRuleNotMatched` `allDeviceStates`|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRuleSatisfied",
  "conditionalAccessCondition": "String",
  "ruleSatisfied": "String"
}
```
