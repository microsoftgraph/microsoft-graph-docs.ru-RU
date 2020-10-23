---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74800d0e4b87dbb30d8cc726b0849b12c2061647
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691374"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Тип ресурса deviceOperatingSystemSummary

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

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
|андроиддедикатедкаунт|Int32|Количество выделенных устройств с Android.|
|андроиддевицеадминкаунт|Int32|Число устройств с Android для администрирования устройств.|
|андроидфуллиманажедкаунт|Int32|Количество полностью управляемых устройств с Android.|
|андроидворкпрофилекаунт|Int32|Количество устройств с Android в рабочем профиле.|
|андроидкорпоратеворкпрофилекаунт|Int32|Количество устройств с Android для корпоративных профилей рабочих профилей. Также называется корпоративным владельцем. Допустимые значения: от 1 до 2147483647|
|конфигмгрдевицекаунт|Int32|Количество управляемых устройств ConfigMgr.|
|аоспусерлесскаунт|Int32|Количество выделенных устройств с АОСП для Android. Допустимые значения — от 0 до 2147483647|

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
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024,
  "androidCorporateWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024,
  "aospUserlessCount": 1024
}
```





