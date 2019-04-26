---
title: Тип ресурса Женерицеррор
description: Общая ошибка общего назначения.
localization_priority: Normal
ms.openlocfilehash: 314bb5f5e94e44c326fceb71f4a79463989f2129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333673"
---
# <a name="genericerror-resource-type"></a>Тип ресурса Женерицеррор

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Общая ошибка общего назначения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| message | String | Сообщение об ошибке. |
| code | String | Код ошибки. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
