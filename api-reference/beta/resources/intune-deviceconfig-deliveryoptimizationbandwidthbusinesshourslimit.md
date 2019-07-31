---
title: Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит
description: Тип часов и процентного отношения для полосы пропускания
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cbd94f135ae893e5e30ab2256ade2574efb771a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970820"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип часов и процентного отношения для полосы пропускания

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Бандвидсбегинбусинесшаурс|Int32|Указывает начало рабочего времени в 24-часовом формате (0-23). Допустимые значения — от 0 до 23.|
|Бандвидсендбусинесшаурс|Int32|Задает время окончания рабочего дня в 24-часовом формате (0-23). Допустимые значения — от 0 до 23.|
|Бандвидсперцентажедурингбусинесшаурс|Int32|Указывает процент пропускной способности для ограничения в рабочее время (0-100). Допустимые значения: от 0 до 100|
|Бандвидсперцентажеаутсидебусинесшаурс|Int32|Указывает процент пропускной способности, ограничивающий рабочие часы (0-100). Допустимые значения: от 0 до 100.|

## <a name="relationships"></a>Отношения
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





