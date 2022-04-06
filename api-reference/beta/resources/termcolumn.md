---
author: swapnil1993
title: тип ресурсов termColumn
description: Ресурс termColumn указывает, что значения столбца содержат данные таксономии.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: fcdad019f3eb2496116767e560f63a4668ed7508
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720883"
---
# <a name="termcolumn-resource-type"></a>тип ресурсов termColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Указывает, что значения столбца содержат данные таксономии.

## <a name="properties"></a>Свойства

| Свойство               | Тип                           | Описание                                                               |
| :--------------------- | :----------------------------- | :------------------------------------------------------------------------ |
| allowMultipleValues    | Boolean                        | Указывает, разрешит ли столбец несколько значений               |
| parentTerm             | microsoft.graph.termStore.term | Указывает термин guid, чьи дети могут быть выбраны в качестве значения столбца. |
| showFullyQualifiedName | Boolean                        | Указывает, отображать ли весь путь терминов или только метку терминов. |
| termSet                | microsoft.graph.termStore.set  | Termset, чьи дети могут быть выбраны в качестве значения столбца.                 |

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса **termColumn** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```
