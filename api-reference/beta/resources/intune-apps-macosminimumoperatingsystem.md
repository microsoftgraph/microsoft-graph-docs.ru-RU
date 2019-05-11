---
title: Тип ресурса Макосминимумоператингсистем
description: Минимальная операционная система, необходимая для приложения MacOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 596b4e6de349528d6e6d5d5524918de084936417
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950230"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>Тип ресурса Макосминимумоператингсистем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Минимальная операционная система, необходимая для приложения MacOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v10_7|Логический|Mac OS 10,7 или более поздней версии.|
|v10_8|Логический|Mac OS 10,8 или более поздней версии.|
|v10_9|Логический|Mac OS 10,9 или более поздней версии.|
|v10_10|Логический|Mac OS 10,10 или более поздней версии.|
|v10_11|Логический|Mac OS 10,11 или более поздней версии.|
|v10_12|Логический|Mac OS 10,12 или более поздней версии.|
|v10_13|Логический|Mac OS 10,13 или более поздней версии.|

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




