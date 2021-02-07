---
title: Тип ресурса convertIdResult
description: Результат преобразования формата ID, выполненного функцией translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1710c437421426b4bd072e3c654df7d076d0f9f7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135156"
---
# <a name="convertidresult-resource-type"></a>Тип ресурса convertIdResult

Пространство имен: microsoft.graph

Результат преобразования формата ID, выполненного [функцией translateExchangeIds.](../api/user-translateexchangeids.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| sourceId | String | Идентификатор, который был преобразован. Это значение является исходным, не преобразованным идентификатором. |
| targetId | String | Преобразованный идентификатор. Это значение не будет представлено, если преобразование не удалось. |
| errorDetails | [genericError](genericerror.md) | Объект ошибки, указывающий причину сбоя преобразования. Это значение не будет представлено, если преобразование успешно. |

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

