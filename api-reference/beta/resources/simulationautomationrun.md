---
title: тип ресурсов simulationAutomationRun
description: Представляет собой запуск автоматизации имитации атак на клиента.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d5ca41d575ec90e150e8f0d54a37f0278b6b6bdb
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758345"
---
# <a name="simulationautomationrun-resource-type"></a>тип ресурсов simulationAutomationRun

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет собой запуск автоматизации имитации атак на клиента.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Выполняется список](../api/simulationautomation-list-runs.md)|[коллекция simulationAutomationRun](../resources/simulationautomationrun.md)|Получите список запусков автоматизации имитации атак.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|endDateTime|DateTimeOffset|Дата и время окончания запуска в автоматизации имитации атак.|
|id|String|Уникальный идентификатор для запуска автоматизации имитации атак.|
|simulationId|String|Уникальный идентификатор для кампании моделирования атак, начатой в запуске автоматизации атак.|
|startDateTime|DateTimeOffset|Дата и время запуска в автоматизации моделирования атак.|
|status|[simulationAutomationRunStatus](#simulationautomationrunstatus-values)|Состояние запуска автоматизации имитации атак. Допустимые значения: `unknown`, `running`, `succeeded`, `failed`, `skipped`, `unknownFutureValue`.|

### <a name="simulationautomationrunstatus-values"></a>simulationAutomationRunStatus values

|Member|Описание |
|:---|:---|
|unknown| Состояние запуска автоматизации моделирования не определено. |
|запуск| Запущена автоматизация моделирования. |
|успешно| Успешного запуска автоматизации моделирования. |
|не удалось| Запуск автоматизации моделирования не удалось. |
|пропущено| Запуск автоматизации моделирования был пропущен. |
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulationAutomationRun",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationAutomationRun",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "simulationId": "String",
  "startDateTime": "String (timestamp)",
  "status": "String"
}
```

