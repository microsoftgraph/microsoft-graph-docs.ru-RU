---
title: тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, которые регулируются при применяемой политике.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6bb96bd08f9ffdd3876ba3836b19878b24fad686
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672548"
---
# <a name="conditionalaccessconditionset-resource-type"></a>тип ресурса conditionalAccessConditionSet

Пространство имен: microsoft.graph

Представляет тип условий, которые регулируются при применяемой политике.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|приложения|[conditionalAccessApplications](conditionalaccessapplications.md)| Приложения и действия пользователей, включенные и исключенные из политики. Обязательный. |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| Пользователи, группы и роли, включенные в политику и исключенные из нее. Обязательный. |
|clientApplications|[conditionalAccessClientApplications](../resources/conditionalaccessclientapplications.md)|Клиентские приложения (директора служб и удостоверения рабочей нагрузки), включенные в политику и исключенные из нее. Требуется **либо** пользователь **, либо clientApplications** . |
|clientAppTypes|коллекция conditionalAccessClientApp| Типы клиентских приложений, включенные в политику. Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`. Обязательный.|
|devices|[conditionalAccessDevices](conditionalaccessdevices.md)| Устройства в политике. |
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Расположения, включенные и исключенные из политики. |
|платформы|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Платформы, включенные и исключенные из политики. |
|signInRiskLevels|коллекция riskLevel| Уровни риска для входов, включенные в политику. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Обязательный.|
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
  "clientApplications": {"@odata.type": "microsoft.graph.conditionalAccessClientApplications"},
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

