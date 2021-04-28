---
title: тип ресурса monitoringRule
description: Правило, определяющее сигнал и пороговое значение для мониторинга, а также действия, выполняемые при выполнении.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 305db31c935329574a2b7d52403dc7664ff53f66
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068088"
---
# <a name="monitoringrule-resource-type"></a>тип ресурса monitoringRule

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Правило, определяющее сигнал и пороговое значение для мониторинга, а также действия, выполняемые при выполнении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|microsoft.graph.windowsUpdates.monitoringAction|    Действие, срабатывае при превышении порогового значения для данного сигнала. Возможные значения: `alertError`, `pauseDeployment`.|
|сигнал|microsoft.graph.windowsUpdates.monitoringSignal|Сигнал для мониторинга. Возможные значения: `rollback` .|
|пороговое значение|Int32|Пороговое значение для сигнала, с которого можно запускать действие. Включительно от 1 до 100 ( включительно).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
  "signal": "String",
  "threshold": "Integer",
  "action": "String"
}
```

