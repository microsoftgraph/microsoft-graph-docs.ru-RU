---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 040b13ab83eacffb33e8903f7d11823adb6e1bf1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973209"
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
