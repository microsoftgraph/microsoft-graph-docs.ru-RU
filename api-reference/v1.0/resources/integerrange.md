---
title: тип ресурсов integerRange
description: Представляет инклюзивный диапазон наборов, описанных двумя границами Int64.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 6af69a7184a88d8540b45b35a58875b5d2934712fa0915bb0d1e59df2623697d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146862"
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