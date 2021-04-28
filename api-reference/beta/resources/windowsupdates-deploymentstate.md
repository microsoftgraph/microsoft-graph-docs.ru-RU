---
title: тип ресурса deploymentState
description: Описывает текущее состояние развертывания и контролирует его.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d05bf09fbad405e93ee994858e2d6ac65a8088a7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067487"
---
# <a name="deploymentstate-resource-type"></a>тип ресурса deploymentState

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает текущее состояние развертывания и контролирует его.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|причины|[коллекция microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md)|Указывает причины, по которой развертывание имеет свое значение состояния. Только для чтения.|
|requestedValue|microsoft.graph.windowsUpdates.requestedDeploymentStateValue|Указывает запрашиваемого состояния развертывания. Поддерживает подмножество значений **для запрашиваемогоDeploymentStateValue.** Возможные значения: `none`, `paused`.|
|значение|microsoft.graph.windowsUpdates.deploymentStateValue|Указывает состояние развертывания. Поддерживает подмножество значений **для deploymentStateValue.** Возможные значения: `scheduled`, `offering`, `paused`. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentState",
  "value": "String",
  "reasons": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
    }
  ],
  "requestedValue": "String",
}
```

