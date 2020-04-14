---
title: Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте
description: 'Максимальный размер кэша для оптимизации доставки: абсолютный тип.'
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a15b1bfea6da2af43c360ff143d8bb55bc44f6b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420459"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Максимальный размер кэша для оптимизации доставки: абсолютный тип.


Наследуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|максимумкачесизеингигабитес|Int64|Задает максимальный размер кэша оптимизации доставки в ГБ. Допустимые значения — от 0 до 4294967295
Значение 0 (ноль) означает "неограниченный" кэш. При оптимизации доставки кэш очищается, когда на устройстве заканчивается свободное место на диске. Допустимые значения — от 0 до 4294967295|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```



