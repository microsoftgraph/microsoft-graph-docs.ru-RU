---
title: тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, которые регулируются при применяемой политике.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 538064190139cb7d8788d25e04b44d54bc372963afb544e89cf47f98b7516f60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189802"
---
# <a name="conditionalaccessconditionset-resource-type"></a>тип ресурса conditionalAccessConditionSet

Пространство имен: microsoft.graph

Представляет тип условий, которые регулируются при применяемой политике.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|приложения|[conditionalAccessApplications](conditionalaccessapplications.md)| Приложения и действия пользователей, включенные и исключенные из политики. Обязательный элемент. |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| Пользователи, группы и роли, включенные в политику и исключенные из нее. Обязательный элемент. |
|clientAppTypes|коллекция conditionalAccessClientApp| Типы клиентских приложений, включенные в политику. Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`. Обязательный элемент.|
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Расположения, включенные и исключенные из политики. |
|платформы|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Платформы, включенные и исключенные из политики. |
|signInRiskLevels|коллекция riskLevel| Уровни риска для входов, включенные в политику. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Обязательный элемент.|
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

