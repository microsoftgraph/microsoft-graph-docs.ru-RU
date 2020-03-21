---
title: Тип ресурса Принтпажеранже
description: Указывает диапазон страниц для печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 65e2455438dbdb8c7bef3ef3439f846e737ebba0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895987"
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
