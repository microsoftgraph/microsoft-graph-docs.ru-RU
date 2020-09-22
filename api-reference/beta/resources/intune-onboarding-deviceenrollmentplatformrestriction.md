---
title: Тип ресурса deviceEnrollmentPlatformRestriction
description: Ограничения на регистрацию для определенных платформ
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 255e9b815657fa354ab4180e8685049ec78ed585
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029752"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>Тип ресурса deviceEnrollmentPlatformRestriction

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничения на регистрацию для определенных платформ

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|platformBlocked|Boolean|Указывает, блокируется ли регистрация платформы|
|personalDeviceEnrollmentBlocked|Boolean|Указывает, блокируется ли регистрация личных устройств|
|osMinimumVersion|String|Минимальная поддерживаемая версия ОС|
|osMaximumVersion|String|Максимальная поддерживаемая версия ОС|
|блоккедмануфактурерс|Коллекция String|Коллекция заблокированных производителей.|

## <a name="relationships"></a>Отношения
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






