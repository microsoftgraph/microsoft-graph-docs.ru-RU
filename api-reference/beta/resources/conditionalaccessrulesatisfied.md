---
title: Тип ресурса conditionalAccessRulesGeography
description: Указывает правила условного доступа, которые удовлетворяются во время события проверки подлинности.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 50ebb20c38275a7ab0192b56ca67058ff640948f
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645438"
---
# <a name="conditionalaccessrulessatisfied-resource-type"></a>Тип ресурса conditionalAccessRulesGeography

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые активируются соответствующим действием входа.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|conditionalAccessCondition|conditionalAccessConditions|Ссылается на условия политики условного доступа, которые выполняются. Возможные значения: `none`, , `application`, `users`, `devicePlatform`, `location`, `clientType`, `userRisk``signInRisk`, `time`, `deviceState`, `client`, `ipAddressSeenByAzureAD`, `ipAddressSeenByResourceProvider`, , `unknownFutureValue`, . `servicePrincipals``servicePrincipalRisk` Обратите внимание, что необходимо использовать заголовок `Prefer: include-unknown-enum-members` запроса для получения следующих значений в этом развиваемом перечислении[:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`servicePrincipals` , `servicePrincipalRisk`.|
|ruleИмя|conditionalAccessRule|Относится к условиям политики условного доступа, которые были выполнены. Возможные значения: `allApps`, , `firstPartyApps``office365``appId``acr``appFilter``allUsers``guest``groupId``roleId``userId``allDevicePlatforms``devicePlatform``allLocations``insideCorpnet``allTrustedLocations``locationId``allDevices``deviceFilter``deviceState``unknownFutureValue``deviceFilterIncludeRuleNotMatched``allDeviceStates``anonymizedIPAddress``unfamiliarFeatures``nationStateIPAddress``realTimeThreatIntelligence``internalGuest``b2bCollaborationGuest``b2bCollaborationMember``b2bDirectConnectUser``otherExternalUser``serviceProvider` Обратите внимание, что необходимо использовать заголовок `Prefer: include-unknown-enum-members` запроса для получения следующих значений в этом развиваемом перечислении[:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`deviceFilterIncludeRuleNotMatched` , `allDeviceStates`.|


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
