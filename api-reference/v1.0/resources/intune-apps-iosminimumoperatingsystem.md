---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f3402155831e5cd77de26f13966061b0a7092a5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474574"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>Тип ресурса iosMinimumOperatingSystem

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Логический|Версия 8.0 или выше.|
|v9_0|Логический|Версия 9.0 или выше.|
|v10_0|Логический|Версия 10.0 или выше.|
|v11_0|Boolean|Версия 11.0 или выше.|
|v12_0|Логический|Версия 12,0 или более поздняя.|
|v13_0|Логический|Версия 13,0 или более поздняя.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true,
  "v13_0": true
}
```







