---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03d270408e383d21cb63cb512dcccb58a155cb08
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256089"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>Тип ресурса windowsMinimumOperatingSystem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Минимальная версия операционной системы, необходимая мобильному приложению для Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Boolean|Windows 8.0 или более поздней версии.|
|v8_1|Boolean|Windows 8.1 или более поздней версии.|
|v10_0|Boolean|Windows 10.0 или более поздней версии.|
|v10_1607|Логический|Windows 10 1607 или более поздней.|
|v10_1703|Логический|Windows 10 1703 или более поздней.|
|v10_1709|Логический|Windows 10 1709 или более поздней.|
|v10_1803|Логический|Windows 10 1803 или более поздней.|
|v10_1809|Логический|Windows 10 1809 или более поздней.|
|v10_1903|Логический|Windows 10 1903 или более поздней.|
|v10_1909|Логический|Windows 10 1909 или более поздней.|
|v10_2004|Логический|Windows 10 2004 или более поздней.|
|v10_2H20|Логический|Windows 10 2H20 или более поздней.|
|v10_21H1|Логический|Windows 10 21H1 или более поздней.|

## <a name="relationships"></a>Связи
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
  "v10_1903": true,
  "v10_1909": true,
  "v10_2004": true,
  "v10_2H20": true,
  "v10_21H1": true
}
```




