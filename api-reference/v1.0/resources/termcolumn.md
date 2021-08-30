---
author: swapnil1993
title: тип ресурсов termColumn
description: Ресурс termColumn указывает, что значения столбца содержат данные таксономии.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 38fa6fe4fdb7b08f93287305e43dddb4ec6d9331
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696780"
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

