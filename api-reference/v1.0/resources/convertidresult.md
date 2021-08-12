---
title: тип ресурса convertIdResult
description: Результат преобразования формата ID, выполняемого функцией translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: ec94f586f0f8233f1b56965f4dea4640360b63eb43f9d1fae69988ae61d401e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155164"
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

