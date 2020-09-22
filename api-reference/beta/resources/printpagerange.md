---
title: Тип ресурса Принтпажеранже
description: Указывает диапазон страниц для печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a8bbf452c337cb5c2ade7302eb29cff4bdb73d23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052544"
---
# <a name="printpagerange-resource-type"></a>Тип ресурса Принтпажеранже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает диапазон страниц для печати.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|startPage|Int32|Начальная страница диапазона (включающая). Только для чтения.|
|ендпаже|Int32|Конечная страница диапазона (включающая). Только для чтения.|

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
  "startPage": 123456,
  "endPage": 123456
}
```


