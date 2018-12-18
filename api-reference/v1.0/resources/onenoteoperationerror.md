---
title: Тип ресурса onenoteOperationError
description: Ошибка, возникшая в результате сбоя операции OneNote.
author: Jewan-microsoft
ms.openlocfilehash: e31d47f9351a050eef134cde2f6a6a8bbdf526d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320694"
---
# <a name="onenoteoperationerror-resource-type"></a>Тип ресурса onenoteOperationError

Ошибка, возникшая в результате сбоя операции OneNote.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|строка|Код ошибки.|
|message|строка|Сообщение об ошибке.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
