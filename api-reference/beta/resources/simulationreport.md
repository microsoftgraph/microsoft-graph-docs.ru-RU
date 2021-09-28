---
title: тип ресурса simulationReport
description: Представляет отчет о имитации атаки и учебной кампании.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8f3e5991192d3d3f72e37e8ac5117a01d0138369
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979759"
---
# <a name="simulationreport-resource-type"></a>тип ресурса simulationReport

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отчет о имитации атаки и учебной кампании, включая обзор и пользователей кампании.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|обзор|[simulationReportOverview](../resources/simulationreportoverview.md)|Обзор кампании моделирования атак и учебной кампании.|
|simulationUsers|[коллекция userSimulationDetails](../resources/usersimulationdetails.md)|Представляет пользователей клиента и его действия в интернете в кампании моделирования атак и обучения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationReport"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationReport",
  "overview": {
    "@odata.type": "microsoft.graph.simulationReportOverview"
  },
  "simulationUsers": [
    {
      "@odata.type": "microsoft.graph.userSimulationDetails"
    }
  ]
}
```

