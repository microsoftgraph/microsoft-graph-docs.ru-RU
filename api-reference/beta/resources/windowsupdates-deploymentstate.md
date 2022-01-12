---
title: тип ресурса deploymentState
description: Описывает текущее состояние развертывания и контролирует его.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: e900e3ec23e50a33fabb2d9bb55cf5bfab91a3f3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61798496"
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

