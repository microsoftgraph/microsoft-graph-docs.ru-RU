---
title: Тип ресурса Упдатерекордингстатусоператион
description: Описывает формат ответа действия обновления состояния записи.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 92cfc481d10cccd3752db29a0c1da7d46000ed3b
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636921"
---
# <a name="updaterecordingstatusoperation-resource-type"></a>Тип ресурса Упдатерекордингстатусоператион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает формат ответа действия обновления состояния записи.

## <a name="properties"></a>Свойства

| Свойство            | Тип                        | Описание|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| Контекст       | String                      | Уникальная строка контекста клиента. Максимальный лимит — 256 символов.                              |
| id                  | Строка                      | Только для чтения.                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | Сведения о результате. Только для чтения.                                                 |
| status              | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "updateRecordingStatusOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
