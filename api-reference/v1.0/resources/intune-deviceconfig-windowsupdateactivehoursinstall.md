---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 556e0f22bb249a8606b3bbf9bb3252d3721793b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845740"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a>Тип ресурса windowsUpdateActiveHoursInstall

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д

Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|activeHoursStart|TimeOfDay|Время начала периода активности|
|activeHoursEnd|TimeOfDay|Время окончания периода активности|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



