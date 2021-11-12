---
title: тип ресурса monitoringRule
description: Правило, определяющее сигнал и пороговое значение для мониторинга, а также действия, выполняемые при выполнении.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 376de8e06d5fee242dc068362a4daaa99c977cd2
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890439"
---
# <a name="monitoringrule-resource-type"></a>тип ресурса monitoringRule

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Правило, определяющее сигнал и пороговое значение для мониторинга, а также действия, выполняемые при выполнении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|action|microsoft.graph.windowsUpdates.monitoringAction|    Действие, срабатывае при превышении порогового значения для данного сигнала. Возможные значения: `alertError`, `pauseDeployment`, `unknownFutureValue`.|
|сигнал|microsoft.graph.windowsUpdates.monitoringSignal|Сигнал для мониторинга. Возможные значения: `rollback`, `unknownFutureValue`.|
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

