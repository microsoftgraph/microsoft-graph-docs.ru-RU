---
title: Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте
description: 'Максимальный размер кэша для оптимизации доставки: абсолютный тип.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a955197e1e75ecb1f953f5ddc50b33b7e01a574b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565879"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Максимальный размер кэша для оптимизации доставки: абсолютный тип.


НаСледуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Максимумкачесизеингигабитес|Int64|Задает максимальный размер кэша оптимизации доставки в ГБ. Допустимые значения — от 0 до 4294967295
Значение 0 (ноль) означает "неограниченный" кэш. При оптимизации доставки кэш очищается, когда на устройстве заканчивается свободное место на диске. Допустимые значения — от 0 до 4294967295|

## <a name="relationships"></a>Отношения
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





