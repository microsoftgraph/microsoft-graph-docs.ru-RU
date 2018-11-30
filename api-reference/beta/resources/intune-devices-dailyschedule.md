---
title: Тип ресурса dailySchedule
description: График ежедневного выполнения повторяющихся сценарий управления устройства.
ms.openlocfilehash: 5d517b0bcd15f041b934a0ca936075bc6d3d3741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080479"
---
# <a name="dailyschedule-resource-type"></a>Тип ресурса dailySchedule

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

График ежедневного выполнения повторяющихся сценарий управления устройства.

Наследуется от [runSchedule](../resources/intune-devices-runschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Description|
|:---|:---|:---|
|interval|Int32|Интервал в днях|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





