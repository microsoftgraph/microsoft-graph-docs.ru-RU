---
title: тип ресурсов integerRange
description: Представляет инклюзивный диапазон наборов, описанных двумя границами Int64.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: aee4ebfab164e6abbbecde083ba028c4c5a98723
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517403"
---
# <a name="integerrange-resource-type"></a>тип ресурсов integerRange

Пространство имен: microsoft.graph

Представляет инклюзивный диапазон наборов, описанных двумя границами Int64.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|начать|Int64|Инклюзивная нижняя граница диапазона integer.|
|end|Int64|Инклюзивная верхняя граница диапазона integer.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.integerRange"
}
-->
```json
{
    "start": 12345,
    "end": 12345
}
```