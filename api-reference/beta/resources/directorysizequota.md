---
title: тип ресурса directorySizeQuota
description: Представляет используемую и общую квоту каталогов компании.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: 54e2280fdb416e5ccfd0853ee77a2ef3f90ddf37
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469376"
---
# <a name="directorysizequota-resource-type"></a>тип ресурса directorySizeQuota

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет используемую и общую квоту каталогов компании.

## <a name="properties"></a>Свойства
| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|used|Int32| Используемая сумма квоты каталога. |
|total|Int32| Общая сумма квоты каталога.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
