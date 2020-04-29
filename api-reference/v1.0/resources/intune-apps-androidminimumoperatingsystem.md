---
title: Тип ресурса androidMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef599e37033c6c0e1e101925559560d6a970bbae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397361"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>Тип ресурса androidMinimumOperatingSystem

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения Android.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v4_0|Boolean|Версия 4.0 или выше.|
|v4_0_3|Boolean|Версия 4.0.3 или выше.|
|v4_1|Boolean|Версия 4.1 или выше.|
|v4_2|Boolean|Версия 4.2 или выше.|
|v4_3|Boolean|Версия 4.3 или выше.|
|v4_4|Boolean|Версия 4.4 или выше.|
|v5_0|Boolean|Версия 5.0 или выше.|
|v5_1|Boolean|Версия 5.1 или выше.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true
}
```







