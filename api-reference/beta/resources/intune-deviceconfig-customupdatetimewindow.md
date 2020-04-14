---
title: Тип ресурса Кустомупдатетимевиндов
description: Настраиваемое окно времени обновления
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b7a83637e3462d33745a14dead15eb86cbb86337
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402170"
---
# <a name="customupdatetimewindow-resource-type"></a>Тип ресурса Кустомупдатетимевиндов

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настраиваемое окно времени обновления

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|стартдай|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|День начала периода времени. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|енддай|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|День окончания периода времени. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|startTime|TimeOfDay|Время начала периода времени|
|endTime|TimeOfDay|Время окончания периода времени|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```



