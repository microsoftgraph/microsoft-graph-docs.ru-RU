---
author: swapnil1993
title: тип ресурсов termColumn
description: Ресурс termColumn указывает, что значения столбца содержат данные таксономии.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d89d389b78c4c8dc1a370722a5b40c7cff794d3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128041"
---
# <a name="termcolumn-resource-type"></a>тип ресурсов termColumn

Пространство имен: microsoft.graph

Представляет столбец управляемых метаданных в SharePoint.

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание|
|:--------------|:-------|:----------------------------------------------------|
| allowMultipleValues | Логический | Указывает, разрешит ли столбец несколько значений.|
| parentTerm     | microsoft.graph.termStore.term | Указывает термин GUID, чьи дети могут быть выбраны в качестве значения столбца.  |
| showFullyQualifiedName | Логический | Указывает, отображать ли весь путь терминов или только метку терминов.  |
| termSet      | microsoft.graph.termStore.set | Termset, чьи дети могут быть выбраны в качестве значения столбца. |

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса **termColumn.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```

