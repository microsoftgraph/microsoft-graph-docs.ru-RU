---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26f29427dfe863ed1b89eaef5025655dc07430fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636597"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>Тип ресурса deviceEnrollmentPlatformRestriction

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения на регистрацию для определенных платформ

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|platformBlocked|Boolean|Указывает, блокируется ли регистрация платформы|
|personalDeviceEnrollmentBlocked|Boolean|Указывает, блокируется ли регистрация личных устройств|
|osMinimumVersion|Строка|Минимальная поддерживаемая версия ОС|
|osMaximumVersion|String|Максимальная поддерживаемая версия ОС|
|блоккедмануфактурерс|Коллекция String|Коллекция заблокированных производителей.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "blockedManufacturers": [
    "String"
  ]
}
```



