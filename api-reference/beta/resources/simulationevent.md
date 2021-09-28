---
title: тип ресурсов simulationEvent
description: Представляет событие моделирования в кампании моделирования атак и учебной кампании.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5d0abb9606b549fb1349b1e98545dcf0f25e4fb7
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979731"
---
# <a name="simulationevent-resource-type"></a>тип ресурсов simulationEvent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет событие моделирования в кампании моделирования атак и учебной кампании.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|count|Int32|Количество случаев возникновения события моделирования в кампании моделирования атак и обучения.|
|eventName|Строка|Имя события моделирования в кампании имитации атаки и учебной кампании.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationEvent",
  "eventName": "String",
  "count": "Integer"
}
```

