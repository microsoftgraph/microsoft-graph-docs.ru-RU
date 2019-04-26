---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
ms.openlocfilehash: e09fab8a6bd59b0a878dfe6c70bd040612ce3b8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328302"
---
# <a name="calculatedcolumn-resource-type"></a>Тип ресурса calculatedColumn

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **calculatedColumn** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание
|:---------------|:--------|:--------------------------------------------------
| **format**     | строка  | Для типов выходных данных `dateTime` это свойство указывает формат значения. Должно иметь тип `dateOnly` или `dateTime`.
| **formula**    | string  | Формула, используемая для вычисления значения для данного столбца.
| **outputType** | string  | Тип выходных данных, используемый для форматирования значений в этом столбце. Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.

В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.
Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": []
}
-->
