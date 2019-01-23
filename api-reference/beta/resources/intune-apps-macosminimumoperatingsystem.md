---
title: Тип ресурса macOSMinimumOperatingSystem
description: Минимальные операционной системы, необходимые для приложения MacOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1b5bb3c31f876cb7444ff90cad5060c08d2f60b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425927"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>Тип ресурса macOSMinimumOperatingSystem

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Минимальные операционной системы, необходимые для приложения MacOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v10_7|Логический|Mac OS 10,7 или более поздней версии.|
|v10_8|Логический|Mac OS 10,8 или более поздней версии.|
|v10_9|Логический|Mac OS 10.9 или более поздней версии.|
|v10_10|Логический|Mac OS 10.10 или более поздней версии.|
|v10_11|Логический|Mac OS 10.11 или более поздней версии.|
|v10_12|Логический|Mac OS 10.12 или более поздней версии.|
|v10_13|Логический|Mac OS 10.13 или более поздней версии.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMinimumOperatingSystem",
  "v10_7": true,
  "v10_8": true,
  "v10_9": true,
  "v10_10": true,
  "v10_11": true,
  "v10_12": true,
  "v10_13": true
}
```




