---
title: Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит
description: Тип часов и процентного отношения для полосы пропускания
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 10b02e2dc25717d2363a2db2edbf57db858cb9db
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696239"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип часов и процентного отношения для полосы пропускания

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|бандвидсбегинбусинесшаурс|Int32|Указывает начало рабочего времени в 24-часовом формате (0-23). Допустимые значения — от 0 до 23.|
|бандвидсендбусинесшаурс|Int32|Задает время окончания рабочего дня в 24-часовом формате (0-23). Допустимые значения — от 0 до 23.|
|бандвидсперцентажедурингбусинесшаурс|Int32|Указывает процент пропускной способности для ограничения в рабочее время (0-100). Допустимые значения: от 0 до 100|
|бандвидсперцентажеаутсидебусинесшаурс|Int32|Указывает процент пропускной способности, ограничивающий рабочие часы (0-100). Допустимые значения: от 0 до 100.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```





