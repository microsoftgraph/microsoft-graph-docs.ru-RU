---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 091ef44a52e20acb987adddbac1c561087db718c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368314"
---
# <a name="devicegeolocation-resource-type"></a>Тип ресурса deviceGeoLocation

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Расположение устройства

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastCollectedDateTime|DateTimeOffset|Время записи расположения относительно времени UTC|
|longitude|Двойное с плавающей точкой|Долгота расположения устройства|
|latitude|Двойное с плавающей точкой|Широта расположения устройства|
|altitude|Двойное с плавающей точкой|Высота (метров над уровнем моря)|
|horizontalAccuracy|Двойное с плавающей точкой|Точность долготы и широты (м)|
|verticalAccuracy|Двойное с плавающей точкой|Точность высоты (м)|
|heading|Двойное с плавающей точкой|Направление от географического севера (градусов)|
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







