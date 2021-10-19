---
title: тип ресурса directorySizeQuota
description: Представляет используемую и общую квоту каталогов компании.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: ac8b26fababe53458b8dd3a92624d9ce0a11514a
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60483017"
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
  "used": "Int32",
  "total": "Int32"
}
```
