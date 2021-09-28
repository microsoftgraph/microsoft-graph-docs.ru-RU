---
title: тип ресурсов simulationReportOverview
description: Представляет отчет об имитации атаки и учебной кампании.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5f096dbe931959707ad067ce3d11fcf0afac4bdb
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979798"
---
# <a name="simulationreportoverview-resource-type"></a>тип ресурсов simulationReportOverview

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет обзор кампании моделирования атак и учебной кампании.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|recommendedActions|[коллекция recommendedAction](../resources/recommendedaction.md)|Список рекомендуемых действий для клиента по улучшению его осанки безопасности в зависимости от типа атаки и типа атаки учебной кампании.|
|resolvedTargetsCount|Int32|Количество допустимых пользователей в кампании моделирования и обучения атак.|
|simulationEventsContent|[simulationEventsContent](../resources/simulationeventscontent.md)|Сводка событий моделирования в кампании моделирования атак и обучения.|
|trainingEventsContent|[trainingEventsContent](../resources/trainingeventscontent.md)|Сводка назначенных тренингов в кампании моделирования атак и обучения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationReportOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationReportOverview",
  "resolvedTargetsCount": "Integer",
  "simulationEventsContent": {
    "@odata.type": "microsoft.graph.simulationEventsContent"
  },
  "trainingEventsContent": {
    "@odata.type": "microsoft.graph.trainingEventsContent"
  },
  "recommendedActions": [
    {
      "@odata.type": "microsoft.graph.recommendedAction"
    }
  ]
}
```

