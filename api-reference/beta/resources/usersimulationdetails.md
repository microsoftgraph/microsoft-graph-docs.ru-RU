---
title: тип ресурса userSimulationDetails
description: Представляет пользователя клиента и его действия в интернете в кампании моделирования атак и обучения.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9ca7adee31eef9d197ac6ecba180be5fbaa7d697
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979760"
---
# <a name="usersimulationdetails-resource-type"></a>тип ресурса userSimulationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя клиента и действия пользователя в интернете в кампании моделирования атак и обучения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedTrainingsCount|Int32|Количество учебных занятий, назначенных пользователю в кампании моделирования атак и обучения.|
|completedTrainingsCount|Int32|Количество учебных занятий, завершимых пользователем в кампании моделирования атак и обучения.|
|compromisedDateTime|DateTimeOffset|Дата и время компрометирующего действия пользователя в ходе имитации атаки и учебной кампании.|
|inProgressTrainingsCount|Int32|Количество обучающих занятий, которые проводит пользователь в кампании моделирования и подготовки атак.|
|isCompromised|Boolean|Флаг, представляющий, был ли пользователь скомпрометирован в ходе имитации атаки и учебной кампании.|
|reportedPhishDateTime|DateTimeOffset|Дата и время, когда пользователь сообщал о доставке полезной нагрузки в качестве фишинга в кампании моделирования атак и обучения.|
|simulationEvents|[коллекция userSimulationEventInfo](../resources/usersimulationeventinfo.md)|Список событий моделирования пользователя в кампании моделирования атак и обучения.|
|simulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Пользователь в кампании моделирования атак и обучения.|
|trainingEvents|[коллекция userTrainingEventInfo](../resources/usertrainingeventinfo.md)|Список учебных событий пользователя в кампании моделирования атак и обучения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSimulationDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSimulationDetails",
  "isCompromised": "Boolean",
  "compromisedDateTime": "String (timestamp)",
  "simulationEvents": [
    {
      "@odata.type": "microsoft.graph.userSimulationEventInfo"
    }
  ],
  "trainingEvents": [
    {
      "@odata.type": "microsoft.graph.userTrainingEventInfo"
    }
  ],
  "assignedTrainingsCount": "Integer",
  "completedTrainingsCount": "Integer",
  "inProgressTrainingsCount": "Integer",
  "reportedPhishDateTime": "String (timestamp)",
  "simulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

