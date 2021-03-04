---
author: swapnil1993
title: тип ресурсов termColumn
description: Ресурс termColumn указывает, что значения столбца содержат данные таксономии.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6d29ec570d7f3fad798fb1e2ba213b5a998643dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447466"
---
# <a name="termcolumn-resource-type"></a>тип ресурсов termColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Указывает, что значения столбца содержат данные таксономии.

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| allowMultipleValues | Boolean | Указывает, разрешит ли столбец несколько значений   
| parentTerm     | microsoft.graph.termStore.term | Указывает термин guid, чьи дети могут быть выбраны в качестве значения столбца.  
| showFullyQualifiedName | Boolean | Указывает, отображать ли весь путь терминов или только метку терминов.  
| termSet      | microsoft.graph.termStore.set | Termset, чьи дети могут быть выбраны в качестве значения столбца. 

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

