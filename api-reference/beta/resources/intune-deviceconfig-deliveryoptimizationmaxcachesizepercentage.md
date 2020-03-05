---
title: Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже
description: 'Оптимизация доставки: максимальный размер кэша типы в процентах.'
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f5ef7bef4f86f78207df37dcb684b714c93b8d5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526746"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Оптимизация доставки: максимальный размер кэша типы в процентах.


Наследуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|максимумкачесизеперцентаже|Int32|Задает максимальный размер кэша, который может использовать оптимизация доставки, в процентах от размера диска (1-100). Допустимые значения — от 1 до 100|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```



