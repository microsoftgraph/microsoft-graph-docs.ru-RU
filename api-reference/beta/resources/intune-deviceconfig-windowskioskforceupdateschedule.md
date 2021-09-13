---
title: тип ресурса windowsKioskForceUpdateSchedule
description: Windows 10 расписания принудительного обновления для устройств Киоска.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 417ca7a81b14c51f1f9876618dc68e5b65f961c1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086514"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a>тип ресурса windowsKioskForceUpdateSchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows 10 расписания принудительного обновления для устройств Киоска.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Время начала перезапуска силы.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Расписание повторения. Возможные значения: `none`, `daily`, `weekly`, `monthly`.|
|dayofWeek|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|День недели. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|dayofMonth|Int32|День месяца. Допустимые значения от 1 до 31|
|runImmediatelyIfAfterStartDateTime|Логическое|Если верно, выполняет задачу немедленно, если StartDateTime находится в прошлом, то в другом случае выполняется при следующем повторе.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```



