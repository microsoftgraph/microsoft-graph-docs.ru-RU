---
title: Тип ресурса macOSMinimumOperatingSystem
description: Минимальные операционной системы, необходимые для приложения MacOS.
author: tfitzmac
ms.openlocfilehash: ff9d4e3fc375f17d7b3c3efdd4af16cd7e87ceb6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354777"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>Тип ресурса macOSMinimumOperatingSystem

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Минимальные операционной системы, необходимые для приложения MacOS.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v10_7|Boolean.|Mac OS 10,7 или более поздней версии.|
|v10_8|Boolean.|Mac OS 10,8 или более поздней версии.|
|v10_9|Boolean.|Mac OS 10.9 или более поздней версии.|
|v10_10|Boolean.|Mac OS 10.10 или более поздней версии.|
|v10_11|Boolean.|Mac OS 10.11 или более поздней версии.|
|v10_12|Boolean.|Mac OS 10.12 или более поздней версии.|
|v10_13|Boolean.|Mac OS 10.13 или более поздней версии.|

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





