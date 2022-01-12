---
title: тип ресурса monitoringRule
description: Правило, определяющее сигнал и пороговое значение для мониторинга, а также действия, выполняемые при выполнении.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3ae09d2f4a3badf62ffa22380372e597b7fd6a4f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792185"
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

