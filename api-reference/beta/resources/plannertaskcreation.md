---
title: Тип ресурса plannerTaskCreation
description: Содержит сведения об источнике plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e8a2a4bf3aae5f23a04c7ecb8ad043631f946b20
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883262"
---
# <a name="plannertaskcreation-resource-type"></a>Тип ресурса plannerTaskCreation

Пространство имен: microsoft.graph

Содержит сведения об источнике [plannerTask.](plannerTask.md) У этого ресурса будут либо все его свойства, либо только одно свойство будет иметь значение, которое указывает, что задача была создана процессом, `null` описанным этим свойством. Все свойства `null` указывают, что эта задача не была создана специализированным процессом. Приложениям не нужно знать источник задачи, чтобы иметь возможность работать с ней; Однако некоторые приложения могут использовать дополнительные сведения для предоставления определенных функций, которые могут быть доступны для выполнения этих задач. Дополнительные дополнительные ресурсы см. в документации.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|teamsPublicationInfo|[plannerTeamsPublicationInfo](../resources/plannerteamspublicationinfo.md)|Сведения о процессе публикации, который создал эту задачу. `null` указывает, что задача не была создана процессом публикации.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTaskCreation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskCreation",
  "teamsPublicationInfo": {
    "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
  }
}
```

