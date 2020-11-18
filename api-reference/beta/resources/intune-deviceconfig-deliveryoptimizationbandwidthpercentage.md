---
title: Тип ресурса Деливерйоптимизатионбандвидсперцентаже
description: Пределы пропускной способности, указанные в процентах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85dc858431b15a142a42afc74b1b7c1ba76a4667
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199611"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a>Тип ресурса Деливерйоптимизатионбандвидсперцентаже

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пределы пропускной способности, указанные в процентах.


Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|максимумбаккграундбандвидсперцентаже|Int32|Указывает максимальную пропускную способность загрузки в фоновом режиме, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100). Допустимые значения: от 0 до 100
Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется для использования доступной полосы пропускания для загрузки в фоновом режиме. Допустимые значения: от 0 до 100|
|максимумфореграундбандвидсперцентаже|Int32|Указывает максимальную полосу пропускания при загрузке переднего плана, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100). Допустимые значения: от 0 до 100
Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загрузки в фоновом режиме. Допустимые значения: от 0 до 100.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```




