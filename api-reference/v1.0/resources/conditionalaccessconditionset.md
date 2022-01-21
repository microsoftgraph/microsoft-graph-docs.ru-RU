---
title: тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, которые регулируются при применяемой политике.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d331a2e1995b6c33ab45f1a99f680b772d090dec
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161706"
---
# <a name="conditionalaccessconditionset-resource-type"></a>тип ресурса conditionalAccessConditionSet

Пространство имен: microsoft.graph

Представляет тип условий, которые регулируются при применяемой политике.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|приложения|[conditionalAccessApplications](conditionalaccessapplications.md)| Приложения и действия пользователей, включенные и исключенные из политики. Обязательный. |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| Пользователи, группы и роли, включенные в политику и исключенные из нее. Обязательное. |
|clientAppTypes|коллекция conditionalAccessClientApp| Типы клиентских приложений, включенные в политику. Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`. Обязательное.|
|devices|[conditionalAccessDevices](conditionalaccessdevices.md)| Устройства в политике. |
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Расположения, включенные и исключенные из политики. |
|платформы|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Платформы, включенные и исключенные из политики. |
|signInRiskLevels|коллекция riskLevel| Уровни риска для входов, включенные в политику. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Обязательное.|
|userRiskLevels|коллекция riskLevel| Уровни риска пользователей, включенные в политику. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Обязательный.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

