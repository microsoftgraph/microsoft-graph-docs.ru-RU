---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01965c1dfaeb04d05d2dc6293fc449c0bbc878fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157640"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Тип ресурса deviceOperatingSystemSummary

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

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
|androidDedicatedCount|Int32|Количество выделенных устройств с Android.|
|androidDeviceAdminCount|Int32|Количество устройств администратора устройств с Android.|
|androidFullyManagedCount|Int32|Количество полностью управляемых устройств с Android.|
|androidWorkProfileCount|Int32|Количество устройств с профилем работы с Android.|
|androidCorporateWorkProfileCount|Int32|Количество устройств Android корпоративного профиля. Также известно как CORPORATE Owned Personally Enabled (СИБ). Допустимые значения : от -1 до 2 147 483 647|
|configMgrDeviceCount|Int32|Количество управляемых устройств ConfigMgr.|
|aospUserlessCount|Int32|Количество устройств с Android без пользователей AOSP. Допустимые значения: от 0 до 2 147 483 647|
|aospUserAssociatedCount|Int32|Количество устройств Android, связанных с пользователем AOSP. Допустимые значения: от 0 до 2 147 483 647|

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
  "aospUserlessCount": 1024,
  "aospUserAssociatedCount": 1024
}
```




