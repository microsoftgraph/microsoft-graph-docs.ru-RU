---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: defaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 400fc25bf38f12db2be8cef21ddc351316d1265b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810593"
---
# <a name="defaultcolumnvalue-resource-type"></a>Тип ресурса defaultColumnValue

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


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
