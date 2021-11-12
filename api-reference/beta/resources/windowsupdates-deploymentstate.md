---
title: тип ресурса deploymentState
description: Описывает текущее состояние развертывания и контролирует его.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 80b691c6404bac3e98c4c5c6acb9596b5d4c8821
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890831"
---
# <a name="deploymentstate-resource-type"></a>тип ресурса deploymentState

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает текущее состояние развертывания и контролирует его.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|причины|[коллекция microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md)|Указывает причины, по которой развертывание имеет свое значение состояния. Только для чтения.|
|requestedValue|microsoft.graph.windowsUpdates.requestedDeploymentStateValue|Указывает запрашиваемого состояния развертывания. Поддерживает подмножество значений **для запрашиваемогоDeploymentStateValue.** Возможные значения: `none`, `paused`, `unknownFutureValue`.|
|значение|microsoft.graph.windowsUpdates.deploymentStateValue|Указывает состояние развертывания. Поддерживает подмножество значений **для deploymentStateValue.** Возможные значения: `scheduled`, `offering`, `paused`, `unknownFutureValue`. Только для чтения.|

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

