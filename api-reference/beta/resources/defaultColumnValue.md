---
author: daspek
description: Ресурс defaultColumnValue в ресурсе columnDefinition указывает значение, используемое по умолчанию, для этого столбца.
ms.date: 09/12/2017
title: DefaultColumnValue
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 3c45329a44a5023b10950f49ef568d8be071e6db
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723509"
---
# <a name="defaultcolumnvalue-resource-type"></a>Тип ресурса defaultColumnValue

Пространство имен: microsoft.graph

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

| Свойство    | Тип   | Описание                                                    |
| :---------- | :----- | :------------------------------------------------------------- |
| **formula** | string | Формула, используемая для вычисления значения, используемого по умолчанию, для данного столбца. |
| **value**   | string | Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.  |

Одновременно можно указать только одну **формулу** или одно **значение**.

В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.
Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": []
}
-->
