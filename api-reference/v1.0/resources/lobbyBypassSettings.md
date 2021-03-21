---
title: тип ресурса lobbyBypassSettings
description: Указывает, какие участники могут обойти вестибюль собрания.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: afd51167179d85706b76c0888f9ee745c7f8b3a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959279"
---
# <a name="lobbybypasssettings-resource-type"></a>тип ресурса lobbyBypassSettings

Пространство имен: microsoft.graph

Указывает, какие участники могут обойти вестибюль собрания.

## <a name="properties"></a>Свойства

| Свойство              | Тип             | Описание                                                                                                                                                          |
| --------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values) | Указывает тип участников, которые автоматически впускаются на собрание, минуя вестибюль. Возможные значения перечислены в следующей таблице. Необязательный параметр. |
| isDialInBypassEnabled | Boolean          | Указывает, следует ли всегда позволять звонителям в обход вестибюля. Необязательный параметр.                                                                                   |

### <a name="lobbybypassscope-values"></a>значения lobbyBypassScope

| Значение                    | Описание                                                                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| organizer                | На собрание впускается только организатор, минуя вестибюль. Все остальные участники размещены в вестибюле собрания.                                                   |
| organization;             | Только участники из одной компании допущены на собрание, минуя вестибюль. Все остальные участники размещены в вестибюле собрания.                         |
| organizationAndFederated | Только участники из одной компании или доверяемой организации впускаются в собрание, минуя лобби. Все остальные участники размещены в вестибюле собрания. |
| все                 | Все допущены к собранию. Участники не размещаются в вестибюле собрания.                                                                                         |
| unknownFutureValue       | Unknow future value.                                                                                                                                                            |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "String",
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
