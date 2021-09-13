---
title: тип ресурсов integerRange
description: Представляет инклюзивный диапазон наборов, описанных двумя границами Int64.
author: nilakhan
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 31661802fa198790e4d30f2da58ac11c86f19b6e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036482"
---
# <a name="integerrange-resource-type"></a>тип ресурсов integerRange

Пространство имен: microsoft.graph

Представляет инклюзивный диапазон наборов, описанных двумя границами Int64.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|start|Int64|Инклюзивная нижняя граница диапазона integer.|
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
