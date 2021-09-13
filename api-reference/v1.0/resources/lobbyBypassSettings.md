---
title: тип ресурса lobbyBypassSettings
description: Указывает, какие участники могут обойти вестибюль собрания.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d850b6335d3a3446516c4fccad1e1dd81518a189
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134740"
---
# <a name="lobbybypasssettings-resource-type"></a>тип ресурса lobbyBypassSettings

Пространство имен: microsoft.graph

Указывает, какие участники могут обойти вестибюль собрания.

## <a name="properties"></a>Свойства

| Свойство              | Тип             | Описание                                                                                                                                                          |
| --------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values) | Указывает тип участников, которые автоматически впускаются на собрание, минуя вестибюль. Возможные значения перечислены в следующей таблице. Необязательное. |
| isDialInBypassEnabled | Логический          | Указывает, следует ли всегда позволять звонителям в обход вестибюля. Необязательное.                                                                                   |

### <a name="lobbybypassscope-values"></a>значения lobbyBypassScope

| Значение                    | Описание                                                                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| organizer                | На собрание впускается только организатор, минуя вестибюль. Все остальные участники размещены в вестибюле собрания.                                                   |
| organization             | Только участники из одной компании допущены на собрание, минуя вестибюль. Все остальные участники размещены в вестибюле собрания.                         |
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
