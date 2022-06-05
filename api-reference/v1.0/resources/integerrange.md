---
title: Тип ресурса integerRange
description: Представляет инклюзивный диапазон целых чисел, описанных двумя границами Int64.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b869d99fc4fef8b6804a3559ddd21e7d661ea32b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899437"
---
# <a name="integerrange-resource-type"></a>Тип ресурса integerRange

Пространство имен: microsoft.graph

Представляет инклюзивный диапазон целых чисел, описанных двумя границами Int64.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|start|Int64|Инклюзивная нижняя граница целочисленного диапазона.|
|end|Int64|Инклюзивная верхняя граница целочисленного диапазона.|

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
