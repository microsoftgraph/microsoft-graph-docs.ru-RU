---
title: Тип ресурса macOSMinimumOperatingSystem
description: Минимальные операционной системы, необходимые для приложения MacOS.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 05ea05d85ac12db5be6fc5eb18eff3bca0c87556
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938092"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>Тип ресурса macOSMinimumOperatingSystem

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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

## <a name="relationships"></a>Связи
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





