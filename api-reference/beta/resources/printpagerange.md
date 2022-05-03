---
title: Тип ресурса printPageRange
description: Указывает диапазон страниц для печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: a8bd855bc4b7d561d9157923d7ce3ace8323b899
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176890"
---
# <a name="printpagerange-resource-type"></a>Тип ресурса printPageRange

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает диапазон страниц для печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Начальная страница|Int32|Начальная страница (включительно) для диапазона. Только для чтения.|
|endPage|Int32|Конечная страница (включительно) для диапазона. Только для чтения.|

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


