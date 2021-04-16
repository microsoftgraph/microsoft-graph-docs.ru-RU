---
title: Тип ресурса windowsMinimumOperatingSystem
description: Минимальная версия операционной системы, необходимая мобильному приложению для Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56e25c57e5cc73cb8ee5c42b142c6f33a1949be2
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865602"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>Тип ресурса windowsMinimumOperatingSystem

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Минимальная версия операционной системы, необходимая мобильному приложению для Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Boolean|Windows 8.0 или более поздней версии.|
|v8_1|Boolean|Windows 8.1 или более поздней версии.|
|v10_0|Boolean|Windows 10.0 или более поздней версии.|
|v10_1607|Логический|Windows 10 1607 или более поздней версии.|
|v10_1703|Логический|Windows 10 1703 или более поздней версии.|
|v10_1709|Логический|Windows 10 1709 или более поздней версии.|
|v10_1803|Логический|Windows 10 1803 или более поздней версии.|
|v10_1809|Логический|Windows 10 1809 или более поздней версии.|
|v10_1903|Логический|Windows 10 1903 или более поздней версии.|
|v10_1909|Логический|Windows 10 1909 или более поздней версии.|
|v10_2004|Логический|Windows 10 2004 или более поздней версии.|
|v10_2H20|Логический|Windows 10 2H20 или более поздней версии.|

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
  "v10_2H20": true
}
```




