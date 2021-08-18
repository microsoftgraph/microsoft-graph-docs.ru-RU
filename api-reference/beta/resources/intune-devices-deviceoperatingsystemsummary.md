---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5bac48206f7e002de6b837d74e4cf65d78e335af20d5d0ec4e19f2b7daa21a4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182765"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>Тип ресурса deviceOperatingSystemSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|AndroidDedicatedCount|Int32|Количество выделенных android-устройств.|
|AndroidDeviceAdminCount|Int32|Количество устройств администратора устройств Android.|
|AndroidFullyManagedCount|Int32|Количество полностью управляемых android-устройств.|
|AndroidWorkProfileCount|Int32|Количество устройств Android профиля работы.|
|AndroidCorporateWorkProfileCount|Int32|Количество устройств Android корпоративного профиля работы. Также известный как корпоративный личный включен (COPE). Допустимые значения -1 до 2147483647|
|configMgrDeviceCount|Int32|Количество управляемых устройств ConfigMgr.|
|aospUserlessCount|Int32|Количество устройств без пользователей AOSP для Android. Допустимые значения от 0 до 2147483647|
|aospUserAssociatedCount|Int32|Количество устройств Android, связанных с пользователем AOSP. Допустимые значения от 0 до 2147483647|
|LinuxCount|Int32|Количество устройств ОС Linux. Допустимые значения от 0 до 2147483647|
|chromeOSCount|Int32|Количество устройств Chrome OS. Допустимые значения от 0 до 2147483647|

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
  "aospUserAssociatedCount": 1024,
  "linuxCount": 1024,
  "chromeOSCount": 1024
}
```




