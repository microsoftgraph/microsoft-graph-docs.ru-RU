---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f230ed4860e3ff8bad7968367ce5337b59521d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152887"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>Тип ресурса windowsMinimumOperatingSystem

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Минимальная версия операционной системы, необходимая мобильному приложению для Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Логический|Windows 8.0 или более поздней версии.|
|v8_1|Логический|Windows 8.1 или более поздней версии.|
|v10_0|Boolean|Windows 10.0 или более поздней версии.|
|v10_1607|Логический|Windows 10 1607 или более поздняя версия.|
|v10_1703|Логический|Windows 10 1703 или более поздняя версия.|
|v10_1709|Логический|Windows 10 1709 или более поздняя версия.|
|v10_1803|Логический|Windows 10 1803 или более поздняя версия.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true,
  "v10_1607": true,
  "v10_1703": true,
  "v10_1709": true,
  "v10_1803": true
}
```




