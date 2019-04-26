---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
ms.openlocfilehash: 5981f75ee071777f9119d0db2c0078153a160180
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341043"
---
# <a name="convertidresult-resource-type"></a>Тип ресурса Конвертидресулт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| Идентификатор | String | Преобразованный идентификатор. Это значение является исходным непреобразуемым идентификатором. |
| targetId | String | Преобразованный идентификатор. Это значение отсутствует, если произошел сбой преобразования. |
| Еррордетаилс | [Женерицеррор](genericerror.md) | Объект Error, указывающий причину сбоя преобразования. Это значение отсутствует, если преобразование выполнено успешно. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
