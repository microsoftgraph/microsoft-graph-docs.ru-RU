---
title: Тип ресурса Даилисчедуле
description: Расписание ежедневного запуска сценария управления для повторяющегося устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf0f5b59992a862b88ae663b45b6ae910ac4ba82
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942964"
---
# <a name="dailyschedule-resource-type"></a>Тип ресурса Даилисчедуле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расписание ежедневного запуска сценария управления для повторяющегося устройства.


Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|Интервал (количество дней)|

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




