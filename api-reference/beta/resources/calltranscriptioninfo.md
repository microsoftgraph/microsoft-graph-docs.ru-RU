---
title: тип ресурса callTranscriptionInfo
description: Представляет одно событие DTMF.
author: rzhang
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1597d86fa37e55ec8c5a205a24688c101c8838e0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023831"
---
# <a name="calltranscriptioninfo-resource-type"></a>тип ресурса callTranscriptionInfo

Пространство имен: microsoft.graph

Представляет одно событие DTMF.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| state | String | Возможные значения: `notStarted`, `active`, `inactive`. |
| lastModifiedDateTime | Даты и время | Время изменения состояния в UTC. |

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


