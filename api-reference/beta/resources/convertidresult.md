---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 3579385fa4c42da3d14914d134dd817c4de08ba5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016756"
---
# <a name="convertidresult-resource-type"></a>Тип ресурса Конвертидресулт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| Идентификатор | String | Преобразованный идентификатор. Это значение является исходным непреобразуемым идентификатором. |
| targetId | String | Преобразованный идентификатор. Это значение отсутствует, если произошел сбой преобразования. |
| еррордетаилс | [женерицеррор](genericerror.md) | Объект Error, указывающий причину сбоя преобразования. Это значение отсутствует, если преобразование выполнено успешно. |

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


