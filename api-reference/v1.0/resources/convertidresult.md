---
title: тип ресурса convertIdResult
description: Результат преобразования формата ID, выполняемого функцией translateExchangeIds.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: e2bb28e7ee4d889fec24152de27e37399e8acfa1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053156"
---
# <a name="convertidresult-resource-type"></a>тип ресурса convertIdResult

Пространство имен: microsoft.graph

Результат преобразования формата ID, выполняемого функцией [translateExchangeIds.](../api/user-translateexchangeids.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| sourceId | String | Идентификатор, который был преобразован. Это значение — исходный, не преобразованный идентификатор. |
| targetId | String | Преобразованный идентификатор. Это значение не присутствует, если преобразование не удалось. |
| errorDetails | [genericError](genericerror.md) | Объект ошибки, указывающий причину сбоя преобразования. Это значение не присутствует, если преобразование удалось. |

## <a name="json-representation"></a>Представление в формате JSON

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

