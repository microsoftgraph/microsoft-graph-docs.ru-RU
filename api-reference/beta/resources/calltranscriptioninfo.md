---
title: тип ресурса callTranscriptionInfo
description: Представляет одно событие DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 27571ad09d6fe29c511b0efa59939dc65074235f9c0c2d4137251687068c47f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54200798"
---
# <a name="calltranscriptioninfo-resource-type"></a>тип ресурса callTranscriptionInfo

Пространство имен: microsoft.graph

Представляет одно событие DTMF.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| state | String | Возможные значения: `notStarted`, `active`, `inactive`. |
| lastModifiedDateTime | DateTime | Время изменения состояния в UTC. |

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


