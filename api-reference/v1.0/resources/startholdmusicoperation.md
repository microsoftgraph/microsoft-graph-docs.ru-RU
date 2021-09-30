---
title: тип ресурса startHoldMusicOperation
description: Представляет состояние операции startHoldMusic, вызываемой вызовом API startHoldMusic.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1c38436cbb8fc7214663aaba9af450879dbd04f
ms.sourcegitcommit: cbad97d6a8ccb89b1822b30a11cc9b6f2670deda
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2021
ms.locfileid: "60016580"
---
# <a name="startholdmusicoperation-resource-type"></a>тип ресурса startHoldMusicOperation

Пространство имен: microsoft.graph

Представляет состояние операции [startHoldMusic,](../api/participant-startholdmusic.md) вызываемой вызовом **API startHoldMusic.** Наследует от [commsOperation](commsoperation.md).

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | Наследуется **от commsOperation**. Уникальная строка контекста клиента. Может иметь не более 256 символов.                                                                               |
| id                             | String                      | Наследуется **от commsOperation**. ID операции сервера. Только для чтения.                                                                                            |
| resultInfo                     | [resultInfo](resultinfo.md) | Наследуется **от commsOperation**. Сведения о результате.  Только для чтения.                                                                                            |
| status                         | String                      | Наследуется **от commsOperation**. Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                 |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.startHoldMusicOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```