---
title: Тип ресурса androidMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения Android.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4328cfe06180be138b2c33840c72620efdaa277b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403128"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>Тип ресурса androidMinimumOperatingSystem

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|v6_0|Логический|Версии 6.0 или более поздней версии.|
|v7_0|Логический|Версии 7.0 или более поздней версии.|
|v7_1|Логический|7.1 или более поздняя версия.|
|v8_0|Boolean|Версия 8.0 или выше.|
|v8_1|Boolean|8.1 или более поздней версии.|
|v9_0|Boolean|Версия 9.0 или выше.|

## <a name="relationships"></a>Отношения
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
  "v5_1": true,
  "v6_0": true,
  "v7_0": true,
  "v7_1": true,
  "v8_0": true,
  "v8_1": true,
  "v9_0": true
}
```




