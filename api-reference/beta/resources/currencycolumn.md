---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
ms.openlocfilehash: 179c0bb1e5c82d7f2af17dcbcae08be8726f2ecd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888937"
---
# <a name="currencycolumn-resource-type"></a>Тип ресурса currencyColumn

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| **locale**    | строка | Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
