---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bc13df043b4e49b4dce28046519be61f021c0ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012165"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>Тип ресурса windowsMinimumOperatingSystem

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Минимальная версия операционной системы, необходимая мобильному приложению для Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Boolean|Windows 8.0 или более поздней версии.|
|v8_1|Boolean|Windows 8.1 или более поздней версии.|
|v10_0|Boolean|Windows 10.0 или более поздней версии.|
|v10_1607|Boolean|Windows 10 1607 или более поздняя версия.|
|v10_1703|Boolean|Windows 10 1703 или более поздняя версия.|
|v10_1709|Boolean|Windows 10 1709 или более поздняя версия.|
|v10_1803|Boolean|Windows 10 1803 или более поздняя версия.|
|v10_1809|Boolean|Windows 10 1809 или более поздняя версия.|
|v10_1903|Boolean|Windows 10 1903 или более поздняя версия.|

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
  "v10_1803": true,
  "v10_1809": true,
  "v10_1903": true
}
```





