---
author: JeremyKelley
description: Ресурс currencyColumn в ресурсе columnDefinition указывает, что значения столбца представляют денежные значения.
ms.date: 09/11/2017
title: currencyColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 037a5f5a0e3c8e6f5b3a69e2dd1066c3960948ca
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722792"
---
# <a name="currencycolumn-resource-type"></a>Тип ресурса currencyColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **currencyColumn** в формате JSON.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a>Свойства

| Свойство   | Тип   | Описание                                                   |
| :--------- | :----- | :------------------------------------------------------------ |
| **locale** | string | Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы. |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": []
}
-->
