---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: defaultColumnValue
localization_priority: Normal
ms.openlocfilehash: ad94cadaa26d0fab72236d4037ceffd09a52c561
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514280"
---
# <a name="defaultcolumnvalue-resource-type"></a>Тип ресурса defaultColumnValue

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **defaultColumnValue** в ресурсе [columnDefinition](columndefinition.md) указывает значение, используемое по умолчанию, для этого столбца.
Значение, используемое по умолчанию, можно указать либо непосредственно, либо в виде формулы.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **defaultColumnValue** в формате JSON.
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| **formula**   | string | Формула, используемая для вычисления значения, используемого по умолчанию, для данного столбца.
| **value**     | string | Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.

Одновременно можно указать только одну **формулу** или одно **значение**.

В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.
Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": [
    "Error: /api-reference/beta/resources/defaultColumnValue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
