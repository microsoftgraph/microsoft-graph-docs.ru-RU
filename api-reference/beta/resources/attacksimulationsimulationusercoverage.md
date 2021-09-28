---
title: тип ресурса attackSimulationSimulationUserCoverage
description: Представляет освещение моделирования для пользователя в имитации атаки и обучении.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9caef11c29dbe003047d1013340c1fdae193d0d6
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979728"
---
# <a name="attacksimulationsimulationusercoverage-resource-type"></a>тип ресурса attackSimulationSimulationUserCoverage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет накопительные данные моделирования и результаты для пользователя в моделировании атак и обучении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Пользователь в кампании моделирования атак и обучения.|
|clickCount|Int32|Количество нажатий ссылок в полученных полезной нагрузке пользователя в кампаниях моделирования атак и обучения.|
|compromisedCount|Int32|Количество компрометирующих действий пользователя в имитации атак и учебных кампаниях.|
|latestSimulationDateTime|DateTimeOffset|Дата и время последнего моделирования атаки и учебной кампании, в которую был включен пользователь.|
|simulationCount|Int32|Количество кампаний моделирования атак и учебных кампаний, в которые был включен пользователь.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationSimulationUserCoverage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationSimulationUserCoverage",
  "simulationCount": "Integer",
  "latestSimulationDateTime": "String (timestamp)",
  "clickCount": "Integer",
  "compromisedCount": "Integer",
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

