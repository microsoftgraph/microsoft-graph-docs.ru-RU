---
title: тип ресурса printPageRange
description: Указывает диапазон страниц, которые будут напечатаны.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 229b13a398a01412a7c85e1df954dcddffb2ed9c
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60354737"
---
# <a name="printpagerange-resource-type"></a>тип ресурса printPageRange

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает диапазон страниц, которые будут напечатаны.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|startPage|Int32|Стартовая страница (включительно) для диапазона. Только для чтения.|
|endPage|Int32|End page (включительно) для диапазона. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printPageRange"
}-->

```json
{
  "startPage": "Int32",
  "endPage": "Int32"
}
```


