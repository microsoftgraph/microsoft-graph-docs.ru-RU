---
title: Тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, управляющих применимой политикой.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e331a482fce3274463f742ceba6dc111437cd95
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137384"
---
# <a name="conditionalaccessconditionset-resource-type"></a>Тип ресурса conditionalAccessConditionSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип условий, управляющих применимой политикой.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applications|[conditionalAccessApplications](conditionalaccessapplications.md)| Приложения и действия пользователей, включенные в политику и исключенные из нее. Обязательный элемент. |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| Пользователи, группы и роли, включенные в политику и исключенные из нее. Обязательный элемент. |
|clientAppTypes|Коллекция объектов string| Типы клиентских приложений, включенные в политику. Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.|
|deviceStates|[conditionalAccessDeviceStates](conditionalaccessdevicestates.md)| Состояния устройств в политике. |
|устройства|[conditionalAccessDevices](conditionalaccessdevices.md)| Устройства в политике. |
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Расположения, включенные в политику и исключенные из нее. |
|платформы|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Платформы, включенные в политику и исключенные из нее. |
|signInRiskLevels|Коллекция объектов string| Уровни риска для входов, включенные в политику. Возможные значения: `low`, `medium`, `high`, `none`.|
|userRiskLevels|Коллекция объектов string| Уровни риска для пользователей, включенные в политику. Возможные значения: `low`, `medium`, `high`, `none`.|

>**Примечание:** 

>**clientAppType** `modern` будет неподготовлен и заменен `mobileAppsAndDesktopClients` . 

>**clientAppType** `easUnsupported` будет не поддерживаться, в том числе поддерживаемые и неподдершенные `exchangeActiveSync` платформы EAS. 

>Условие **deviceStates** является неподготовленным, и оно может быть удалено в будущем. В будущем используйте **условие устройств.**

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


