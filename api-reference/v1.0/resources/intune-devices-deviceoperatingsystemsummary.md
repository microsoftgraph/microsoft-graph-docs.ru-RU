---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ccd719ba02797d1f6d8b497666a8d48f13a2fd8
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450448"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Тип ресурса deviceOperatingSystemSummary

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Общие сведения об операционной системе устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|androidCount|Int32|Количество устройств с Android.|
|iosCount|Int32|Количество устройств с iOS.|
|macOSCount|Int32|Количество устройств с Mac OS X.|
|windowsMobileCount|Int32|Количество мобильных устройств с Windows.|
|windowsCount|Int32|Количество устройств с Windows.|
|unknownCount|Int32|Количество неизвестных устройств.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



