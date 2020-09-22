---
title: Тип ресурса Каллтранскриптионинфо
description: Представляет одно событие DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd95ebf165bad8cde296d54e5b0a06f969f1c903
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042711"
---
# <a name="calltranscriptioninfo-resource-type"></a>Тип ресурса Каллтранскриптионинфо

Пространство имен: microsoft.graph

Представляет одно событие DTMF.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| state | String | Возможные значения: `notStarted`, `active`, `inactive`. |
| lastModifiedDateTime | DateTime | Время изменения состояния в формате UTC. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.callTranscriptionInfo"
}-->
```json
{
  "state": "notStarted | active | inactive",
  "lastModifiedDateTime": "String (timestamp)"
}
```


