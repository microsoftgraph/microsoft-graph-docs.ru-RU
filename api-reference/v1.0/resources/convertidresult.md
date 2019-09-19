---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 405d663e4f1f7fb040e79cdd10669bc824e3edef
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036447"
---
# <a name="convertidresult-resource-type"></a>Тип ресурса Конвертидресулт

Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
| Идентификатор | String. | Преобразованный идентификатор. Это значение является исходным непреобразуемым идентификатором. |
| targetId | String. | Преобразованный идентификатор. Это значение отсутствует, если произошел сбой преобразования. |
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
