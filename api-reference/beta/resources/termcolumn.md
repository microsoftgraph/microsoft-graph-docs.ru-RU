---
author: swapnil1993
title: тип ресурсов termColumn
description: Ресурс termColumn указывает, что значения столбца содержат данные таксономии.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6ccf926f646f11f12bc150fd22b339777df4208b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757747"
---
# <a name="termcolumn-resource-type"></a>тип ресурсов termColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Указывает, что значения столбца содержат данные таксономии.

## <a name="properties"></a>Свойства

| Свойство               | Тип                           | Описание                                                               |
| :--------------------- | :----------------------------- | :------------------------------------------------------------------------ |
| allowMultipleValues    | Логический                        | Указывает, разрешит ли столбец несколько значений               |
| showFullyQualifiedName | Логическое                        | Указывает, отображать ли весь путь терминов или только метку терминов. |

## <a name="relationships"></a>Связи

| Связь   | Тип                      | Описание
|:----------------|:--------------------------|:-------------------------------
| parentTerm     | microsoft.graph.termStore.term | Указывает родительский термин, для которого можно выбрать термины ребенка в качестве столбца.
| termSet      | microsoft.graph.termStore.set | Termset, чьи дети могут быть выбраны в качестве значения столбца.

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса **termColumn** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "showFullyQualifiedName": false,
}
```
