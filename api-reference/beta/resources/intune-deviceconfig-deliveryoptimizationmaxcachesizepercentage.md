---
title: Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже
description: 'Оптимизация доставки: максимальный размер кэша типы в процентах.'
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6cd4f706009990a0257a6f58cf15dd8fce87c498
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420412"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже

Пространство имен: microsoft.graph

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



