---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 69e097d433d774c3dd445c94cd29eb059292806f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091231"
---
# <a name="devicegeolocation-resource-type"></a>Тип ресурса deviceGeoLocation

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расположение устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastCollectedDateTime|DateTimeOffset|Время записи расположения относительно времени UTC|
|longitude|Double|Долгота расположения устройства|
|latitude|Double|Широта расположения устройства|
|altitude|Double|Высота (метров над уровнем моря)|
|horizontalAccuracy|Double|Точность долготы и широты (м)|
|verticalAccuracy|Double|Точность высоты (м)|
|heading|Double|Направление от географического севера (градусов)|
|speed|Double|Скорость передвижения устройства (м/с)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```









