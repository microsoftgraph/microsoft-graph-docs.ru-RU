---
title: тип ресурса lobbyBypassSettings
description: Указывает, какие участники могут обойти вестибюль собрания.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5fa0fac27d8dfaacb27572476ab49e80cb3832e
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805585"
---
# <a name="lobbybypasssettings-resource-type"></a>тип ресурса lobbyBypassSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, какие участники могут обойти вестибюль собрания.

## <a name="properties"></a>Свойства

| Свойство              | Тип    | Описание                                                         |
| --------------------- | ------- | ------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | Указывает тип участников, которые автоматически впускаются на собрание, минуя вестибюль. Необязательное.|
| isDialInBypassEnabled | Boolean | Указывает, следует ли всегда позволять звонителям в обход вестибюля. Необязательное. |

### <a name="lobbybypassscope-values"></a>значения lobbyBypassScope

| Значение                    | Описание     |
| ------------------------ | --------------------------------------------------- |
| organizer | В собрание и обход вестибюля впускается только организатор. Все остальные участники размещены в вестибюле собрания. |
| organization | Только участники из одной компании и **гости** допущены к собранию и обходу вестибюля. Все остальные участники размещены в вестибюле собрания. |
| organizationAndFederated | Только участники из одной компании или доверенных организаций и гости могут быть допущены на собрание и обход вестибюля. Все остальные участники размещены в вестибюле собрания. |
| все | Все допущены к собранию. Участники не размещаются в вестибюле собрания. |
| приглашенный | На собрание и обход вестибюля впускаются только те люди, которых приглашает организатор. Все остальные участники размещены в вестибюле собрания. |
| organizationExcludingGuests |  Только участники из одной и той же компании допущены к собранию и обходу вестибюля. Все остальные участники размещены в вестибюле собрания. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
