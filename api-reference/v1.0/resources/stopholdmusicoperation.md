---
title: тип ресурса stopHoldMusicOperation
description: Представляет состояние операции stopHoldMusic, вызываемой вызовом aPI stopHoldMusic.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a0a30e783bfbcb08c613b2c0dd80a933d206830e
ms.sourcegitcommit: cbad97d6a8ccb89b1822b30a11cc9b6f2670deda
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2021
ms.locfileid: "60016577"
---
# <a name="stopholdmusicoperation-resource-type"></a>тип ресурса stopHoldMusicOperation

Пространство имен: microsoft.graph

Представляет состояние операции [stopHoldMusic,](../api/participant-stopholdmusic.md) вызываемой вызовом **aPI stopHoldMusic.** Наследует от [commsOperation](commsoperation.md).

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
  "@odata.type": "microsoft.graph.stopHoldMusicOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```