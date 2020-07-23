---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 993201181a9256b54663ce279c914e3669f4dc91
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384681"
---
# <a name="conditionalaccessconditionset-resource-type"></a>Тип ресурса Кондитионалакцесскондитионсет

Пространство имен: microsoft.graph

Представляет тип условий, определяющих, когда применяется политика.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|заявлен|[conditionalAccessApplications](conditionalaccessapplications.md)| Приложения и действия пользователя, включенные в политику и исключенные из нее. Обязательный. |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| Пользователи, группы и роли, включенные в политику и исключенные из нее. Обязательный. |
|клиентапптипес|Коллекция String| Типы клиентских приложений, включенные в политику. Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.|
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Расположения, включенные в политику и исключенные из нее. |
|Embedded|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Платформы, включенные в политику и исключенные из нее. |
|сигнинрисклевелс|Коллекция String| Уровни риска, включенные в политику. Возможные значения: `low`, `medium`, `high`, `none`.|

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
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
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
