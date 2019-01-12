---
title: Тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1b757e9c621f77d1a26251345ee6751eca2ca7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980225"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a>Тип ресурса mobileAppSupportedDeviceType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Свойства устройства
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|[deviceType](../resources/intune-shared-devicetype.md)|Тип устройства. Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.|
|minimumOperatingSystemVersion|Строка|Минимальная версия операционной системы|
|maximumOperatingSystemVersion|Строка|Максимальная версия ОС|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```





