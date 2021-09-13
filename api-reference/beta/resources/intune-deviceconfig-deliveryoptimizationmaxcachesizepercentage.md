---
title: тип ресурса deliveryOptimizationMaxCacheSizePercentage
description: Типы максимального размера кэша для оптимизации доставки.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb05fa4f38e6920d56862082d86b1d920d2bdcc7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147943"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>тип ресурса deliveryOptimizationMaxCacheSizePercentage

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Типы максимального размера кэша для оптимизации доставки.


Наследует от [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|maximumCacheSizePercentage|Int32|Указывает максимальный размер кэша, который может использовать оптимизация доставки, в процентах от размера диска (1-100). Допустимые значения от 1 до 100|

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



