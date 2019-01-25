---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
ms.openlocfilehash: b3a0d76a236cc4bce53bf476a90e8f37757ae003
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512628"
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
| **format**     | string  | Для типов выходных данных `dateTime` это свойство указывает формат значения. Должно иметь тип `dateOnly` или `dateTime`.
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
  "suppressions": [
    "Error: /api-reference/beta/resources/calculatedColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
