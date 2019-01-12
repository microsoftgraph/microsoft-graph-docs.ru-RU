---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание обновления force Windows 10 для приложения
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 50793ee4ba26adc4b89cc8d36b3e8186debc402a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981989"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>Тип ресурса windows10AppsForceUpdateSchedule

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Расписание обновления force Windows 10 для приложения
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Перезапустите время начала для сотрудников.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Расписание повторения. Возможные значения: `none`, `daily`, `weekly`, `monthly`.|
|runImmediatelyIfAfterStartDateTime|Логический|Если значение true, если StartDateTime в прошлом else, будет выполняться в следующего повторения немедленно запускается задание.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```





