---
title: тип ресурса trainingEventsContent
description: Представляет обучающие события в кампании моделирования атак и учебной кампании.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 489e3b996f86a28f1d555489a30861e5251229f8
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979810"
---
# <a name="trainingeventscontent-resource-type"></a>тип ресурса trainingEventsContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет обучающие события в кампании моделирования атак и учебной кампании.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedTrainingsInfos|[коллекция assignedTrainingInfo](../resources/assignedtraininginfo.md)|Список назначенных тренингов и их сведений в кампании моделирования атак и обучения.|
|trainingsAssignedUserCount|Int32|Количество пользователей, которым назначены тренинги в кампании моделирования атак и обучения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.trainingEventsContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trainingEventsContent",
  "trainingsAssignedUserCount": "Integer",
  "assignedTrainingsInfos": [
    {
      "@odata.type": "microsoft.graph.assignedTrainingInfo"
    }
  ]
}
```

