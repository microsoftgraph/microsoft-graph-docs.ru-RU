---
title: тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, которые регулируются при применяемой политике.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 162943a5f2d51744ae37d6644f8a01eafb31c259
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961295"
---
# <a name="conditionalaccessconditionset-resource-type"></a>тип ресурса conditionalAccessConditionSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип условий, которые регулируются при применяемой политике.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|приложения|[conditionalAccessApplications](conditionalaccessapplications.md)| Приложения и действия пользователей, включенные и исключенные из политики. Обязательный. |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| Пользователи, группы и роли, включенные в политику и исключенные из нее. Обязательный. |
|clientAppTypes|коллекция conditionalAccessClientApp| Типы клиентских приложений, включенные в политику. Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`. Обязательный.|
|deviceStates|[conditionalAccessDeviceStates](conditionalaccessdevicestates.md)| Состояния устройств в политике. |
|устройства|[conditionalAccessDevices](conditionalaccessdevices.md)| Устройства в политике. |
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Расположения, включенные и исключенные из политики. |
|платформы|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Платформы, включенные и исключенные из политики. |
|signInRiskLevels|коллекция riskLevel| Уровни риска для входов, включенные в политику. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Обязательный.|
|userRiskLevels|коллекция riskLevel| Уровни риска пользователей, включенные в политику. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Обязательный.|

>**Примечание:**
>* **clientAppType** `modern` будет обесценить и заменить `mobileAppsAndDesktopClients` . <br>
>* **clientAppType** `easUnsupported` будет обесцениться, в пользу которой будут включены поддерживаемые и неподдермываемые платформы `exchangeActiveSync` EAS. <br>
>* Мы отстраняем состояние **deviceStates,** и оно может быть удалено в будущем. В будущем используйте **условие устройств.**

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
    "devices",
    "locations",
    "platforms",
    "signInRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


