---
title: Тип ресурса Упдатерекордингстатусоператион
description: Описывает формат ответа действия обновления состояния записи.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: de1cf2578f699fde25d8863d12fcf4e262d78000
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962551"
---
# <a name="updaterecordingstatusoperation-resource-type"></a>Тип ресурса Упдатерекордингстатусоператион

Пространство имен: microsoft.graph

Описывает формат ответа действия обновления состояния записи.

## <a name="properties"></a>Свойства

| Свойство            | Тип                        | Описание|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| Контекст       | String                      | Уникальная строка контекста клиента. Максимальный лимит — 256 символов.                              |
| id                  | Строка                      | Только для чтения.                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | Сведения о результате. Только для чтения.                                                 |
| status              | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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
