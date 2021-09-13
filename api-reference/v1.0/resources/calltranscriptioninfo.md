---
title: тип ресурса callTranscriptionInfo
description: Представляет одно событие DTMF.
author: rzhang
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 92b95c3a6fde436ffbeca19620c3eed7f16d2297
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067495"
---
# <a name="calltranscriptioninfo-resource-type"></a>тип ресурса callTranscriptionInfo

Пространство имен: microsoft.graph

Представляет одно событие DTMF.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| state | String | Возможные значения: `notStarted`, `active`, `inactive`. |
| lastModifiedDateTime | Даты и время | Время изменения состояния в UTC. |

## <a name="json-representation"></a>Представление в формате JSON

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

