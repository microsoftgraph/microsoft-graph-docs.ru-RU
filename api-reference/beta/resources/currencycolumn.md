---
author: JeremyKelley
description: Ресурс currencyColumn в ресурсе columnDefinition указывает, что значения столбца представляют денежные значения.
ms.date: 09/11/2017
title: currencyColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d355d6e7226d538b214958f936d656799e999a21
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944999"
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
