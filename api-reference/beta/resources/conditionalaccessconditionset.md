---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e81e8b2748a7dc3b6a9ca028472c1f6ab153b0e
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638514"
---
# <a name="conditionalaccessconditionset-resource-type"></a>Тип ресурса Кондитионалакцесскондитионсет

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип условий, определяющих, когда применяется политика.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|заявлен|[кондитионалакцессаппликатионс](conditionalaccessapplications.md)| Приложения и действия пользователя, включенные в политику и исключенные из нее. Обязательный элемент. |
|users|[кондитионалакцессусерс](conditionalaccessusers.md)| Пользователи, группы и роли, включенные в политику и исключенные из нее. Обязательный элемент. |
|клиентапптипес|Коллекция строк| Типы клиентских приложений, включенные в политику. Возможные значения: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.|
|deviceStates|[кондитионалакцессдевицестатес](conditionalaccessdevicestates.md)| Состояния устройств в политике. |
|locations|[кондитионалакцесслокатионс](conditionalaccesslocations.md)| Расположения, включенные в политику и исключенные из нее. |
|Embedded|[кондитионалакцессплатформс](conditionalaccessplatforms.md)| Платформы, включенные в политику и исключенные из нее. |
|сигнинрисклевелс|Коллекция строк| Уровни риска, включенные в политику. Возможные значения: `low`, `medium`, `high`, `none`.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
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