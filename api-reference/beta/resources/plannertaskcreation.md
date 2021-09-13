---
title: тип ресурса plannerTaskCreation
description: Содержит сведения о происхождении планировщикаTask.
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 49d1ec116108cb955c353c00e59b34efe534694a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125591"
---
# <a name="plannertaskcreation-resource-type"></a>тип ресурса plannerTaskCreation

Пространство имен: microsoft.graph

Содержит сведения о происхождении [планировщикаTask](plannerTask.md). Этот ресурс будет иметь все его свойства, заданной, или точно одно свойство будет иметь значение, которое указывает, что задача была создана процессом, описанным `null` этим свойством. Все свойства указывают на то, что эта `null` задача не была создана специализированным процессом. Приложениям не нужно знать происхождение задачи, чтобы иметь возможность работать с ней; однако некоторые приложения могут использовать дополнительные сведения для предоставления определенных сведений об этих задачах. Дополнительные дополнительные возможности см. в документации по конкретным ресурсам.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|teamsPublicationInfo|[plannerTeamsPublicationInfo](../resources/plannerteamspublicationinfo.md)|Сведения о процессе публикации, создав эту задачу. `null` значение указывает, что задача не была создана в процессе публикации.|

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

