---
title: тип ресурса simulationEventsContent
description: Представляет события моделирования в кампании моделирования атак и учебной кампании.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 0a35ce8a743a358ab319388dc9aa25fe88e32dec
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979735"
---
# <a name="simulationeventscontent-resource-type"></a>тип ресурса simulationEventsContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет события моделирования в кампании моделирования атак и учебной кампании.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|compromisedRate|Двойное|Фактический процент пользователей, которые попались на имитацию атаки в кампании моделирования и обучения атак.|
|events|[коллекция simulationEvent](../resources/simulationevent.md)|Список событий моделирования в кампании моделирования атак и учебной кампании.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationEventsContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationEventsContent",
  "compromisedRate": "Double",
  "events": [
    {
      "@odata.type": "microsoft.graph.simulationEvent"
    }
  ]
}
```

