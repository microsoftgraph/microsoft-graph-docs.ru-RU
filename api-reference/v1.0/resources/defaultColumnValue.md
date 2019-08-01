---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: Ресурс defaultColumnValue в ресурсе columnDefinition указывает значение, используемое по умолчанию, для этого столбца.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a2ddff8de7efb2bb697ffae63d69376588e6ac9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029514"
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
