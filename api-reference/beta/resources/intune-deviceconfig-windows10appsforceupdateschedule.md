---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание принудительного обновления Windows 10 для приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7041f61bfe56a12c238426864e82563c88d23f98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985932"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>Тип ресурса windows10AppsForceUpdateSchedule

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расписание принудительного обновления Windows 10 для приложений

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startDateTime|DateTimeOffset|Время начала принудительного перезапуска.|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|Расписание повторения. Возможные значения: `none`, `daily`, `weekly`, `monthly`.|
|руниммедиателифафтерстартдатетиме|Boolean|Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.|

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






